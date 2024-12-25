java c
EMET8002 Case Studies in Applied Economic
Analysis and Econometrics
Semester 2 2024
Computer Lab in Week 4This   week we use   the   2015   Programme   for   International   Student   Assessment   (PISA)   dataset for   our   analysis.   PISA assesses skills of 15-year-old students across many   countries and involves data on   student performance   (reading, mathematics   and   science knowledge),   as well as parent, school and teacher questionnaires. The data is publicly available and can be downloaded   from   the   PISA   website   under   the   section   “SPSS   (TM)   Data   Files   (compressed)”   (https://www.oecd.org/pisa/data/2015database/).      PISA codebooks and questionnaires are available through the same link. However, these are large files and take sometime to download      and   convert   to   Stata   format.   Therefore,   we   have   prepared   a   smaller   merged   dataset   of the      Student   and   School   questionnaire   data   files   which   now   only   includes   the   relevant   variables.      You can download this data (“Week4_PISA_data.dta”) from Wattle.
Question   1: Categorical Dependent Variables
We are interested in what determines whether a student has   to   repeat   a   grade   at   school   at   least   once. We call our dependent variable “repeated” and   this   is   a   dummy variable   that   is   equal   to 1 if   a student has repeated a grade at least   once,   and   equal to   0   when   the   student has   never repeated a   grade.
(a)   Drop missing observations for the “repeated” variable (hint:   missing values   are
sometimes   coded   as   “.” or   “.a”;   you   may   consider   “keep” or   “drop”   commands).
(b)   There are several dummy variables that we will include as   independent variables.
These are usually coded as “1” or “0”, but in   the   PISA   dataset   these   are   given   as   “2”   or “1”   . For example, “male” is equal to   2   if   the   student   is   male   and   equal to   1   if   the student is female. Recode these dummy variables such that   they   are   equal   to   1   if   the variable description applies to the student, and 0   otherwise   (e.g.,   the   “male”   dummy   is equal to   1 if   the student is male, and   equal to   0   if   the   student   is   female).   Do   this   for   the ”male”, “international_lan”, “quiet study” and   “training” dummy variables.   (hint:   you   can   use   the   “replace” command)
(c)   Explain why we only need to include one dummy variable (e.g.,   “male”)   in   the   regression to describe a binary variable with two possible values (e.g., male or      female).
(d)   Run   alogit   model   with   “repeated” as   the   dependent   variable   and   the   following
independent variables: “international_lan”, “male”, “mother_edu”, “father_edu”,   “quiet_study”, “school_size”, “class_size”, “training”, “computer”   . How   do   you    interpret   the   estimated   coefficients?
(e)   Exclude missing values for all independent variables. Repeat the logit model   from
part d but estimate it without missing values. Are there any differences? Which   model   do you prefer?
(f)    Repeat your preferred logit model from part e but estimate it代 写EMET8002 Analysis and Econometrics Semester 2 2024
代做程序编程语言 using clustered   standard   errors (by school). When do we use clustered   standard errors   and why?
(g)   What are the effects of   mother’s education (“mother_edu”) on   whether   a   student has
to repeat a grade? Include   joint tests in your answer.   (hint:   this variable   is   based on   the survey question:   "What is the    completed by   your   mother?"   Possible answers: ISCED level 3A (coded as   1); ISCED level 3B, 3C (coded   as 2); ISCED level 2   (coded as 3); ISCED level   1   (coded as 4); She did not complete            ISCED   level   1   (coded   as   5). For   definitions   of   ISCED   education   levels   see,for   example, https://stats.oecd.org/glossary/detail.asp?ID=1436)
(h)   Calculate and interpret odds ratios for the logit regression   in part   d.
(i)    Calculate and interpret   marginal effects   for   father’s   education   (“father_edu”)   based   on   your logit regression part d.
(j)    Run both logit and probit models using the   same variables   as   in part   d   and   export your   results to an excel file. How do   your results   differ   across the two   models?   (hint:   commonly   used   commands   to   export   data   from   Stata   are   the   “outreg2” and   “estout”   commands)
(k)   Compare   the   predicted   probability   values   for   father’s   education   (“father_edu”) for
both logit and probit models from part   j and   export   them   to   an   excel   file.   How   do   your   results differ across the two models?
Question 2: Preparation for Research Proposal   [not required   for problem   set]The Research Proposal is due on   1   September 2023. First of   all, you   are   expected to provide   a   summary of   the main findings, data and methods of   the paper that you have   chosen   for your research project as well as a brief   literature review. Next, you need to propose a minor   extension to the original paper. Your idea for the extension needs to be backed up with prior   literature and/or theory. You need to explain why your research question is interesting,   what   you expect to find, and how you are   able to   test   it   (with   specific   statistical hypotheses,   data and methods). There is no need to do any   analysis   at   this   stage.
(a)   Identify a couple of   references from the academic   literature   that   are relevant   to your   project. How are they similar or different   from your paper?   (methods,   data,   sample         period, country). Are their findings consistent or contradictory to your paper?
(b)   Discuss what involves developing an effective research   question. You may refer to   section 3.1.2 of   the following   document:
https://www.economicsnetwork.ac.uk/handbook/ugresearch/31
(c)   Come up with a few ideas for your extension. Why   do you   think that   they   are      interesting? Based on theory and prior literature, what do you   expect to   find?      Formulate your idea in the form. of   a research question and   a   formal   statistical   hypothesis. Make sure that your extension is feasible given the   data   and   time      constraints that you have.







         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
