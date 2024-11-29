java c
COSC2759 Assignment   1 Specifications 
Deadline                                                                                          Sunday 1 September 2024 (11:59 pm AEST)
% allocated to this   assignment                           35% (to be marked out of 35) 
To be   submitted   via                                                           Canvas 
To   be attempted                                                                   Individually or   in   pairs
Scenario 
Alpine   Inc   has   recently   built   a web   application that   allows   users to   record simple   Notes   application.   The   application   is   built   using   NodeJs,   Express   and   backed   by   a   NoSQL   MongoDB. 
The   source   code   for   this   application   is   stored   in   GitHub   but   the   code   itself   is   built   and deployed   manually   from   the   lead   developer’s   (Pete)   laptop. Although   this   process   has   worked in the past, Pete had recently taken leave from work which has meant that Alpine   Inc   missed a critical   release that contained a   new feature for   one   of their   largest   clients.
There have also been instances where bugs have been introduced into production which   has   caused   an   increase   in   the   number   of   support   calls   from   their   customers,   and   the   support   and   development   teams   have   had   to   work   overtime   to   manage   the   load   and   fix the issues. These issues are causing reduced morale among the teams, as well    as   impacting   the   revenue   of   Alpine   Inc.
As   the   newly   hired   DevOps   practitioner,   Alpine   Inc   has   turned   to   you   to   help   resolve   their   issues   and   enable   their   teams   to   better   deliver   new   features   and   ensure   releases   into production are   quick   and   reliable. 
To   help   kick   off   this   transformation, you   have   proposed   that   Alpine   Inc   start   looking   at establishing   a   CI   pipeline   to   help   reduce   dependency   on   Pete   by   introducing   automated   builds   and   automate   their   testing   processes. This   will   reduce   the   strain   on   the   QA   team and   ensure    bugs   and   development   defects   are picked up quickly and   fed    back   to   developers   to   be   resolved   before   any   changes   are   promoted   to   production. 
The   Approach 
To make this easier for Alpine Inc, which is rather immature with DevOps methodologies   and   practices,   you   have   opted   to   use   SaaS   tools   where   possible   to   help   reduce   the   learning   curve for their   development team. You   will   follow   best   practice   principles   and   make as much of your solution   using code, this   includes your   CI   build   configuration   and scaffolding   scripts. 
Tools to   use:
•            GitHub
•            GitHub   Actions   –   used   for   creating   the   pipelines
•             Basic   npm   commands
After a lengthy and heated debate amongst the team, it was decided to use GitHub Flow   as   the   branching   strategy.   Rather   than   committing   directly   to   the   “main”   branch,   it   was agreed   to   always   use   feature   branches   and   pull   requests.   However,   it   was   also   agreed   that engineers could approve their   own   PR’s. 
Deliverable 
Alpine   Inc   expects   you   to   update   your   GitHub   repository   with   the   code   and documentation   required to   run the Continuous   Integration build you are creating for   them   including all files. So far, the company   has   been sending   around   a zip   for their application   and   it’s   up   to   you   to   bring   them   into   the   modern   age. 
You task   is to:
1.      Define   a   CI   pipeline   by   creating   a   file   in   the   .github/workflows   directory. Your pipeline   will   automatically   execute   on   GitHub   Action   runners.
2.      Define   your   readme.md.
Note   that   when   you   implement   things   like   linting   and   end-to-end   testing, you   might   discover    bugs   or   errors   which   the   development   team   had   not   noticed   before! You   will   need   to   fix   them so that your pipeline   passes. (Hint: some of the   package versions   pinned   by the   dev   team   in   package.json   might   need   to   be   “bumped” to   operate   in   a   more   current   environment.)
Access   GitHub   Org 
1.       Log   in   to   GitHub, navigate   to ‘Your   organ代 写COSC2759 Assignment 1
代做程序编程语言izations’ and   accept   invite
2.       Create   new   repository, naming   should   be   student_id-assignment-1
3.       Upload   the   zipped   file   found   under   the   assignments   section   in   canvas   –   happy   coding!
Setting up   MongoDB This   application   being   sent   relies   on   a   local   MongoDB   application   to   store   the   notes   you   are   taking.   For this   application   the default installation   will   suffice.   Below   are   steps   on   how   to   install   and   run   MongoDB.   You will   NOT   be marked on your   DB   but   it   NEEDED to ensure your   node application   works   before   and      after   updates. You   will   need   MongoDB   Community   and   MongoDB   shell.
GUIDES:
https://www.mongodb.com/docs/manual/tutorial/install-mongodb-on-windows/ 
https://www.mongodb.com/docs/manual/tutorial/install-mongodb-on-os-x/ 
https://www.mongodb.com/docs/manual/administration/install-on-linux/ 
1. https://www.mongodb.com/try/download/community 
Follow the   instructions   here for installing   MongoDB. When   installing,   please   use all DEFAULT settings   to   ensure   the   application   connects   properly.
2. https://www.mongodb.com/try/download/shell 
Once   MongoDB   is   installed,   install and   run   MongoDB shell to actually   run the database to allow   connections   locally.
Tasks The   Alpine   Inc   team   needs   to   be   able   to   understand   why   you   chose   to   approach   your   solution   the way   you   did. Create   a   document   with   details   for   each   of   the   elements   in   your   solution, explain   how the element works and   how   it forms   part of the   overall   DevOps   process. Write   as   little   as   possible   to   communicate   your   message. Add   screenshots   where   appropriate   to   demonstrate   that   you   have   completed   the   requirements   of   each   section.
For   a   Pass 
1.      Create   a   Readme.md   at   the   root   of   your   git   repo   that   contains   the   following:
a simple explanation of how the   pipeline   is   run (what   commands   will   cause   the   pipeline to   run correctly, what output   is expected)      (4   marks)
2.      Create   an   analysis.txt   file   at   the   root   of   your   git   repo   that   contains   the   following sections:
a)      Analysis of the   problem (What are you trying to   solve?)   (2   marks)
b)      Explain and justify the solution (How does the solution work?)   (1   mark)
c)      Writing quality,   layout, and accuracy   (1   mark)
3.    Things   that   need   to   be   added   to   your   Continuous   Integration   build
a)      Static Code Analysis /   Lint   (2   marks)
b)      Unit testing   (2   marks)
c)       Ensure code coverage   is checked   (Hint:   Research   how you   enable   code   coverage with Jest) (2   marks)
d)    Generating an   artefact that   can   be   deployed   (2   marks)
4.    A   proper branching   is   implemented (GitHub   Flow   is   required).   Ensure   new features      are developed on feature   branches and   merged   into the   main with   Pull   Requests. (4   marks)
For   Credit 
5.      Perform. all tasks   from the   previous   level and   in addition:
Ensure artefacts are generated on the   main   branch   ONLY   (4   marks)
For   Distinction 
6.      Perform. all tasks   from the   previous   level and   in addition:
Ensure   the   pipeline   works   with   multiple   branches, the   CI   should   trigger   when   a change occurs to any   branch.      (4   marks)
For   High   Distinction 
7.      Perform. all tasks from the   previous   level and   in addition:
a)      Run end-to-end tests as   part of the   pipeline.   End-to-end testing   is a test that
checks   if   the   flow   of   an   application   from   start   to   finish   is   behaving   as   expected.   The   purpose   of   performing   end-to-end   testing   is   to   find   system   dependencies    and   to   ensure   that   the   data   integrity   is   maintained   between   various   system components and systems.   Please   read the   ReadMe file on the   project.      (3   marks)
b)       Execute   automated   tests   that   validate   that   the   application   functions   as   expected from the   user   interface.   (2   marks)
c)       If the tests fail,   break the   build and   report   back why   it failed   in the   log.   (2   marks)





         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
