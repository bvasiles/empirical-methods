## L17: Segmented Regression of Interrupted Time Series Data ([pdf](../slides/17-time-series.pdf), [video](https://youtu.be/wuDfI71oPVs))

[![Lecture17-Interrupted-Time-Series](../assets/images/17-time-series.jpeg)](../slides/17-time-series.pdf)

Interrupted time series is a valuable study design for evaluating the effectiveness of interventions. A segmented regression approach can be used to analyze an interrupted time series study by testing the effect of an intervention on the outcome of interest using an appropriately defined impact model. A typical scenario involves testing the degree to which a treatment shifts the underlying trajectory of an outcome.

In this lecture we go over the seasonality-trend decomposition of time series and discuss methodological considerations specific to interrupted time series analysis. (But first we have a few leftovers from the previous lecture, including the Lim Wikipedia paper.)


### Lecture Readings


> Shadish, William R., Thomas D. Cook, and Donald Thomas Campbell. Experimental and quasi-experimental designs for generalized causal inference. Boston: Houghton Mifflin, 2002.

- Chapter 6: Interrupted time series
- Chapter 7: Regression discontinuity design

*THE* textbook on the matter.

---

> Morgan, S. L., & Winship, C. (2015). [Counterfactuals and causal inference](https://content.schweitzer-online.de/static/catalog_manager/live/media_files/representation/zd_std_orig__zd_schw_orig/023/777/881/9781107065079_foreword_pdf_1.pdf). Cambridge University Press.

- Chapter 11: Repeated Observations and the Estimation of Causal Effects 

The fundamental challenge of causal inference is that an individual cannot be simultaneously observed in both the treatment and control states. In some situations, however, it is possible to observe the same individual or unit of observation in the treatment and control states at different points in time. If the potential outcomes do not evolve in time for reasons other than the treatment, then the causal effect of a treatment can be estimated as the difference between an individual’s observed outcome in the control state at time 1 and the same individual’s observed outcome in the treatment state at time 2. The assumption that potential outcomes are stable in time (and thus age for individuals) is often heroic. If, however, potential outcomes evolve in a predictable way, then it may be possible to use the longitudinal structure of the data to predict the counterfactual outcomes of each individual.

The chapter discusses the interrupted time series (ITS) design and the closely related regression discontinuity design (RDD). 

---

> Bernal, J. L., Cummins, S., & Gasparrini, A. (2017). [Interrupted time series regression for the evaluation of public health interventions: a tutorial](https://core.ac.uk/download/pdf/42636401.pdf). International Journal of Epidemiology, 46(1), 348-355.

Interrupted time series is a valuable study design for evaluating the effectiveness of population-level health interventions. A segmented regression approach can be used to analyze an interrupted time series study by testing the effect of an intervention on the outcome of interest using an appropriately defined impact model. Methodological considerations specific to interrupted time series analysis include possible time-varying confounders such as seasonal trends or concurrent events to the intervention, and potential autocorrelation of data.

---

> Bhaskaran, K., Gasparrini, A., Hajat, S., Smeeth, L., & Armstrong, B. (2013). [Time series regression studies in environmental epidemiology](https://www.scienceopen.com/document_file/bf451389-6999-436d-a611-8899c4aa8730/PubMedCentral/bf451389-6999-436d-a611-8899c4aa8730.pdf). International Journal of Epidemiology, 42(4), 1187-1195.

The paper describes the general features of time series data, and outlines the analysis process, beginning with descriptive analysis, then focusing on issues in time series regression that differ from other regression methods: modelling short-term fluctuations in the presence of seasonal and long-term patterns, dealing with time varying confounding factors and modelling delayed ('lagged') associations between exposure and outcome. The paper ends with advice on model checking and sensitivity analysis, and some common extensions to the basic model.

---

> Humphreys, D. K., Gasparrini, A., & Wiebe, D. J. (2017). [Evaluating the impact of Florida’s "stand your ground" self-defense law on homicide and suicide by firearm: an interrupted time series study](https://researchonline.lshtm.ac.uk/id/eprint/3429596/1/Humphreysetal2016_JAMAInternMed.pdf). JAMA Internal Medicine, 177(1), 44-50.

Since Florida’s stand your ground law took effect in October 2005, rates of homicide (+24.4% through 2014) and homicide by firearm (+31.6%) in the state have significantly increased. 
These increases appear to have occurred despite a general decline in homicide in the United States since the early 1990s.
In contrast, rates of homicide and homicide by firearm did not increase in states without a stand your ground law (New York, New Jersey, Ohio, and Virginia), or for either suicide or suicide by firearm. 
Findings support the hypothesis that increases in the homicide and homicide by firearm rates in Florida are related to the stand your ground law. 



### Example Papers

> Wagner, A. K., Soumerai, S. B., Zhang, F., & Ross‐Degnan, D. (2002). [Segmented regression analysis of interrupted time series studies in medication use research](https://www.alnap.org/system/files/content/resource/files/main/segmented-regression-wagner-2002.pdf). Journal of Clinical Pharmacy and Therapeutics, 27(4), 299-309.

Beginning in September 1981, New Hampshire’s Medicaid program restricted the number of prescriptions reimbursed to a maximum of three per patient per month to decrease state medication expenditures. Implementation of the three-drug payment limit, or cap, interrupts the time series and creates the two segments of interest. An abrupt level change in the mean number of prescriptions, from about five per patient to fewer than three per patient, followed the cap. There was very little month-to-month change (or trend) in the number of prescriptions before as well as after the cap.

---

> Trockman, A., Zhou, S., Kästner, C., & Vasilescu, B. (2018). [Adding sparkle to social coding: an empirical study of repository badges in the npm ecosystem](https://cmustrudel.github.io/papers/icse18badges.pdf). In Proceedings of the 40th International Conference on Software Engineering (pp. 511-522).

Time-series analysis  revealed that the introduction of quality-assurance badges tends to correlate with positive intervention effects: The underlying qualities they signal tend to improve immediately, especially improved dependency freshness and more tests in pull requests.

### Additional Readings

> Metcalfe, A. V., & Cowpertwait, P. S. (2009). [Introductory time series with R](https://link.springer.com/book/10.1007%2F978-0-387-88698-5). Springer-Verlag New York.

