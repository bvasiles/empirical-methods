## L21: Diff-in-Diff & CausalImpact ([slides](../slides/21-diff-in-diff.pdf), [video](https://youtu.be/IZXPdvceOZQ))

[![Lecture21-Diff-in-Diff](../assets/images/21-diff-in-diff.jpg)](../slides/21-diff-in-diff.pdf)

In this last lecture in the regression / quantitative analysis series, we talk about two popular causal inference techniques for evaluating the effects of an intervention. 

[Difference-in-differences](https://en.wikipedia.org/wiki/Difference_in_differences) (or diff-in-diff) is a classic statistical technique used in econometrics and quantitative research in the social sciences that attempts to mimic an experimental research design using observational study data, by studying the differential effect of a treatment on a 'treatment group' versus a 'control group' in a natural experiment. It calculates the effect of a treatment (i.e., an explanatory variable or an independent variable) on an outcome (i.e., a response variable or dependent variable) by comparing the average change over time in the outcome variable for the treatment group, compared to the average change over time for the control group.

[CausalImpact](https://google.github.io/CausalImpact/CausalImpact.html) is a modern approach to estimating the causal effect of a designed intervention on a time series. Given a response time series (e.g., clicks) and a set of control time series (e.g., clicks in non-affected markets or clicks on other sites), the CausalImpact R package constructs a Bayesian structural time-series model. This model is then used to try and predict the counterfactual, i.e., how the response metric would have evolved after the intervention if the intervention had never occurred. For a quick overview, watch the [tutorial video](https://www.youtube.com/watch?v=GTgZfCltMm8). For details, see: [Brodersen et al., Annals of Applied Statistics (2015)](http://research.google.com/pubs/pub41854.html).

*Note*: Bogdan was out with COVID. This is a rerun of the Spring 2021 lecture instead of a live lecture.

### Example Papers

> Yang, L., Jaffe, S., Holtz, D., Suri, S., Sinha, S., Weston, J., ... & Teevan, J. (2020). [How Work From Home Affects Collaboration: A Large-Scale Study of Information Workers in a Natural Experiment During COVID-19](https://arxiv.org/pdf/2007.15584.pdf). arXiv preprint arXiv:2007.15584.

### Lecture Readings

> Diff-in-diff lecture from the [Foundations of Program Evaluation III course](https://ds4ps.org/pe4ps-textbook/docs/p-030-diff-in-diff.html)

The source for the diff-in-diff example I used in class.

---

> Rajendran, P. [Causal Inference using Difference in Differences, Causal Impact, and Synthetic Control](https://towardsdatascience.com/causal-inference-using-difference-in-differences-causal-impact-and-synthetic-control-f8639c408268). 

Another useful tutorial on diff-in-diff.

---

> Wing, C., Simon, K., & Bello-Gomez, R. A. (2018). [Designing difference in difference studies: best practices for public health policy research](https://www.annualreviews.org/doi/full/10.1146/annurev-publhealth-040617-013507). Annual review of public health, 39.

The paper explains the key assumptions of the diff-in-diff design and discusses analytic tactics, supplementary analysis, and approaches to statistical inference that are often important in applied research. 

### Additional Readings

Two good textbooks on causal inference, including the techniques above.

> Gertler, P. J., Martinez, S., Premand, P., Rawlings, L. B., & Vermeersch, C. M. (2016). [Impact
evaluation in practice](https://repositorio.minedu.gob.pe/bitstream/handle/20.500.12799/4813/Impact%20Evaluation%20in%20Practice.pdf). The World Bank.


> Pearl, J., Glymour, M., & Jewell, N. P. (2016). [Causal inference in statistics: A primer](http://bayes.cs.ucla.edu/PRIMER/). John Wiley & Sons.