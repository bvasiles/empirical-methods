## L17: Simpson's Paradox ([Rmd](../slides/17-mixed-effects.html), [video](https://youtu.be/PvHd_GqH6Tw))

![Lecture17-Simpsons-Paradox](../assets/images/17-random-effects.jpg)

In this lecture in the regression series we talked about within-between mixed-effects model and how it can deal with an example illustrating [Simpson's paradox](https://en.wikipedia.org/wiki/Simpson's_paradox). 

See this [R markdown file](../slides/17-mixed-effects.html) for details, plus the video.

We also discussed two example papers that used mixed-effects models as part of their analyses.

### Exemplars

> Peoples, B. K., Midway, S. R., Sackett, D., Lynch, A., & Cooney, P. B. (2016). [Twitter predicts citation rates of ecological research](https://journals.plos.org/plosone/article/file?id=10.1371/journal.pone.0166570&type=printable). PloS One, 11(11), e0166570.

---

> Vasilescu, B., Posnett, D., Ray, B., van den Brand, M. G., Serebrenik, A., Devanbu, P., & Filkov, V. (2015). [Gender and tenure diversity in GitHub teams](https://cmustrudel.github.io/papers/chi15.pdf). CHI Conference on Human Factors in Computing Systems, CHI, ACM, pp 3789–3798. See also [this erratum](https://dl.acm.org/action/downloadSupplement?doi=10.1145%2F2702123.2702549&file=chi2015erratum.pdf).

### Lecture Readings


> Bates, D., Mächler, M., Bolker, B., & Walker, S. (2015). [Fitting Linear Mixed-Effects Models Using lme4](http://mirrors.nics.utk.edu/cran/web/packages/lme4/vignettes/lmer.pdf). Journal of Statistical Software, 67(1), 1 - 48. 

Official vignette for the `lme4` package in R, that describes the syntax and how to specify and interpret mixed-effects linear regression models.

---

> Bell, A., & Jones, K. (2015). [Explaining fixed effects: Random effects modeling of time-series cross-sectional and panel data](). Political Science Research and Methods, 3(1), 133-153.

> Bell, A., Fairbrother, M., & Jones, K. (2019). [Fixed and random effects models: making an informed choice](https://core.ac.uk/download/pdf/161126779.pdf). Quality & Quantity, 53(2), 1051-1074.

Both papers assess the options available to researchers analyzing multilevel (including longitudinal) data, with the aim of supporting good methodological decision-making. Capabilities and limitations of fixed and random effects (FE and RE) models are presented, together with the within-between RE model -- the most general of the three, with all the strengths of the other two. 

The earlier paper argues that "there are few, if any, occasions in which FE modeling is preferable to RE modeling" and that "a well-specified RE model can be used to achieve everything that FE models achieve, and much more besides." Fun read.

---

> McNeish, D., & Kelley, K. (2019). [Fixed effects models versus mixed effects models for clustered data: Reviewing the approaches, disentangling the differences, and making recommendations](https://www3.nd.edu/~kkelley/publications/articles/McNeish_Kelley_PsychMethods_2019.pdf). Psychological Methods, 24(1), 20.

This article discusses the differences between mixed effects and fixed effects models for clustered data, reviews each approach, and helps to identify when each approach is optimal. It then discusses the within–between specification, which blends advantageous properties of each framework into a single model.

There is overlap in content with the Bell et al papers above.

---

> Hair Jr, J. F., & Fávero, L. P. (2019). [Multilevel modeling for longitudinal data: concepts and applications](https://core.ac.uk/download/pdf/288188778.pdf). RAUSP Management Journal.

Another paper that discusses multilevel modeling for longitudinal data, clarifying the circumstances in which they can be used.

---

> Hox, J. J., Moerbeek, M., & Van de Schoot, R. (2017). [Chapter 2](http://joophox.net/mlbook2/Chapter2.pdf) from Multilevel analysis: Techniques and applications. Routledge.

The multilevel regression model is commonly needed and used. Such models assume that there is a hierarchical data set, with one single outcome or response variable that is measured at the lowest level, and explanatory variables at all existing levels. Conceptually, it is useful to view the multilevel regression model as a hierarchical system of regression equations. This chapter explains the multilevel regression model for two-level data.


### Additional Readings


> Bell, A., Jones, K., & Fairbrother, M. (2018). [Understanding and misunderstanding group mean centering: a commentary on Kelley et al.’s dangerous practice](https://d-nb.info/1149996188/34). Quality & Quantity, 52(5), 2031-2036.

"Group-mean-centering is, in short, no more dangerous than any other statistical procedure, and should remain a normal part of multilevel data analyses where it can be judiciously employed to good effect."

---

> Townsend, Z., Buckley, J., Harada, M., & Scott, M. A. (2013). [The choice between fixed and random effects](http://agfda.userweb.mwn.de/ALD_2016/downloads/Uebung2/Townsend_et_al_2013.pdf). The SAGE handbook of multilevel modeling, 73-88.

---

> Clark, T. S., & Linzer, D. A. (2015). [Should I use fixed or random effects](https://datajobs.com/data-science-repo/Fixed-Effects-Models-[Clark-and-Linzer].pdf). Political Science Research and Methods, 3(2), 399-408.
