# Paper Motivation Critique

Mengchen (Sam) Yong

18 February 2021

---

Here I summarize the main ideas in "Truncating the Y-Axis: Threat or Menace?" by Michael Correll, Enrico Bertini, and Steven Franconeri. The paper is in the proceedings of the ACM Conference on Human Factors in Computing Systems (CHI) 2020.

> Michael Correll, Enrico Bertini, and Steven Franconeri. 2020. Truncating the Y-Axis: Threat or Menace? In Proceedings of the 2020 CHI Conference on Human Factors in Computing Systems (CHI '20). Association for Computing Machinery, New York, NY, USA, 1-12. DOI:https://doi.org/10.1145/3313831.3376222

## Summary

In conventional data visualization guidelines, the practice of starting the y-axis from non-zero values, i.e. "truncating the y-axis", has often been deemed "deceptive". Truncating the y-axis is believed to exaggerate effects and influence how people interpret the significance of effects, correlation, and trends. This is especially true for bar charts, where values are represented with areas, and the difference between two values would not be proportional to the difference in bar heights if the y-axis does not start at zero.

However, as the authors point out in the paper, "there is relatively little empirical work" on how truncating the y-axis affect the viewers' interpretation of the data and effects for a range of different visualization methods. Specifically, conventional guidelines often claim that line charts are not as much subject to the vulnerability of deception, and that explicitly indicating the y-axis truncation helps mitigate the deception; however, there is little empirical work examining these beliefs.

Therefore, the authors present their research questions in the paper as,

> Do the differences in visual design and framing (trend vs. value) behind line and bar charts result in different subjective effect sizes when the y-axis is altered? That is, is the impact of y-axis truncation different between bar charts and line charts?

> Does explicitly indicating that y-axis truncation has taken place reduce the bias introduced by truncation? That is, can visual designs alleviate the exaggeration caused by truncation?

The authors conducted a series of three crowd-sourced experiments via the platform `prolific.ac`, a service similar to Amazon Mechanical Turk but solely focused on studies. "The core of [their] experimental design is based on assessing qualitative changes brought by truncation." The authors used a 5-point rating scale to measure how subjects interpret the effect size of value differences and data trends in various visualization designs.

Experiment One focuses on comparing the impact of truncating the y-axis on bar charts versus line charts. Since the measurements are subjective, the study was conducted within-subject. Each subject was shown each of 48 different combinations of factors including chart type (bar chart or line graph), question framing (value-based on trend-based), truncation level, slope, and data size.

Experiment Two focuses on answering the second research question - whether indications of y-axis truncation alleviate the impact of truncation on viewers' interpretation. Each subject was shown each of 36 different combinations of factors, including a modified chart type selection among regular bar chart, broken axis bar chart, and gradient bar chart. The latter two are both common methods of mitigation, as the authors have discovered in literature.

Experiment Three used the same design as Experiment Two, but sought to answer the question - whether the impact of truncating the y-axis on viewers' interpretations is partly due to the viewer misreading data values on the charts.

For each of the above experiments, the subject was also shown 8 initial stimuli of different combinations slope and truncation level in order to calibrate the subject's individual perception of effect size, as grounding for their ratings in the experiments. After the experiment, the subject was given a graphical literacy test.
