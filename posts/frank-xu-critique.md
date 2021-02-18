## Frank Xu's Blog Post: Paper Motivation Critique

> Dey, T., Mousavi, S., Ponce, E., Fry, T., Vasilescu, B., Filippova, A., and Mockus, A. (2020). [Detecting and Characterizing Bots that Commit Code](https://doi.org/10.1145/3379597.3387478). In Proceedings of the International Conference on Mining Software Repositories, MSR, ACM (2020). 

The paper tackles the problem of identifying automation tools that commits code from human manual activities. The authors propose BIMAN, a systematic approach to detect bots using author names, commit messages, files modified by the commit, and projects associated with the commits.
The paper also aim to characterize the types of bots based on their activity patterns.
As an additional bonus, the paper produces a shareable dataset containing detailed information about 461 bots they found and 13,762,430 commits they created to fuel future research on this topic.


### Description of problem
Traditionally, many activities such as making code commits, opening, managing, or closing
issues are all done by the human developers manually.
However, the recent trend is that more and more such operations are done by automation tools, especially in open source projects.
In many software mining scenarios related to developer productivity or code quality, it is desirable to identify bots in order to separate their actions from actions of individuals.
To solve this problem, the authors aim to develop an automatic tool to identify bots from commits.


### Research questions
- RQ1: How can we determine if a particular author is a bot?
- RQ2: What type of work do bots perform and which programming languages do they work with?


## Overview of study design / methods 

The paper uses the data from the World of Code dataset, containing information on 73,314,320 unique non-forked Git repositories, 34,424,362 unique author IDs, and 1,685,985,529 commits.
The authors manually identified and labeled some gold classifications of bots vs. non-bots for training and validation purposes.

To answer RQ1, the authors then propose an ensemble of regular expression matching on name and email, random forest classification model on files and projects, as well as document template model on commit messages to predict whether the author is a bot.
Qualitatively, the author validates how the tool is performing in detecting a few known bots.
Quantitively, the performance of the tool is evaluated using AUC-ROC score on gold validation dataset.

To answer RQ2, the authors characterize the bots based on their activity during the day by analyzing the activity time; and what types of files do bots modify, both using the golden dataset of bots.



### Critique

The authors seem to have a philosophical stance of a positivism, where "knowledge is exclusively derived from experience of natural phenomena and their properties and relations" (Wikipedia). 
The literature review is well-structured demonstrating a clear gap and hook.
Some of the closest related work are presented in the introduction, along with the motivation why identifying bots is an important problem and what existing work has done along this way.
More loosely related work are presented in the dedicated related work section, discussing bots in general, bots characteristics, and OSS communities.

The study design and methods presented have advantages and disadvantages.
On the one hand, the tool creation and the automatic model training and evaluation are convincing, as the use the manually labeled gold data for validation, as well as widely used AOC-RUC metrics.
On the other hand, the authors also present a qualitative study on a predefined set of well-known bots.
It seems to me that this part may have the bias towards better performance as the widely used bots are also very dominant in the data samples.
It would be great if we could also see more detailed qualitative analysis on a random sample of bots, that ideally covers both well-known bots and in-house lesser-seen bots.

For analyzing the bot characteristics, the card sorting methods used for categorizing bots based on activity patterns are following good practices.
However, when analyzing what type of files (languages) the bot is most frequently touching, I think the analysis does not show the difference in terms of the file frequency in different projects, i.e. a popular language may be more prevalent than a less-popular one, and thus the bot activity is higher due to more files written in that language.

Also, throughout the paper, there might be some implicit theories around, but it would be great if the authors could present some explicit theory supporting the research questions and hypothesis.
