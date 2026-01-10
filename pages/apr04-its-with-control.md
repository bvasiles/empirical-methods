## L21: Hands-on: Interrupted Time Series Analysis With Control ([notebook](../assets/activities/its_control.pdf), [video](https://youtu.be/Kxmc5tNOIxQ))

[![Lecture21-Interrupted-Time-Series-With-Control](../assets/images/21-diff-in-diff-synth-control.jpeg)](https://www.degruyterbrill.com/document/doi/10.1515/em-2018-0010/html)

In this lecture we discussed an exciting Nobel prize idea -- [natural experiments](https://www.nobelprize.org/uploads/2021/10/popular-economicsciencesprize2021-3.pdf).

We spent most of the lecture on a [hands-on activity](../assets/activities/its_control.pdf), showing students how to model jointly two interrupted time series, one for treated and one for controls, effectively recreating a difference-in-differences design. I used an [artificial dataset](../assets/activities/its_with_control.csv) for this. You can find an example solution in the [ITS notebook from last time](../assets/activities/its.pdf).

In the second part of the lecture we went over the [synthetic control method](https://medium.com/data-science/causal-inference-using-synthetic-control-4377b457c6bb), in particular the California Prop 99 case study. See the Abadie et al and Arkhangelsky et al papers. We went over this [notebook](../assets/activities/its_synthetic_class.pdf) illustrating the method.

Unfortunately I lost most of the video recording.

### Lecture Readings

> Bottomley, C., Scott, J. A. G., & Isham, V. (2019). [Analysing interrupted time series with a control](https://www.degruyterbrill.com/document/doi/10.1515/em-2018-0010/html). Epidemiologic Methods, 8(1), 20180010.

---

> Fichtenberg, C. M., & Glantz, S. A. (2000). [Association of the California Tobacco Control Program with declines in cigarette consumption and mortality from heart disease](https://www.nejm.org/doi/pdf/10.1056/NEJM200012143432406). New England Journal of Medicine, 343(24), 1772-1777.

---

> Arkhangelsky, D., Athey, S., Hirshberg, D. A., Imbens, G. W., & Wager, S. (2021). [Synthetic difference-in-differences](https://www.aeaweb.org/articles?id=10.1257/aer.20190159). American Economic Review, 111(12), 4088-4118.

---

> Abadie, A., Diamond, A., & Hainmueller, J. (2010). [Synthetic control methods for comparative case studies: Estimating the effect of California’s tobacco control program](https://doi.org/10.1198/jasa.2009.ap08746). Journal of the American statistical Association, 105(490), 493-505.