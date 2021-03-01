** Description of problem **

   Sustainability of GitHub project is an important and unsolved problem for open source software community. 
   Usually projects rely on a large community of users voluntter to contribute and lack of contribution causes major loss in the real world like "the HeartBleed instance". 
   Because of the voluntary nature of open source contribution, volunteer dilemma and common poor theory states users may not actively
contribute becuase they think "others will do". Reported online content creation field, the shared responsibility may lead to a "90-9-1 principle" , 
which states 90% of users never contribute back, 9% of users make minor contribution and the rest 1% users make the majority.
Quantifying the extent of which this principle applies in open source world and 
what is the extent of contribution equality in oss is important for the understanding of open source development activity and studying the sustainability of open source projects.

** Main research questions **
   The question are three-folded:
   
      a) Do open source software developers exhibit participation inequality in their contributions
      b) Do open source software projects suffer from partici-pation inequality?
      c) Does the popularity of an open source software project affect participation inequality?

** Overview of study design / methods **
   Users can perform differen actions (or operations) on GitHub. Authors manually code those actions into three categories: 
   
      a) WATCH(only passive event)
      b) INTERACT(weakly active event)
      c) CONTRIBUTE(active event). 
   
   Authors collect user action record and project level information from GHArchive data, and create three datasets:
   
      a) Random user set, where they randomly sample users from the complete data and collect their asscoiated projects.
      b) Random project set, where they randomly sample projects from the complete data.
      c) Popular project set, where they select the 500 most popular projects from the complete data.
      
   They caclualte the distribution of each action category in the three dataset.
   
   
** Critique **
    * What's the authors' likely philosophical stance? *
         I would think they are "Positivist", as they start from common-pool resource and voluntter-contribution theory and expect this theory can "predict" what's happening in oss.
    * How well structured is the literature review? Is there a clear gap / hook? What are they? *
         The literature reviews starts from the lituracy of contribution inequality in other fields like Twitter and Wikipedia, where a 90-9-1 principle is reported.
         And it describes how researchers in oss community study contribution inequality: two major directions are introduced, one focus on the inequality of non-coding activity like 
         user activity on project mailing-list, the other focuses on inequality of coding contribution.
         According to the author, this paper introduces "90-9-1" principle into oss field and measure the inequality based on the type of action, not the amount of contribution.
         I think this paper doesn't do a good job of explaining why it's needed to measure inequality based on actions, and what benefit does bring "90-9-1" principle into oss better
         than the concept previously studies in oss (e.g. core team VS non core team). Adding descriptions about what are the problems unsolved/unanswered with inequality measured by 
         contribution size, and what might be the value of introducing inequality metrics with action type benefit the research community.
    * What are the strengths and weaknesses of the study design and research methods, as best you can tell? *
   Strength: 
          
            + Writing is clear and easy to read.
            + Provide detailed coding protocal on how to code actions into types, and the reasoning behind the coding.
            + The method is simple to operate and replicate


   Weakness:
          
            - The method is not complicated enough to provide a deep insight.


   * Do the authors use theory? How? *
       Yes, the authors referred to the theory of common pool resource and voluntter contribution. They use the theory to infer how might inequality of contribution be like in oss, 
       which helps them to construct research questions and hypothesis in the study.










