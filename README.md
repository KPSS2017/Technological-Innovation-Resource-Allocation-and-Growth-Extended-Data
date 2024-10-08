# Extended Data (till 2023) following Kogan, L., Papanikolaou, D., Seru, A. and Stoffman, N., 2017 
 
This data provides an updated data series for KPSS values and forward citations, a patent number to the CRSP "permno" match and a patent number to CPC class match following the paper **Kogan, L., Papanikolaou, D., Seru, A. and Stoffman, N., 2017. Technological innovation, resource allocation, and growth. Quarterly Journal of Economics, 132(2), pp. 665-712.** The paper is available at https://academic.oup.com/qje/article/132/2/665/3076284.
 

## Data

#### Data Versions:

The version released on August 9, 2020 is the latest data that updates and adds data for the second half of 2019.

The version released on August 21, 2020 adds filing date information for each patent.

The version released on September 6, 2020 updates filing date information for each patent.

The version released on June 8, 2021 is the latest data that updates and adds data for 2020.

The version released on May 10, 2023 is the latest data that updates until the end of 2022.

The version released on Oct 7, 2024 is the latest data that updates until the end of 2023.


#### Data Description:

We provide three data sets constructed from the paper here:

- **KPSS_2023.csv**: Patent level panel data from 1926 to 2023
- **Match_patent_permco_permno_2023.csv**: Patent-CRSP permco and permno match data from 1926 to 2023
- **Match_patent_cpc_2023.csv**: Patent-CPC class match data from 1926 to 2023

For the patent level panel data, the variable definitions are:

| Variable name  | Definition                                         | 
| :---------------|:------------------------------------------------- | 
| patent_num     | Patent ID number                                   |
| permno         | CRSP permno                                        |  
| issue_date     | Issue date of patent (mm/dd/yyyy)                  |  
| filing_date     | Filing date of patent application(mm/dd/yyyy)              |   
| xi_nominal    | Value of innovation(&xi;) in millions of nominal dollars |
| xi_real  | Value of innovation(&xi;) deflated to 1982 (million) dollars using the CPI|
| cites | Forward citations |

For the patent-permco-permno match data, the variable definitions are:

| Variable name  | Definition                                         | 
| :--------------|:-------------------------------------------------- | 
| patent_num     | Patent ID number                                   |
| permco         | CRSP permco                                        | 
| permno         | CRSP permno                                        |  

For the patent-CPC class match data, the variable definitions are:

| Variable name  | Definition                                            | 
| :--------------|:------------------------------------------------------- | 
| patent_num    | Patent ID number                                    |
| cpc            | Full CPC class of patent                           | 


## Notes:

1. The value of innovation(xi_real) is equal to the nominal value of innovation(xi_nominal) deflated to 1982 (million) dollars using the CPI. In other word, we can simply calculate the xi_real through the following equation: xi_real = xi_nominal / CPI * 100.

2. We drop patents in the dataset that were assigned to multiple CRSP permnos.

3. The updated KPSS values differ slightly from the data in the QJE paper for any of the following reasons:

	a)	Changes in the CRSP dataset over time.

	b)	Improvements in the matching process to firms.

	c)	Re-estimation of the parameters needed to compute the KPSS value: 

	- The newly estimated gamma in the 2023 updated sample is 0.0155. This estimate was 0.0143 in 2022, 0.0142 in 2021, 0.0138 in 2020, and 0.0146 in the QJE paper.

	- Stock return volatility is now computed over the last 52 weeks for stocks with at least 20 days non-missing data (as opposed to the previous calendar year in the QJE paper).

4. Till 2023, there are 3,308 patents in KPSS dataset do not have CPC information; they're reflected as missing values in the match Patent-CPC dataset. 

5. The number of forward citations is also updated to 2023. 

6. The datasets we provided on GitHub may exceed the download limit of your web browser. You may need to Git Clone this repository to local machine in order to download the zipped csv files in such cases.

## Contact:

Please contact Dimitris Papanikolaou (d-papanikolaou@kellogg.northwestern.edu) or Amit Seru (aseru@stanford.edu) for any questions regarding the data.

**Please see the paper for more information on the data. If you use these data sets, please CITE this paper as the data source.**
