Jeremy Lacomis: Paper motivation critique
===

In this blog post I will be critiquing ["Docable: Evaluating the Executability
of Software Tutorials"](https://chrisparnin.me/pdf/docable_FSE_20.pdf) from
ESEC/FSE 2020 by Samim Mirhosseini and Chris Parnin. In this paper, the authors
study software tutorials, which give guidance to new users of a software
system. Specifically, they study tutorials that include code examples and the
"executability" of this code. Their main research questions are "Can tutorials
be naively executed? If not, Why?" and "Can tutorials be executed with limited
human annotation?".

They conducted a mixed-methods study to answer these questions. First, they
performed an analysis of tutorials that they collected and executed a random
sample of them naively (i.e., by copy-pasting the code in order) and with a
small set of annotations they developed directing how to use code blocks (e.g.,
an annotation of *run* means to run code, while an annotation of *user* means to
perform a command as a user). They found that with naive execution only 13% of
code blocks were executable, and only 26% of annotated blocks were
executable. They then recruited 6 "informants" who were "expert stakeholders in
technical documentation and performed a qualitative analyses of their results by
asking them open-ended questions about problems during execution and their
opinions of the severity of the problems they encountered.

The related work is partially presented in the introduction and partially
presented in a "Related Work" section near the end of the paper. The related
work section identifies previous work that studied if tutorials follow best
pedagogical practices, and the pain points of tutorial takers or tutorial
creators. The gap they identify is in studies of the _executability_ of
tutorials: at most existing work studied the executability of Jupyter notebooks
or code found on Stack Overflow.

The authors clearly use theory, citing properties of an ideal tutorial directly
from existing guidelines published by DigitalOcean. These guidelines point out
that tutorials should be as accessible as possible for all tutorial takers
(e.g., should not assume prior knowledge such as how to execute a given
command), should explicitly include every command a reader needs to know, and
should not merely be scripts, but should explain every step and impart
knowledge. The theory is that if code is not executable, it is less useful to a
tutorial user.

The strongest part of the paper is its summary of the most common problems found
during the qualitative study. For example, they found that many tutorials made
assumptions about the reader's computing environment that may not hold and that
others contained blocks without explicit indication of the expected action a
reader should take. They also enumerate weaknesses of their study in a
"Limitations" section, including that their domain was limited and that they did
not execute inline code blocks.
