# Extended Data (till 2019) following Kogan, L., Papanikolaou, D., Seru, A. and Stoffman, N., 2017 
 
This data provides an updated data series for KPSS values and forward citations and a patent number to the CRSP "permno" match following the paper **Kogan, L., Papanikolaou, D., Seru, A. and Stoffman, N., 2017. Technological innovation, resource allocation, and growth. Quarterly Journal of Economics, 132(2), pp. 665-712.** The paper is available at https://academic.oup.com/qje/article/132/2/665/3076284.
 

## Data

The version released on August 9, 2020 is the latest data that updates and adds data for the second half of 2019.

We provide two data sets constructed from the paper here:

- **KPSS_2019_public.csv**: Patent level panel data from 1926 to 2019
- **patent_permco_permno_match_public.csv**: Patent-CRSP permco and permno match data 


For the patent level panel data, the variable definitions are:

| Variable name  | Definition                                         | 
| :---------------|:------------------------------------------------- | 
| patent_num     | Patent number                                      |
| permno         | CRSP permno                                        |  
| issue_date     | Issue date of patent (mm/dd/yyyy)                  |    
| xi_nominal    | Value of innovation(&xi;) in millions of nominal dollars |
| xi_real  | Value of innovation(&xi;) deflated to 1982 (million) dollars using the CPI|
| cites | Forward citations |

For the patent-permco-permno match data, the variable definitions are:

| Variable name  | Definition                                         | 
| :--------------|:-------------------------------------------------- | 
| patent_num     | Patent number                                      |
| permco         | CRSP permco                                        | 
| permno         | CRSP permno                                        |  


## Notes:

1. The value of innovation(xi_real) is equal to the nominal value of innovation(xi_nominal) deflated to 1982 (million) dollars using the CPI. In other word, we can simply calculate the xi_real through the following equation: xi_real = xi_nominal / CPI * 100.

2. We drop patents in the dataset that were assigned to multiple CRSP permnos.

3. The updated KPSS values differ slightly from the data in the QJE paper for any of the following reasons:

	a)	Changes in the CRSP dataset over time.

	b)	Improvements in the matching process to firms.

	c)	Re-estimation of the parameters needed to compute the KPSS value: 

	- the parameter gamma is re-estimated in the full sample to 2019: the new estimate is 0.0139, while the estimate of gamma in QJE paper is 0.0146.

	- stock return volatility is now computed over the last 52 weeks (as opposed to the previous calendar year in the QJE paper)

4. The number of forward citations is updated to 2019.


## Contact:

Please contact Dimitris Papanikolaou (d-papanikolaou@kellogg.northwestern.edu) or Amit Seru (aseru@stanford.edu) for any questions regarding the data.

**Please see the paper for more information on the data. If you use these data sets, please CITE this paper as the data source.**
