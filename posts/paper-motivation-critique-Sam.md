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

## Authors' Philosophical Stance

From the study design it appears to me that the authors lean towards the Constructivist/Interpretivist worldview. As the authors point out in literature review, most of the guidelines for visualization design in this area are simply conventions without too much empirical evidence. The authors acknowledge the intricacies in visualization design for a variety of context and audiences, yet seek to construct some truth on the particular question of truncating the y-axis in different charts via empirical studies. The experiments are rigorously designed based on existing literature and methods, yet remain very qualitative in nature due to individual's subjective views.

The constructivist nature of the study is apparent in the design of the series of three experiments, where the subsequent experiment always builds on the findings of the previous one. Experiment One shows no significant difference in the impact of truncation on bar charts versus line charts, suggesting that "designers may have to employ other methods to indicate that a y-axis has been truncated" rather than simply using a different chart type. This prompted the authors to design Experiment Two to measure exactly the effectiveness of the "other methods". This experiment shows that calling attention to the truncated axis does not noticeably impact the subject's perception; however, there lies the alternative explanation that the subjects could have simply misread the information on the axis. This prompted them to design Experiment Three to investigate and ultimately dismiss this explanation. Throughout the process, the authors designed experiments to establish their theory on the matter in an inductive, exploratory way.

## Structure of the Literature Review

The authors clearly establish the problem of y-axis truncation in the paper introduction. Then, they discuss existing guidelines about y-axis truncation in various sources, including Huff's "How to Lie with Statistics", Brinton's "Standards for Time Series Charts", Alberto Cairo's "How Charts Lie", and more. The authors present a narrative of different viewpoints from these sources. Although there is no sub-sections grouping common stance for different sources, the entire narrative is logically clear.

First, the authors present discussions on y-axis truncation on bar charts in particular. This is the most well established part of the problem. Then, they present discussions about other chart types including line charts, as well as methods of indicating the truncation. Here, some voices differ. Finally, the authors point out that although there do not lack discussions on the topic, most are opinionated but without rigorous evidence. Thus, the major gap in the area is the lack of empirical basis supporting any of the competing beliefs.

On the other hand, the authors do not clearly indicate the "hook" of their study - why their study makes a significant contribution to the gap of the problem. Nevertheless, they implicate in various parts of the discussion on experimental results that chart designers should keep in mind the effect of truncating the y-axis on chart types other than bar charts and even when the truncation is indicated explicitly, in order to avoid deception as much as possible.
