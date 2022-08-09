<div align="center">

# Technology Stack

The software and systems we use to build the **`dwyl`** platform.

</div>

## Why?

As a ***team of people*** using technology to **_make_ digital products**, <br />
it's _essential_ to **be _unambiguous_**
about the **technology/tools** we use, <br />
**so that _everyone_** is **clear** what we _all_ need to learn/use <br />
to make product(s) that are **functional, fast, beautiful, useable and reliable**!

> _If **anything** is **unclear** or you have **any questions** please_
[***ask***](https://github.com/dwyl/technology-stack/issues).

## What?

This document + diagram _describes_ the full "**PETE**" Technology Stack
we use for dwyl products and services (clients).

Each element in our stack was _carefully_ selected based
on its individual merits. <br />
When _assembled_ into a seamless "machine",
the stack is _unrivaled_ for **developer productivity**
and ***world-class quality***!

### The "PETE" Stack

![dwyl-pete-stack](https://cloud.githubusercontent.com/assets/194400/23000461/8688abcc-f3d8-11e6-86ab-804720619d8e.png)

"PETE" is an acronym<sup>1</sup> for the following elements:

+ **Phoenix** is a Web Application Framework that does not compromise
on speed, reliability or maintainability!
Phoenix is the "_successor_"
to the incredibly popular "Ruby-on-Rails" framework.
Built _from scratch_ by highly experienced engineers
who worked on/with Rails. It _solves_
all of the speed/socket/scaling/concurrency, issues
people felt when building/using Rails apps.
The list of ***benefits*** Phoenix has over
(_virtually every_) other Web Frameworks is _extensive_.<br />
Please see:
[github.com/dwyl/learn-phoenix-framework#our-**top-10-reasons**-why-phoenix](https://github.com/dwyl/learn-phoenix-framework#our-top-10-reasons-why-phoenix) <br />

+ **Elixir** is the _functional_ programming language used
by the Phoenix framework. Elixir is a _beautiful_ language
written _from scratch_ to be ***friendly, concise and efficient***.
***Yes***, Elixir not as "_popular_" as JavaScript, Java, C# or PHP,
but the adoption is _growing rapidly_ and most importantly
many _experienced_ developers are gravitating towards and
describing it as their ["most wanted"](https://github.com/dwyl/the-book#you-will-learn-in-demand-tech-toolsskills)
Also a language's popularity has more
to do with the intellectual inertia people/companies have because
they allow existing (_legacy_) codebases to dictate future development;
i.e.
[***sunk cost bias***](http://www.investopedia.com/terms/s/sunk-cost-trap.asp).
see: [github.com/dwyl/learn-elixir#key-advantages](https://github.com/dwyl/learn-elixir#**key-advantages**)

+ **Tachyons** is the most _sane_ way of creating a _beautiful_ web app UI
that can _easily_ be extended by a team of people
without fear of one person's change "_breaking_" another feature.
Unlike "_traditional_" CSS which - _as it's name implies_ - encourages
"_cascading_" of styles, Tachyons makes the style of each component _specific_
and _local_ to that component.
see: https://github.com/dwyl/learn-tachyons

+ **Elm** is a front-end developer's _dream_
made _reality_ by a community of unbelievably
brilliant and dedicated developers. <br />
While Elm is
[***incredibly fast***](http://elm-lang.org/blog/blazing-fast-html-round-two)
the _reason_ we love elm has _nothing_ to do
with "_benchmarks_" and everything to do
with the _experience_ of writing/reading/maintaining
an app built with elm; _that experience is like
a **reassuring hug** from a loved one_. <br />
When you discover elm, things that used
to be _difficult_ or "_error-prone_" become easy and ***reliable***.
See: [github.com/dwyl/learn-elm#why](https://github.com/dwyl/learn-elm#**why**)


Elm has [***considerably*** **better performance**](http://elm-lang.org/blog/blazing-fast-html-round-two)
than similar/alternative front-end frameworks
(e.g: Angular, Ember, React, Vue.js etc.)
so _hopefully_ the "performance" discussion can _"go away"!_


¹Thanks to [**Jimmy Ruts**](https://github.com/dwyl/technology-stack/issues/37#issuecomment-278282619)
for _coining_ the "PETE" acronym. He's the guy we go to for _naming_
and other "[**hard things**!](https://twitter.com/codinghorror/status/506010907021828096)"
;-)

## Database?

The _reason_ we do not _specify_ our Database in the "PETE" Acronym is
that Phoenix allows us to use **_any_ Relational Database**.

By _abstracting_ the data layer using "Ecto" the application is "_decoupled_"
from the database. <br />
This means that if a client _asks_ us to deploy to MySQL or
Microsoft SQL Server <br />
(_e.g. because they already have in-house capability
  for maintaining one of these databases_) <br />
we can easily accommodate that without re-writing _any_ of the Phoenix app!

### We _Prefer_ PostgreSQL (Postgres)

![postgresql logo](https://cloud.githubusercontent.com/assets/194400/22939394/6cc00918-f2d6-11e6-8400-77886d70b520.png)


Our "_standard_" (_preference_) @dwyl is for Postgres.
see: [github.com/dwyl/**learn-postgresql**](https://github.com/dwyl/learn-postgresql)
<br />
Postgres is the most "_mature_" Open Source Relational Database.
It's ***100% Free*** (_including all **"advanced"** features_) <br />
and has been deployed and ***battle-tested*** in ***every*** environment
from AWS to "Bare Metal" and Google Cloud to Microsoft Azure!


> _**Many** well-known/successful apps rely
on Postgres as their `main` database_. <br />
> _**NOT** that you should adopt a particular technology
based on who `else` is using it,_ <br />
> _but it's **good to know** that **plenty** of teams
are getting **excellent results** with PostgreSQL!_
<br />

##### See: [List of Organizations Using PostgreSQL](https://github.com/dwyl/learn-postgresql/issues/31)

We have used _most_ of the "_popular_" Relational Databases.
e.g: MySQL, MS SQL Server, Oracle and Aurora; all
[RDBMS](https://en.wikipedia.org/wiki/Relational_database_management_system)
have their pros/cons. <br />
The ***reason*** we like/use Postgres is because the ***community***
is _superb_. There is a great "_bank_" of _answered_ questions on
[StackOverflow](http://stackoverflow.com/questions/tagged/postgresql)
and new questions get answered _fast_.

## Operating System?

A _"traditional"_ **LAMP** stack includes the **Linux** Operating System
in the _name_. <br />
The "**PETE**" stack runs on _any_ (_desktop/server_) Operating System <br />
and can be deployed to any "_cloud_" infrastructure provider. <br />

While we have a _strong_ preference for Unix (e.g. FreeBSD) or
Linux (_e.g. Ubuntu or CentOS_) we know that <br />
_both_ Phoenix and Postgres run
on almost _any_ environment _including_ Microsoft Windows Desktop & Server.


## Continuous Integration

We use and *recommend* Travis-CI for Continuous Integration (CI).
If you or anyone on your team are *new* to Travis-CI,
please checkout our ***complete beginner's guide***:
[github.com/dwyl/**learn-travis**](https://github.com/dwyl/learn-travis)


## Deployment

We make a point of deploying our work as _soon_ as
there is something worth showing to the target audience of "_end users_"
so that we can get ***feedback*** as early as possible.

### "Development" and Testing

We use Heroku for all our development deployment.
It's **by _far_ the most time-effective** way to "_ship_" <br />
the project and get it _tried & tested_ by _real_ people.
Using heroku is like having a "Dedicated DevOps" person
on the team. <br />
Once the deployment is configured we can automatically deploy
a _new version_ of app for each feature and test incrementally.<br />
This alone is worth the _modest_ fee Heroku charges for their service!
<br >

> If you are _completely_ `new` to Heroku you can get started
in 10 minutes with our <br />
***complete beginner's tutorial***: https://github.com/dwyl/learn-heroku <br />

> For a ***step-by-step guide*** to **deploying** a Phoenix ("PETE")
application to **Heroku**, <br />
please see:
[github.com/dwyl/learn-phoenix-framework/**heroku-deployment**](https://github.com/dwyl/learn-phoenix-framework/blob/master/heroku-deployment.md) <br />
(_special thanks to [Tony](https://github.com/tonydaly) & [Jimmy](https://github.com/jruts) for doing a superb job putting the guide together!_)

"_Under the Hood_" Heroku is using AWS for their infrastructure. <br />
So when we need to "_graduate_" an app from Heroku to AWS it's easy!

### "Production"

Our _preference_ is to deploy to Amazon Web Services (AWS)
because we have good experience/knowledge of the platform.

### Microsoft Azure

One of our projects has a _requirement_ to be deployed
to Microsoft Azure Cloud. We achieve this with the following
configuration:

#### Application Server

The Phoenix Application Server is hosted on (_a minimum of_)
Two Linux Servers. <br />
(_often many more which **message**
one another to distribute load as a cluster_). <br />
The "_cluster_" is managed by Erlang's "Supervisor".
The Erlang Supervisor is the "_Gold Standard_" in infrastructure management,
having been used by Telecoms companies for over 20 years in production
with some Telcos reporting 99.99999% ("_seven nines_") of "_up-time_".

> It's _far_ more likely that the _infrastructure_ provider (_e.g. AWS/Azure_)
will have a fault in their network/datacenter than an Erlang server "crashing".


#### Database Cluster

Thanks to Esmaeil Sarabadani of Haufe.com there is a "Template"
for deploying a ***Highly-Available PostgreSQL Cluster on Azure***
this can be setup with only a few clicks and scaled automatically
to as little or large as required!
See: http://dev.haufe.com/PostgreSQL-Cluster-Azure/

#### SSL/TLS Encryption

All communication is over secure/encrypted channel
(_by default at all times_) <br />
to protect the data/privacy
of people using the applications we make. <br />

We recommend using the "Let's Encrypt" service for SSL Certificates
it's ***100% Free*** (and _provided by a Non-Profit foundation_) <br />
to help you get started, we wrote a
***step-by-step setup guide*** for apps deployed to Heroku:
[SSL-certificate-step-by-step-setup-instructions.md](https://github.com/dwyl/learn-heroku/blob/master/SSL-certificate-step-by-step-setup-instructions.md)

### Beginner Tutorials?

We have _crafted_ a "***Complete Beginner's Guide***"
for each element in the stack, so that we:
+ ***Document our collective learning***
`while` we are building projects.
(_because as humans we **forget fast** unless we **write it**_!)
+ ***Share*** our knowledge with other people so we can
  + Help to train (_potential_) new team members
  as quickly/effectively as possible.
  + ***Collectively iterate*** on our knowledge and "_level-up_" as a _team_!
  + "Onboard" the client team (_who may want/need_) to
  support/maintain the codebase/project if/when we _seamlessly_ "hand over".
  + Inform the wider community of both technical _and_ non-technical
  people ("stake holders") who are _generally_
  interested in _understanding_ the project.
  + Enlighten other teams/organisations/agencies/etc. we aren't in
  _direct_ contact with that there is a "_more fun_" way of building software!
+ Make _everyone's_ life easier/better
by having a "launch pad" for
[_rapid_ learning](https://youtu.be/hOZnP4dZYK0 "Matrix Easter Egg ;-)")!

> For an _example_ project where this "Stack" is _implemented_
see: https://github.com/healthlocker/healthlocker


<br /> <br /> <br /> <br /> <hr />




# tl;dr

There is _no shortage_ of options available for
Technology Stack! <br />
See: https://www.google.com/search?q=technology+stack&tbm=isch <br />
So, _how_ did we _arrive_ at the conclusion that "PETE"
was "_the **one**_" for us...?
We _already_ had a _really_ good
[Node.js Stack](https://github.com/dwyl/technology-stack#nodejs-stack)
which worked well for us and our clients. so . . .


## Why Try a "New Stack"?

#### Why Try Something New When We're _Already_ Good with the "Old"...?

Our _reasoning_ for
_considering_ an alternative approach/stack for building web apps
was fueled by our
[_curiousity_](https://www.goodreads.com/quotes/tag/curiosity)
and
["_shoshin_"](https://en.wikipedia.org/wiki/Shoshin). <br />

> "_The important thing is not to **stop questioning**. **Curiosity** has its own reason for existence._" ~ Albert Einstein <br /> ~
"Old Man's Advice to Youth: '**Never Lose** a Holy ***Curiosity***.'"
LIFE Magazine (2 May 1955) p. 64”

In November 2016 we (_once again_) **questioned our _assumptions_**,
***re-examined*** and
[***surveyed***](https://github.com/dwyl/learn-elm/issues/10)
the "landscape" of "_emerging trends_" in web app development.
We were ~~pleasantly surprised~~ ***delighted*** to see the _amazing progress_
made by the people in the Elixir, Phoenix and Elm communities!
These technologies are set to "***take off***" in 2017 and we are _excited_
to be _sharing_ the technical/competitive advantage with our clients!

Please see: https://github.com/dwyl/learn-phoenix-framework#questions

## Making Difficult Decisions

One of the most "_difficult decisions_" you will make in your "_career_" is
which technologies and tools you will use
to deliver the desired solution/benefit to the "_end users_".

Most people have the Tech/Tools decision made _for_ them
by the company/organisation/boss they work for
(_e.g: Java -> Spring, Ruby -> Rails or PHP -> WordPress or Symphony, etc._)
This is because most companies _already_ have an _existing_ app in "production",
which you have been hired to extend.

Occasionally you will get the chance to build an app from "_scratch_"  
however _most_ of the time someone `else` (_the "Architect"_)
will make the decision for what "_stack_" to use on your behalf,
so you will _still_ be stuck with someone _else's_ choices.
If you are _incredibly lucky_ the "Architect(s)"
will have done their homework: surveyed the latest industry
trends and investigated the "_new and promising_" technologies
e.g: Stack Overflow
["Most Wanted" list](https://github.com/dwyl/the-book#most-wanted-programming-languages).

#### _Most_ "_Application Architects_" will pick one of these 3 options:

1.  ***Go with what you (already) know***, use _existing_ stack
with a minor variation because it's "easy to deploy" with
the existing infrastructure and will not get questioned by the "Executives",
DevOps team or "Compliance" department. This is the easy choice
and nobody ever got "_fired_" for sticking with what they know "_works_".

2.  Buy the whizz-bang all-in-one solution sold to them by the "Consultant"
from "Big Vendor XYZ" (_outsource the thinking to a sales person who last
  wrote code in the 90's ... seems like a great idea ... NOT!_)

3. Be "Bold" and try "***Popular Framework XYZ***" and hire an _external_
team to build the new magic app. Then attempt to "_up-skill_" the _internal_
team to _maintain_ the code written by the consultants.

None of these choices is _optimal_, all have different levels of risk/reward.
The "_hardest_" choice to make is the one where you try something
_totally_ different
The _reality_ is that very few people
have the time/resources/mindset/inclination to take a step back
and open their minds to the idea that there _might_ be a "_better tool_"
for the job than the one they are _currently_ using.

### Toast Knife Analogy

Imagine Want to Make Yourself Some Toast.
Let's write a quick "_user story_" for this:

> `As a` **peckish person** <br />
> `I want` a slice of tasty toast <br />
> `So that` I can have some crunch for my brunch!

> (_let's assume that you bought a loaf of bread from a baker
to reduce the options for solutions for simplicity
(i.e. not baking from scratch!_)

The "_traditional_" way to "_solve_" the challenge of making toast: <br />

+ Cut bread with bread knife
+ Put sliced bread in toaster
+ Turn on toaster for pre-determined amount of time
+ Wait patiently for toaster to make toast


But ... what if instead the "_old_" way we just described,
someone invented a way to _toast_ the bread `while` slicing it...?!

![b4df5698-914e-4dd2-b271-9c00881b6599-274-0000001c8c73f018_tmp](https://cloud.githubusercontent.com/assets/194400/22363833/07798ad6-e465-11e6-9d92-44898a774148.png)
![9f9fc56d-b22a-4e77-b60f-f3619254023b-274-0000001ce1dcb22a_tmp](https://cloud.githubusercontent.com/assets/194400/22363837/0d860594-e465-11e6-9dcd-292f441983b0.png)

Simply by using the "***New Tool***" - _in this case the
["**Toast Knife**"](https://youtu.be/3ttzWuaPGMo?t=1m1s)_ - you can
simplify the process to a ***single step***! <br />
This is the power of being _open_ to considering "New" Tools/Technologies!
Get the ***same result*** in **fewer** than half the "**steps**"!

### Focussing on Long-term Benefits

The _short-term_ cost of learning a new stack
(_programming language or framework_) is time,
We contend that the 1-3 week learning time (_depending on the focus of learners_)
will pay for itself within 3 months
(_often sooner if the team is large/distributed because the **structure**
  offered by Phoenix means everyone working on the project
  has a disciplined approach to adding new features_)

#### Further Reading on Long-term Thinking

+ https://hbr.org/2012/08/thinking-long-term-in-a-short
+ https://hbr.org/2011/03/capitalism-for-the-long-term

### *Contextualising* Technology Adoption (_Mini History Lesson_)

In **1996** Nokia introduced the
["***Communicator***"](https://en.wikipedia.org/wiki/Nokia_Communicator)
and was a **_incredible_ revolutionary innovation**!
**Internet, Email and _Fax_** in your ***Pocket***!! <br />

![nokia-communicator](https://cloud.githubusercontent.com/assets/194400/23014351/89c07b64-f426-11e6-8c5a-f93b71a3aa53.jpg) <br />

Nokia continued to _dominate_ the mobile phone industry/market for the next
***decade*** producing the _best-selling_
**5110** and **3310** we all remember! <br />
But by being "_ahead_" Nokia was _unable_ to see the "_contender_"
coming "_out of nowhere_" to challenge their position.

In 2006 _nobody_ was making/buying "smart" mobile phones
with glass touch screens that ran "apps" ... <br />
in [January 2007 Steve Jobs introduced the iPhone](https://www.youtube.com/results?search_query=Steve+Jobs+iPhone+Introduction+2007)
and _literally_ changed the industry!

![Steve Jobs introduces iphone](https://cloud.githubusercontent.com/assets/194400/22934275/4bc76090-f2c6-11e6-9b90-91226e39ea09.png)

The dominant/incumbent mobile phone maker **Nokia** had
[***49% market share in 2007***](http://www.bbc.co.uk/news/technology-23947212)
_mocked_ Apple's lack of features, poor battery life and high price. <br />
By 2013 Nokia had 3% Market Share (_for new device sales_) and was sold off "for parts" to Microsoft
while Apple was the [most valuable company](https://www.statista.com/statistics/263264/top-companies-in-the-world-by-market-value/)
in history!

> _Many **people still buy** "**feature phones**"
(the polite name for a device that does not have any
  "smart" functionality!) <br />
but few people can **convincingly** argue that the **reason**
they **don't have** a smart phone is because they **don't want** one; <br />
[**over 90% 16-24 year olds own a smart phone**](https://www.ofcom.org.uk/about-ofcom/latest/media/media-releases/2015/cmr-uk-2015) and that number is expected to reach 100% by 2020 ... <br />
ask someone in their 20's if they would go "**back**"
to using a non-smart phone
and see what they say ... "**No Way**!!" <br />
they laugh uncomfortably and
admit that: "**My Smartphone is my Life**!" <br />
We feel **exactly** the same about "**old technology**".
Sure the "**old way still works**",
but if you can **inexpensively switch** <br />
to something **demonstrably better** in **every aspect**,
why would you stick with the "feature phone" of web frameworks...?_ <br />
_It's like taking the Bus to work when there's a perfectly
good teleporter right next to the bus stop!! Madness._

We are not _suggesting_ that _everyone_
is going to _suddenly_ flock to the "**PETE**" stack
the way people adopted smart phones.
This is merely an _illustration_ that when a technology
has a _specific/measurable_ advantage to it's users
the adoption _can_ be _fast_.

In the case of programming languages or application frameworks,
moving one framework to another is a _much_ more difficult decision.

But one thing is for _sure_ we are going to use the "_smart phone_"
even if other people insist on using the "brick".


### But Phoenix Uses Node.js for Static Asset Compilation ...

***Yes***, if you are using the (http://brunch.io/)
"_static asset compilation_".
We _aren't_ using it for our project(s) because our only
"_static assets_" are the Elm files which we compile using `elm-compiler`.
The [`elm` compiler](https://github.com/elm-lang/elm-compiler)
is written in Haskell so technically we aren't writing _any_ JS
in our PETE projects.


### Does it _Scale_?!?

If you are new to web development,
_please focus on UX and forget about "**scale**"_! <br />

> _Unless you work somewhere that
  **already** has "**millions of users**" and <br />
your team **cannot consider** anything that
does not support a million concurrent connections...!_ <br />

> _But let's face it, **most** people have [**imaginary scaling
issues**](https://twitter.com/ThePracticalDev/status/800752571497545729)
not **real** ones. <br />
discussing "scalability" before you have 10,000 paying customers is
a waste of time!!_ <br />

Stop worrying about "scalability"
and instead **focus** on building something **useful** <br />
**focus** on **User Experience** not "backend" **scalability**!

The _good_ news is that Phoenix "***scales***" _really well_! <br />
see: http://www.phoenixframework.org/blog/the-road-to-2-million-websocket-connections

Forget about "_scaling_" until you have _made_
[***something people want***](http://paulgraham.com/good.html)
and are _paying_ for! <br />
Then _use_ the pile of cash you got from your product
to hire "_engineers_" to make it _available_ to more people!!

<br /> <br />

### _No JavaScript_ in "PETAL"...?

![no-javascript](https://cloud.githubusercontent.com/assets/194400/22939705/88d3e524-f2d7-11e6-91c6-47513f6b4fa7.jpg)

This not the place to "diss" JavaScript;
_plenty_ of people have written blog posts/tweets "_ranting_"
about the
["_State of Web Development_"](https://medium.com/@wob/the-sad-state-of-web-development-1603a861d29f).
<br />
e.g: Douglas Crockford (_the authority on JS_) recently gave a presentation on
The **Post JavaScript _Apocalypse_**: https://youtu.be/6Fg3Aj9GzNw <br />
(_in which he describes all the "features" of JS that are "**unnecessary**"..._)
<br />
Or Max Ogden (_a prominent JS developer_) who created
a website dedicated to the "Callback Hell" issue: http://callbackhell.com <br />
why do we even _need_ to have an _expression_ for that?
why can't ***elegant*** asynchronous control flow
be the **_only_ way** to write code?


The **fact** is: we _only_ use JavaScript because it is the
["***Lingua Franca***"](https://en.wikipedia.org/wiki/Lingua_franca)
that _all_ web browsers "_understand_".<br />
It's _definitely_ not because it's a
"_better_" language than Python, Julia or Lisp;
we write JS out of _necessity_ not _choice_. <br />


With Elm we no longer _need_ to write our Client-side
(_progressive enhancement_) code in JavaScript!
We can write in a beautiful/functional language <br />
and "_compile_" it to JS for running in Browsers.
The JS that is produced by the Elm compiler
is almost _always_ more efficient/faster <br />
than "_hand-written_" JS,
so _why_ would we waste our _time_ with writing JavaScript...?!

> _If you aren't `.ready()` to try something (way) **more productive**
than **JavaScript**, `.then` please just **ignore** `this`! <br />
We have written this "Technology Stack" description for **ourselves**
and not because we want to "**convince**" anyone. <br />
But ... we wanted to put down our thoughts
in `case` anyone is
["**on the fence**"](https://en.wikipedia.org/wiki/Sitting_on_the_fence)!
If you're in any doubt, ***Just Do it***._

![just-do-it-nike-log](https://cloud.githubusercontent.com/assets/194400/22940322/63db1308-f2d9-11e6-8d84-e024b00e37a4.png)

### What About _Full Stack JavaScript_?

We still think that "***Full Stack JavaScript***"
is a ***compelling proposition***
_especially_ for people who are just starting out!
However we have learned from years of experience



### Alternative Databases?

If we were to _consider_ an alternative to SQL, we
would use RethinkDB:
https://rethinkdb.com <br />
But we are _relieved_ that the Phoenix team
is _focussed_ on PostgreSQL because that _eliminates_ <br />
the "ambiguity" or "discussion" of "_which database_" to use!
Postgres is a _fantastic_ "_general purpose_" <br />
store that has a _rich_ ("_structured_") query language
that lets you JOIN data!! <br />
Also, now that [Citus DB is Open Source](https://www.citusdata.com/blog/2016/03/24/citus-unforks-goes-open-source)
we _know_ that Postgres can _easily_ handle billions of writes per day!
