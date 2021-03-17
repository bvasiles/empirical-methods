## Blog Post: Paper Motivation Critique  *by Nadia Nahar*

> Zhang, A. X., Muller, M., Wang, D. (2020). [How do Data Science Workers Collaborate? Roles,
Workflows, and Tools](https://doi.org/10.1145/3392826). In Proceedings of the ACM on Human-Computer Interaction. 4, CSCW1, Article 22 (May 2020), (pp. 1-23). 

The paper aimed to understand the collaborative practices of data science teams from both the perspectives of technical (e.g., data scientist, engineers) and non-technical (e.g., managers, domain experts) team members. They designed an online survey targeting a large scale of users with 183 participants working in various roles (5 major roles). They reported the extent of interaction between these roles in different stages of the workflow and using different tools. They also identified the collaboration practices of the workers and discussed some design implications based on those to support the data science team collaboration.

### Description of problem

Interdisciplinary collaboration has always been considered as challenging which stands true for the modern machine learning projects as well. From the literature, it has been understood that data science collaboration is not the same as the traditional software development teams. As per the authors of the paper and other related papers, due to being engaged with more "exploration" process than "engineering" process, distinct skills and knowledges reside, and make the collaboration even more challenging.
The paper presents a rich literature overview in three bundles -
- HCI and CSCW research on data science work practices
- specific literature aiming to understand and support collaboration in data science
- proposed tools and features in data science 

#### Gap
The paper points out a gap in the current knowledge that, till now understanding of data science collaboration only focuses on the perspective of the data scientist, ignoring other potential forms of data science collaboration. As quoted from the paper -

> Unfortunately, most of today’s understanding of data science collaboration only focuses on the perspective of the data scientist, and how to build tools to support distant and asynchronous collaborations among data scientists, such as version control of code. The technical collaborations afforded by such tools [100] only scratch the surface of the many ways that collaborations may happen within a data science team, such as when stakeholders discuss the framing of an initial problem before any code is written or data collected [79]. However, we have little empirical data to characterize the many potential forms of data science collaboration.

Also, the existing works focusing on data science practices mostly adopt interview research methods and a few use ethnographic research methods, falling short to generalize understanding from a larger user population. As quoted from the paper -
> Many of the papers about solitary data science work practices adopted the interview research method [34, 50, 54, 67, 92, 95]. An interview research method is well-suited for the exploratory nature of these empirical works in understanding a new practice, but it also falls short in generating a representative and generalizable understanding from a larger user population.
> These related projects focused only on a civic data hackathon [43] and on the collaborative projects between data scientists and bio-medical scientists in scientific discovery projects [61]. Also, both of them used ethnographic research methods aiming for in-depth understanding of the context. In this work, we wanted to target a more commonly available scenario—data science teams' work practices in corporations—as this scenario is where most data science professionals work. We also want to gather a broader user perspective through the deployment of an online survey.

The paper also argues that the collaboration researches and tool supports till now have been focusing on the technical aspects only, ignoring the non-technical roles causing multidisciplinary problems (e.g., deep domain knowledge often only resides in domain experts mind). As quoted from the paper -

> In sum, almost all of the proposed tools and features in data science focus only on the technical users’ scenarios (e.g., data scientists and data engineers), such as how to better understand and wrangle data [18, 41], or how to better write and share code [49, 81, 92, 93].

#### Hook
The hook of the paper is to propose better design suggestions from a multi-disciplinary perspective. As quoted from the paper -
> In this work, we want to present an account that covers both the technical roles and the non-technical roles of a professional data science team in corporations, so that we can better propose design suggestions from a multi-disciplinary perspective.

To elaborate, currently only the technical users’ (e.g., data scientists) perspectives are taken into account while designing a tool. This leads to inconvenience for the non-technical users to interpret the coding solutions and results. Thus, for designing better tools, perspectives of the multi-disciplinary people like domain experts, managers, etc. are needed. Thus, the target of this paper is to better understand the collaborative practices from not only the technical users but also the non-technical ones. The authors believe that by understanding the collaborative problems from all these users, better design decisions can be taken for designing future collaboration tools.

Thus, the authors of this paper wanted to gather a broader user perspective through a large-scale online survey to complement the existing qualitative narratives, so that they can cover both technical and non-technical perspectives, and provide better tool design suggestions.

The authors provided some tool suggestions later on in the discussion section as Possible Collaborative Features (Section 5.1). For example, they suggested "Transparency" to be provided as a feature so that the data scientists do not inadvertently take hidden decisions that causes difficulty for the other team members in transmission of knowledge. Such assumptions and undocumented decisions can cause problems in establishing management plans. Thus, while designing a collaborative tool, transparency feature is needed to advocate making invisible activities more visible.

### Research questions
The research question that the paper aims to answer is -
> What is the extent of collaboration on data science teams?

## Overview of study design / methods 

The paper designed an online survey as the study method. The targeted participants are the employees of IBM, working in diverse roles. The participants are approached through slack channel having approximately 1000 employees, and 183 self-selected participants provided data. The survey questions were kept optional to encourage people to contribute. It consisted of questions about project, collaboration with team and roles in different phases, open-ended questions about tools used to collaborate in different workflow stages, and collaboration practices. The open-text responses were coded using a coding guideline set in advance.

### Critique

The authors philosophical stance seems to be somewhere in between Positivist and Constructivist. Although both the world views are opposites, the work seems to have some essences from both the views. The authors do not start with a theory, and test a hypothesis, which manifests them to not be in the Positivist stance. Again, they treated theory as a product of research similar to inductive researchers, that indicates their Constructivist stance. However, the confusion arises when the survey questions seem to be precise about the answers they are looking for (some are open-ended like used tools in different workflow stages, but again the possible answers don't seem to have a very broad domain), and the adoption of the quantitative approach. Thus, it seems that, there ought to be some theory, which is implicit in the whole paper. However, because of the unmentioned theory at the beginning, the authors can be concluded to be in the Constructivist stance, with some skepticism.

To be explicit about some more criticisms, the research question was very broad, and the authors attempted to relate that to tools, stages, practices, etc. However, the connections were not explicitly stated, again along with a theory. Additionally, the research suffers from the bias of self-reported data. Also, they stated the purpose why they used quantitative approach was to do a large-scale study that can be 
