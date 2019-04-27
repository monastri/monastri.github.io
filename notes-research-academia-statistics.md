*[Word count](https://wordcounter.net/): 21,900*

## What is this?

This is the "research, academia and statistics" section of [this notebook](https://monastri.github.io/). 

<a name="#overview"></a>

## Overview

I've sorted the quotes below into the following categories. This is a provisional taxonomy, subject to perpetual refactoring. The reason it has a [Borgesian flavor](https://github.com/monastri/monastri.github.io/blob/master/poetry.md#the-celestial-emporium-of-benevolent-knowledge) is that it's meant to aid recall and idea-building. The categories are ordered alphabetically; the actual quotes (the top-level categories that is) are chronologically added.

1. [Advice and tactics](#research-tactics)
	1. [Using Anki to read a paper in an unfamiliar field thoroughly](#anki-in-research)
2. [Debt, interpretive labor, distillation](#distillation-and-research-debt)
2. [Doing science better](#Doing-science-better)
	1. [Science should be more like open-source software](#Science-should-be-more-like-open-source-software)
1. [General statistics](#general-statistics)
2. [Mindset](#research-mindset)
2. [Productivity](#Productivity)
	1. [Structured procrastination](#Structured-procrastination)
	2. [Tactical procrastination](#Tactical-procrastination)
	2. [Batch low-intensity tasks](#Batch-low-intensity-tasks)
	2. [Resize value batches](#Resize-value-batches) (Tiago Forte takes the obvious idea and runs away with it)
	2. [Email](#email)
2. [Research in industry](#research-in-industry)
2. [Statistical literacy](#statistical-literacy)
2. [The general function of intellectual traditions](#role-of-intellectual-traditions)
2. [The role of statistics in doing science](#the-role-of-statistics-in-science)
2. [Why academic writing sucks](#why-academic-writing-sucks)
2. [Why I left academia](#Why-I-left-academia)

--------------------------------

<a name="#Doing-science-better"></a>
## Doing science better
([overview](#overview))

Honestly most of the "research" part of this sub-notebook is about how to do science better. 

<a name="#Science-should-be-more-like-open-source-software"></a>
### Science should be more like open-source software
([overview](#overview))

Brian Armstrong's essay [Ideas on how to improve scientific research: bridging the gap from scientific discovery to new products](https://medium.com/@barmstrong/ideas-on-how-to-improve-scientific-research-9e2e56474132) argues that science should be more like open-source software. Brian, it turns out, doesn't waste words at all, so I had difficulty not just quoting his entire essay. I like this no-BS, every-sentence-is-here-for-a-reason style, even though I don't necessarily aspire to it (except in certain contexts, like convincing no-BS people I have something interesting to say). 

Academic research, Brian claims, is inefficient in terms of

	prioritization of what to work on
	reproducibility of results
	alignment to market incentives
	access to funding
	cost and delays from academic journals	
	
These are depressingly familiar themes. I still like Brian's short-n-sweet executive summary of each.

For instance, here's the reproducibility issue:

	In some fields, more than 50% of experiments are not able to be reproduced.
	Many papers do not include the underlying datasets. Researchers sometimes
	have an incentive to hide key details in their paper to stay one step ahead 
	of competing labs. In addition, negative results⁵ are less likely to be published.
	
Prioritization (see also GiveWell on [cause prioritization](https://causeprioritization.org/Cause_prioritization)):	

	We often don’t fund or pursue work that would do the most good⁶. While it can
	be difficult to tell what a line of inquiry will eventually lead to (many 
	great discoveries happened while looking at something unrelated), it would be
	nice if there was a better feedback mechanism from private industry about the
	most important challenges they are facing. This ties into “market incenives” 
	below. One scientist I spoke with while writing this post shared an anecdote 
	that “In my field of [redacted], I see >70% of publications being on technology
	that will never come close to commercialization. [a recent big push of $100M 
	in funding] yielded, in my opinion, nothing.”
	
Market incentives:

	Research seems too disconnected from the real world at times, perhaps because 
	scientists don’t often capture the financial upside of their work. Instead, they 
	use alternate currencies (like citations). Perhaps licensing⁷ could be simplified
	to align research more with market incentives and help scientists capture more 
	upside form their inventions.
	
Funding:

	It can take a huge amount of time for researchers to apply for grants and receive
	funding⁸. They often have to alter their ideas⁹ to fit them into grant proposals
	(i.e. could I argue that this is somehow relevant to defense spending?¹⁰) and a 
	lot of money goes to running the university itself (about 50% at Stanford, for
	instance). In addition, a lot of NIH/NSF funding is arguably too conservative.
	The people writing the grants are trying to minimize downside, not maximize 
	upside, which means they are likely to overlook (contrarian) breakthrough ideas.
	
Speed:

	Making a new discovery is difficult enough, but once one is made, it can still
	be many years before it sees the light of day. The process of applying to 
	journals and peer review adds a lot of delay. In addition, people are hesitant 
	to publish in-progress or half finished work (although “pre-print” servers have
	helped with this), so there is a tendency to wait until something is “done” to 
	share it.
	
Comprehensibility, which ties in to [research debt](#distillation-and-research-debt) and [terrible academic writing being the norm](#why-academic-writing-sucks):

	Academic papers use a lot of jargon that is only decipherable by other people
	in the field. Some of this is unavoidable (research is about complex topics),
	but it also makes it less likely that people outside the field will understand
	the potential of a new discovery.
	
Volume:

	There are a large number of papers published, some without much original content.
	This can make it difficult to wade through all the material out there to see what
	might be relevant to you.
	
Cost/accessibility, i.e. "goddamn paywalls":

	There are a large number of papers published, some without much original content.
	This can make it difficult to wade through all the material out there to see what 
	might be relevant to you.
	
	The academic journals seem to slow things down in terms of time and money, in
	exchange for providing some curation and credentialing. The aggregate revenue of 
	the academic journals is about $20B annually, for little value add.
	
What Brian calls the "ivory tower", which sounds to me more like fragmentation due to balkanization and this-is-my-turfing:

	Research can take place anywhere from CERN’s Large Hadron Collider to a garage, 
	and be done by anyone from tenured professors to hobbyists (or even anonymous
	people). It can also take place in private companies, and in any language 
	(right now there is a barrier between machine learning papers published in 
	Chinese and English). It would be nice to see a wider definition of research
	come together all in one community.
	
Brian wants research to be "more like open-source software" (yay!) and "more aligned with market incentives (not sure about this, sounds like a potential failure mode). He wants "prioritization like Reddit, comments like Google Docs, and pull requests like GitHub" (also yay!). 

His proposed solution? 

	an app or website that brings together a community of researchers in a novel
	way. It attempts to improve the quality and speed at which research gets done,
	how it gets communicated to entrepreneurs and business people, and how scientists
	could get funding and upside.

	This is idea is not very new, I just don’t think it’s been executed on yet.

	You’ll see elements of Reddit, Github, Wikipedia, StackExchange, RapGenius, and 
	Kickstarter present. Part of this is really just taking the best of what is 
	already working online.

	The other part of this is providing a viable alternative to scientific journals.
	To do this we need to replicate the positive aspects of journals (curation of
	content and status/reputation for those getting published) and eliminate the 
	negative aspects (cost and delays).
	
How to solve prioritization? PageRank-style:

	The sheer volume of papers published every day is overwhelming. If we can get 
	trusted people to rate papers, we can turn this into rankings or leaderboards. 
	Imagine being able to see the “top papers in biology this year/month/week” based 
	on crowd sourced votes from knowledgeable people. If you only have a few hours 
	to read papers in a month (like me), this would help a lot.

	Perhaps out of some sense of politeness, people in academia seem to be reluctant
	to give a thumbs up/down to their colleagues work in a public forum. Journals 
	often don’t publish the identity of the people doing the peer review. This strikes
	me as a key part of the problem.

	The ratings could be similar to Google’s Page Rank algorithm, meaning they are 
	weighted by how knowledgeable or trusted the rater is.

	I could imagine research being rated across a handful of metrics:

	1. Originality: Is there a genuine breakthrough here that added a branch on the 
	tree of knowledge?

	2. Reproducibility: Does the paper contain sufficient detail for others to reproduce
	the work, and how many other people/labs have actually been able to do so?

	3. Commercial viability: Could this research plausibly lead to something that would
	benefit people?

	These ratings could be aggregated into an overall score for each paper, possibly
	eventually incorporating hundreds of variables (like Page Rank). There are some
	basic rankings today, such as the H-Index, which looks at how often a paper is cited.

	It would be interesting to try aggregating papers into meta studies as well, to
	generate a “confidence” score on a particular conclusion, and see how it has changed
	over time.

	There should be some way to clearly mark research as “in progress” as well to prevent
	people getting negative ratings before it is really “finished”. In theory, all
	research is “in progress”, so the idea of a static PDF seems woefully outdated.
	
Of course I agree with the last part by the way. It's [the entire reason this notebook exists](https://github.com/monastri/monastri.github.io/blob/master/README.md).	

I also approve of Brian's sketch at a score for meta-analyses. 

How to gain trust, so people use the platform? Reputation like Reddit/SE:

	The reputation of the people doing the rating (and discussion) in the community is
	the other key component here. For this site to be trusted, the people with real
	knowledge of a field need to have their voice rise to the top, and not be drowned
	out or bullied by the internet trolls. Similar to other online forums (Reddit, 
	Hacker News, StackExchange) users should develop a reputation over time based on
	their contributions. This can be derived from their comments, edits, original 
	research, or it could be their reputation outside of the app (LinkedIn, more 
	traditional academic credentials, etc) which could appear on a profile page. In
	other words, traditional academic credentials shouldn’t be the only way to develop
	a reputation in research. ...
	
	The most important reason to have reputation on the site is just to have sane 
	discussion take place so that legitimate scientists feel they can interact with 
	other rational people.
	
Should we allow anons? Yes, to allow dissent without repercussion:

	It’s an interesting question about whether the site should allow anonymous users. 
	My instinct is to say yes, and allow users to be anonymous if they want to. The
	reason is simply that there are some fields where it is difficult to offer a 
	dissenting opinion without repercussions. As Sam Altman points out, “nearly all 
	ideas that turn out to be great breakthroughs start out sounding like terrible 
	ideas”. Galileo was famously imprisoned for proposing the idea that the earth 
	moved around the sun. Satoshi proposed the idea of Bitcoin under a pseudonym. 
	I’ve heard stories from a handful of scientists who faced retaliation when their
	research was contradictory or competitive with another well respected person in
	the field.

	Users who want to remain anonymous may not be able to bring their external 
	reputation with them to the site (this is downside), but hopefully they can
	speak freely and “crazy” ideas can be evaluated on their own merit.
	
How to align incentives, encourage participation? Incentivize community norms with money, e.g. an ICO:	

	How do we align incentives amongst everyone in this community? We want to encourage
	participation (submitting research, commenting/editing, etc) and also fund research 
	that the community deems worthy.

	One idea on this is to do an ICO of sorts, and give away a coin that incentivises 
	the behavior the community needs to keep growing. People could potentially also 
	apply for grants and get paid in this new coin.
	
How to capture commercial upside? By simplifying the hell out of licensing -- the dream is one-click a la Amazon:

	Today, there is a ton of promising research that never gets commercialized.
	When it does happen, a company or entrepreneur typically reaches out to the
	tech transfer office of the university to try and license the technology. Or
	in some cases, the researchers themselves try to spin out companies, with
	varying degrees of success.

	I wonder if the process of licensing technology from researchers could be made
	much simpler. Imagine having a “License” button at the bottom of every research
	paper profile page that hand holds you through the process. Or imagine having
	standard licensing terms, similar to the YCombinator SAFE documents, but for 
	licensing the technology. Ideally, people could license your technology in 5 
	minutes, without ever having the pick up the phone.

	Every piece of research published could be available under one of the following 
	licenses (for instance):

	1. Free, public domain: This could actually be a requirement depending on the 
	source of funding.

	2. “Standard” license terms: For instance, receive 1–5% of profit for any product
	derived from it for the first 5 years. Non-exclusive license.

	3. Custom: Contact the tech transfer office (or equivalent) to discuss a custom deal.
	
I'm never sure when it comes to aligning with market incentives, because the market is [Not Your Friend](https://slatestarcodex.com/2014/05/23/ssc-gives-a-graduation-speech/). 

How to make research more comprehensible? Plain English summaries:

	I find most academic papers to be fairly challenging to read, so it would be
	great to see a “plain English” explanation of what each paper attempted to do,
	and what it found. These summaries could be crowdsourced like Wikipedia or 
	written by paying grad students, for instance.

	Most papers contain an “abstract” and “conclusion” section that takes a good
	step in this direction, but I don’t think it goes far enough.

	I think summarizing research for a wider audience could be dramatically improved,
	perhaps targeting a high school or bachelors level of reading, or limiting 
	summaries to the N most common words in the English language. Wikipedia is a 
	great example to follow here. They have some content on how to make technical 
	articles more understandable and how to write clear articles in general. Their
	guidelines suggest a “straightforward, just the facts” style that is free from
	opinion and “available to the widest possible general audience”

	I’ve wondered at times whether scientists are hesitant to explain things in plain
	language for good reason. People may inappropriately act on what they are saying 
	as medical advice, they may be misquoted or attacked by digital mobs, or they may
	be accused of “hyping” their work instead of speaking in the precise language of 
	science. Speaking in code helps ensure that only the people they want to speak with
	can understand what they’re saying. This is a reasonable survival instinct, but it
	also means that most research is happening in small closed groups. Wikipedia I
	think demonstrates that it is possible to explain complex topics to a wide audience
	while still getting into technical detail when necessary.
	
It's definitely [not this easy](#distillation-and-research-debt), but I applaud the spirit. 

How to improve collaboration, discussion, editing? See Reddit/SE and Google Docs, as well as "perpetual drafts"/"perpetual beta":

	It would be great to see modern tools in this area applied to research.

	Sites like Reddit, Hacker News, and StackExchange have demonstrated 
	how powerful nested and voted/sorted comments are. It’s surprising to me
	that this hasn’t become ubiquitous on the internet. They are not terribly
	difficult to implement, yet the vast majority of sites on the internet
	still have comment section that are chronological and filled with low 
	quality content. This includes every site I’ve seen where academic research
	can be discussed.

	It would also be interesting to try inline comments like on Genius.com or 
	Google Docs to discuss specific lines in papers.

	Discussion is just scratching the surface though. Why not allow people to 
	submit pull requests to papers like on Github, or make suggested edits like
	in Google Docs? Why not let people add collaborators (even if they’ve never
	met in real life). Why not let people fork research and take it in a new 
	direction?

	One of the biggest issues with research today (at least in my view) is that
	teams seem to work in isolation until something is “done” or ready for publication.
	Of course, research (just like software) is rarely “done”; it is continually
	being refined. I think open source software has
	a much better model and culture here, where you make your very first commit 
	public from day one and it is never “done”. It’s totally ok in open source 
	to show work that is “in progress”. In fact, that is half the point because
	you never know who might show up to help you along the way.
	
How to reduce siloing/balkanization? The above tools, as well as Reddit/SE/Google Docs, already allow for that, and we see this in practice already -- see also small research centers like Caltech and the Santa Fe Institute that are necessarily (sometimes gleefully) interdisciplinary. Brian doesn't have much to say here that I don't already know:

	Many great innovations happen as a by product of trying to build something.
	Bringing applied scientists, engineers, and researchers closer together in one
	community could help a lot.

	It could be great to see tenured professors and tinkerers commenting side by 
	side. We could expand the number of people collaborating on a particular problem
	by 10x.
	
How to encourage perpetual beta? Incentivize research in progress, refactor "the fundamental unit of science":

	A paper implies a finished publication with a fixed set of contributors.

	It would be great if people could post in progress research as well. Maybe just
	a hypothesis (something you’d like to see tested in the future), or a dataset
	(that you weren’t able to draw any conclusions from, but maybe someone else 
	could). This could also take the form of a Jupyter notebook.

	Maybe the more fundamental unit is really an experiment. What did you try? What
	was the result? What does this imply? How sure are we that it is true/correct?
	What are some examples where this could be useful?
	
What hacks and workarounds are people already using today, since Brian's dream app above doesn't exist yet? I liked this section as a resource. Basically 

- networking/conferences/friends (problem: relies too much on happenstance)
- Wikipedia (for plain language summaries)
- GitHub (datasets)
- Arxiv.org, PubMed, PubChem, Biorxiv, etc (goddamn paywalls)
- Reddit/HackerNews/StackExchange (ranking and rep, plus filtering, subreddit-specific)
- Sci-Hub (goddamn paywalls, and screw the guys who say it's illegal)
- Google Scholar, ResearchGate
- Meta.org, OccamszRazor (using NLP to make discovering related papers easier)
- Center For Open Science (hell yeah open science!)
- Experiment.com / ScienceExchange.com (crowdsourcing science!)

Some other comments by scientists who read Brian's essay below. 

- apparently there used to be greater information flow between scientists and businesspeople, but "the modern NSF/NIH grants system arose out of Vannevar Bush’s memos, which federalized scientific research and set up a division between scientists and businessmen"
- publishing leading to additional grants being "the root of the problem":

	Grants from the NIH are the lifeline of most academic labs, and they heavily 
	weight prestigious publications i.e. Nature, Science, Cell. Many of the top
	journals are for-profit, so they are optimizing for getting the hot science
	stories first for readership (a la CRISPR), rather than reproducibility or 
	commercialization. In addition the NIH is in reality, quite risk averse, and
	skews towards funding already established investigators that are proposing 
	incremental de-risked science. We often put famous investigators on our grant
	because we knew it would increase our chances of getting grants. In my old 
	lab (one of the most highly funded in California), our PI (boss) would actually
	get grants for work he had already done and in reality use the grant for other
	new work, which speaks to how risk averse the grant system is.
	
Way too many actually, check out the essay for more.	

<a name="#distillation-and-research-debt"></a>
## Distillation and research debt
([overview](#overview))

I keep coming back to Chris Olah and Shan Carter's essay [Research debt](https://distill.pub/2017/research-debt/), which in my eyes makes it an all-time great. The key terms are 'research debt', 'interpretive labor', and 'distillation'.

What is research debt? First, a parable:

```markdown
Achieving a research-level understanding of most topics is like climbing a mountain. Aspiring 
researchers must struggle to understand vast bodies of work that came before them, to learn 
techniques, and to gain intuition. Upon reaching the top, the new researcher begins doing novel
work, throwing new stones onto the top of the mountain and making it a little taller for whoever 
comes next.

Mathematics is a striking example of this. For centuries, countless minds have climbed the mountain 
range of mathematics and laid new boulders at the top. Over time, different peaks formed, built on
top of particularly beautiful results. Now the peaks of mathematics are so numerous and steep that
no person can climb them all. Even with a lifetime of dedicated effort, a mathematician may only
enjoy some of their vistas.

People expect the climb to be hard. It reflects the tremendous progress and cumulative effort that’s
gone into mathematics. The climb is seen as an intellectual pilgrimage, the labor a rite of passage.
But the climb could be massively easier. It’s entirely possible to build paths and staircases into 
these mountains. The climb isn’t something to be proud of.

The climb isn’t progress: the climb is a mountain of debt.
```

On to research debt, analogizing to programming and management:

```markdown
Programmers talk about technical debt: there are ways to write software that are faster in the short 
run but problematic in the long run. Managers talk about institutional debt: institutions can grow 
quickly at the cost of bad practices creeping in. Both are easy to accumulate but hard to get rid of.

Research can also have debt. It comes in several forms:

Poor Exposition – Often, there is no good explanation of important ideas and one has to struggle to
understand them. This problem is so pervasive that we take it for granted and don’t appreciate how 
much better things could be.
Undigested Ideas – Most ideas start off rough and hard to understand. They become radically easier
as we polish them, developing the right analogies, language, and ways of thinking.
Bad abstractions and notation – Abstractions and notation are the user interface of research, shaping
how we think and communicate. Unfortunately, we often get stuck with the first formalisms to develop
even when they’re bad. For example, an object with extra electrons is negative. 
Noise – Being a researcher is like standing in the middle of a construction site. Countless papers 
scream for your attention and there’s no easy way to filter or summarize them. 2 We think noise is 
the main way experts experience research debt.

The insidious thing about research debt is that it’s normal. Everyone takes it for granted, and 
doesn’t realize that things could be different. For example, it’s normal to give very mediocre 
explanations of research, and people perceive that to be the ceiling of explanation quality. On the
rare occasions that truly excellent explanations come along, people see them as one-off miracles
rather than a sign that we could systematically be doing better.
```

Research debt is the accumulation of missing interpretive labor:

```markdown
There’s a tradeoff between the energy put into explaining an idea, and the energy needed to understand
it. On one extreme, the explainer can painstakingly craft a beautiful explanation, leading their
audience to understanding without even realizing it could have been difficult. On the other extreme,
the explainer can do the absolute minimum and abandon their audience to struggle. This energy is called
interpretive labor.

Many explanations are not one-to-one. People give lectures, write books, or communicate online. In these
one-to-many cases, each member of the audience pays the cost of understanding, even though the cost of 
explaining stays the same. 3 As a result, the cost of understanding has a multiplier in the interpretive
labor tradeoff — sometimes a huge multiplier.

In research, we often have a group of researchers all trying to understand each other. Just like before,
the cost of explaining stays constant as the group grows, but the cost of understanding increases with 
each new member. At some size, the effort to understand everyone else becomes too much. As a defense 
mechanism, people specialize, focusing on a narrower area of interest. The maintainable size of the field
is controlled by how its members trade off the energy between communicating and understanding.

Research debt is the accumulation of missing interpretive labor. It’s extremely natural for young ideas to
go through a stage of debt, like early prototypes in engineering. The problem is that we often stop at that
point. Young ideas aren’t ending points for us to put in a paper and abandon. When we let things stop there
the debt piles up. It becomes harder to understand and build on each other’s work and the field fragments.
```

The importance of good 'user interfaces' for ideas:

```markdown
It’s worth being clear that research debt isn’t just about ideas not being explained well. It’s a lack 
of digesting ideas – or, at least, a lack of the public version of ideas being digested. It’s a communal
messiness of thought.

Developing good abstractions, notations, visualizations, and so forth, is improving the user interfaces
for ideas. This helps both with understanding ideas for the first time and with thinking clearly about 
them. Conversely, if we can’t explain an idea well, that’s often a sign that we don’t understand it as
well as we could.
```

A great real-world example of research debt killing a field is Bill Thurston and foliations. Here's his reminiscences in my favorite paper of his, [On proof and progress in mathematics](https://arxiv.org/pdf/math/9404236v1.pdf):

```markdown
At that time, foliations had become a big center of attention among geometric 
topologists, dynamical systems people, and differential geometers. I fairly rapidly
proved some dramatic theorems. I proved a classification theorem for foliations,
giving a necessary and sufficient condition for a manifold to admit a foliation. I
proved a number of other significant theorems. I wrote respectable papers and
published at least the most important theorems. It was hard to find the time to
write to keep up with what I could prove, and I built up a backlog.

An interesting phenomenon occurred. Within a couple of years, a dramatic evacuation 
of the field started to take place. I heard from a number of mathematicians that they
were giving or receiving advice not to go into foliations—they were saying that Thurston
was cleaning it out. People told me (not as a complaint, but as a compliment) that I was
killing the field. Graduate students stopped studying foliations, and fairly soon, I turned
to other interests as well. ...

I do not think that the evacuation occurred because the territory was intellectually exhausted—
there were (and still are) many interesting questions that remain and that are probably 
approachable. ... I believe that two ecological effects were much more important in putting a
damper on the subject than any exhaustion of intellectual resources that occurred.

First, the results I proved (as well as some important results of other people)
were documented in a conventional, formidable mathematician’s style. They depended heavily on 
readers who shared certain background and certain insights. 
The theory of foliations was a young, opportunistic subfield, and the background
was not standardized. I did not hesitate to draw on any of the mathematics I
had learned from others. The papers I wrote did not (and could not) spend much
time explaining the background culture. They documented top-level reasoning and
conclusions that I often had achieved after much reflection and effort. I also threw
out prize cryptic tidbits of insight, such as “the Godbillon-Vey invariant measures
the helical wobble of a foliation”, that remained mysterious to most mathematicans
who read them. This created a high entry barrier: I think many graduate students
and mathematicians were discouraged that it was hard to learn and understand the
proofs of key theorems.
```

<a name="#Why-I-left-academia"></a>
## Why I left academia
([overview](#overview))

I like [research distillation](https://distill.pub/2017/research-debt/) more than research "generation", but:

```markdown
Lots of people want to work on research distillation. Unfortunately, it’s very difficult 
to do so, because we don’t support them.

There is a strange kind of informal support for people working on research distillation.
Christopher (Olah) has personally benefitted a great deal from this. But it’s unreliable
and not widely advertised, which makes it hard to build a career on.

An aspiring research distiller lacks many things that are easy to take for granted: 
a career path, places to learn, examples and role models. Underlying this is a deeper issue: 
their work isn’t seen as a real research contribution. 
```

From [Richard Wills' answer](https://qr.ae/TW1GCR) to the Quora question "What made you decide to leave academia after being in a PhD program in Mathematics or Physics?":

```markdown
After five years of grad school (at Caltech, in the lab of a Nobel Laureate) and three years
of post-doc’ing (at UCLA and Caltech), I decided to get out of academic science and find 
something personally more rewarding. Why?

1. Although I really enjoyed “doing” science, that is, actually dreaming up and doing the 
experiments, that was not what I saw Assistant Professors (my next step up in the academic 
ladder) doing.

2. What I saw them doing was managing a lab (consisting of others), which I had no desire to
do, and spending great gobs of time and energy applying for research grants, which I had no 
desire whatsoever to do. Frankly, being an Assistant Professor and working my way up from 
there just did not appeal. Among other reasons, I hate committee work and find sitting in 
committee meetings boring as hell. I admit it: I’m an introvert and not a team player. I
want to be left alone to do my own thing (for which grad school and post-doc’ing were ideal).

3. I also wanted to have the choice of where I and my family would live and had no desire 
to live in some podunk town where I might get a job as an Assistant Professor. I had lived 
in LA and its environs for eight years, and I had no desire to leave. (Am I the minority 
of one who actually enjoys LA?)

4. Also, I will admit that it became clear to me that after grad school and post-doc’ing,
while I may be smart and creative, I was not the next Feynman, Watson, or Crick, and that 
I was not going to get a faculty job at Caltech, Stanford, Harvard, etc., as when I had begun
this process, I had initially thought that I might. That changed my perspectives to where it
became more important to me to find myself in a life’s work that I enjoyed than being the top
dog in it.

5. Lastly, although it was not one of the reasons I left science for the law, one pleasant
outcome of that has been that I imagine lawyering has left me far more financially secure 
than remaining in academic science would have. (I was making a multiple of what a top
professor in the Ivies made. But far more to the point, I got to do what I enjoyed, work for
the clients I enjoyed, work on the legal challenges that I enjoyed, be my own Boss —- what’s
not to like about that?
```

Another big honest reason is that doing a PhD is hard, and it wasn't really the kind of thing I wanted to do. Kay Aull expounds on this articulately in [his answer](https://qr.ae/TW1uAY) to the Quora question "What are the 3 hardest things about doing a PhD?":

```markdown
**1) It's actually hard.**

When you're in school, it's hard to see how much work has gone into the knowledge you're
presented with. I don't just mean the brilliant mind that came up with whatever the raw 
material was - a theorem, a symphony, whatever. There's an insane amount of unheralded 
work that packages these raw inputs and breaks them into digestible chunks. What is the 
correct notation for working with these concepts? What is the most logical way to explain 
them to newcomers? What's important about this particular thing?

If you have an aptitude for your field, you may get through undergrad thinking that it's 
easy. Everything is self-evident. It all "makes sense". You don't realize that the well-
paved road you're walking on is surrounded on all sides by thick jungle. Now it's your 
turn to extend the road, and suddenly EVERYTHING is hard. Maybe you'll be the genius who 
invents the machete. More likely you won't be, and you'll spend the next five years 
clearing a few meters of jungle with your hands and teeth. You'll look back and think...
that was IT?! That's all I did? The difficulty gap between understanding stuff that's 
already been done, versus being the first person to do the stuff, spans a lot more orders 
of magnitude than people think.

**2) Success is ill-defined.**

Ever hear of SMART goals? Specific, Measurable, Achievable, Relevant, Timed. Grad school is
the polar opposite of that. You do get feedback, but it's typically worse than useless. 
(I’m not impressed yet. Your project just lacks that special something. If you were worthy, 
you'd already know what to do, and in fact you'd be done already.)

It is very hard to maintain a consistent level of productivity in the radical absence of 
SMART goals. No, "graduate" does not count as a goal, because there is no concrete action 
attached. You're wandering in the fog, and you have no idea if you're heading the right 
direction. You can go months, even years, without feeling like it mattered that you got out
of bed that day. If there's a more effective way to induce depression in otherwise healthy 
people, I've yet to see it.

When you're in regular school, there are assignments. When you're at work, there are
deadlines and deliverables. The rest of the world is organized this way for a reason. People
need SMART goals.

**3) Your eggs are in one basket.**

As a PhD student, you are an apprentice. Your only purpose is to convince the master that you
are worthy to join the guild. It will be his or her word that launches you to greatness. Or...
not. Then you will have the choice between being underemployed until you die or starting from
zero in a field that doesn't require specialized training. It's almost impossible to get 
another PhD position if you had a falling out with your advisor. In the real world, unless you
end up in jail or on the evening news, there are no career-ending mistakes. You can get another
job, even if your last boss hates you. Your experience in that last job still counts for 
something. It's not pass/fail.

Likewise, you have one PhD project. You may have had a few to choose from as a beginning
student, but now this one is yours. It's your identity. This is your chance to prove you can
do independent research. Or...not. Your advisor's research program cannot fail, but it can be
failed. By you. Make it work, or else. (If you disprove your advisor's pet hypothesis, which 
is THEIR identity, who do you think they will blame? Even if you merely show infeasibility,
this won't end well for you.)

In the real world, projects fail. That's a good thing! Fail fast and pivot quickly. Most people
have several projects going at once, so the loss of one isn't devastating. Sure, people get 
attached to their ideas, but there's enough pressure from above that people are generally forced
to cull the weaklings. Projects are not allowed to limp along for years (or decades!) just
because someone's ego won't allow them to admit defeat. "Oh yeah, Aull's Magnificent Theorem. 
There's a whole page of counterexamples on Wikipedia. I tried to tell her that, but she said it
was fake news. Also she called me a poopyhead." That stuff is NOT tolerated in industry, thank 
the merciful nerd gods. Let's just say that I have developed an allergy after repeated exposure.

It's not healthy to stake your entire future and self-worth on the success of one project. And 
it's much worse when the project is hard, when its ultimate failure may be due to factors
outside your control, and when you're wandering around with no concrete markers of progress. Even
patient, level-headed, and naturally optimistic people come out with scars.
```

Another reason is that academia rewards a very particular kind of research, and that there are outlets/avenues in industry that reward other kinds of research, including ones you wouldn't expect e.g. product design, per [Bryan Sim's answer](https://qr.ae/TW1uHs) to "What made you decide that academia is not for you?":

```markdown
For me, it was when I discovered what type of scientist I was.

In my opinion, there are two types of people who get into academia: People who care about what
they are studying, and people who care about how they study it.

At some point, I realized I was being pressured to become someone I didn’t want to be. I care 
about how we gain knowledge about the world. And over time, I found that I was happy doing research
on trivial things for fun, but that I didn’t enjoy “building houses” or “castles”, or whatever 
analogy was being used to denote one’s legacy of research. I especially didn’t enjoy the notion 
that I had to “defend” my line of research from evidence to the contrary (why can’t I/we just be
wrong?).

Today, I realize that I can be a scientist anywhere, as long as my job involves learning about some
aspect of reality the “right” way, with people I enjoy working with. This, if you think about it,
is the core of any good product design process: You work together with a team to figure out if your
hypothesis of what people want is true, and the results speak for themselves, whether in terms of 
user growth or $$$ growth.
```

Another is the huge incentive/pressure to hyperspecialize, with few exceptions (mostly involving being very smart), per [Colleen Farrelly's answer](https://qr.ae/TW1uHk) to same:

```markdown
When I was working on one of my three graduate research projects, a professor with whom I was
working congratulated me on a breakthrough and mentioned that I could make a career out of 
studying that method and helping other researchers apply it. The thought of studying one problem
basically to the exclusion of anything else was enough to make me literally run away. I was 
already sick of that project and not being able to move on to something new until everything was 
perfect and everyone liked the paper. I could never spend my whole life doing one thing. I 
couldn't spend a year doing one thing. Data science in industry allows me to dabble in all types 
of algorithms, advanced mathematics (like differential geometry, graph theory, algebraic
topology...), and work on a variety of projects at once.

This anecdote is but one of many reasons, and I've found a lot of academics end up pigeon-holed or
teaching classes they don't enjoy teaching, confined by grants when something interesting comes up.
Industry research is a lot faster and more varied, and I don't have to deal with 18-year-olds' 
parents arguing for better grades or graduate students cheating on exams and claiming "cultural 
differences" made them cheat...
```

<a name="#research-mindset"></a>
## Research mindset
([overview](#overview))

More by Carl Shulman from [the same document above](https://docs.google.com/document/d/1_yuuheVqp1quDfkuRcpoW_HO7jPaI7QnRjF1zl_VovU/edit), this time on research mindset:

```markdown
Don't dismiss ideas as unthinkable (rather than actions as subject to strong injunctions): things that
people are afraid of thinking about (because it might make them look bad, might imply bad news, is 
unpopular) have an elevated chance of offering low-hanging fruit for thinking.

Have a strong emotional revulsion to self-delusion and sloppy reasoning/research, including people 
Wrong on the Internet within communities you have some affiliation with.

Listen to yourself if something seems troubling, and try articulating, exploring, and steel-manning 
that intuition in multiple ways until it makes sense in a way that can be integrated with other knowledge 
(with whatever updates/revisions follow) or goes away. Don't just run roughshod over 'system 1' feelings.

Being comfortable with your own personality, emotions, and desires can help with being willing to do that 
kind of analysis, by making fewer conclusions unacceptable to you (empirical ones in particular).

Rigid ideological systems in a lot of tension with your real goals can be a problem there. E.g. in
Mormonism or utilitarianism or social justice, various empirical conclusions combine with the ideology
to recommend ruining your life, and people are strongly conditioned to avoid them. 

Recognizing partial, as opposed to impartial, motives (personal projects, selfishness, family, tribalism) 
and not trying to rationalize everything with a 100% impartial facade, can help more comfortably think
about questions like average well-being, or the real trade-off between burnout and effort, etc.
```

<a name="#anki-in-research"></a>
## Anki in research
([overview](#overview))

From Michael Nielsen's [Augmenting long-term memory](http://augmentingcognition.com/ltm.html), where he describes his experience reading the AlphaGo paper:

```markdown
I find Anki a great help when reading research papers, particularly in fields outside my expertise.
As an example of how this can work, I'll describe my experience reading a 2016 paper describing AlphaGo,
the computer system from Google DeepMind that beat some of the world's strongest players of the game Go.

After the match where AlphaGo beat Lee Sedol, one of the strongest human Go players in history, I 
suggested to Quanta Magazine that I write an article about the system. AlphaGo was a hot media topic at 
the time, and the most common angle in stories was human interest, viewing AlphaGo as part of a long-
standing human-versus-machine narrative, with a few technical details filled in, mostly as color.

I wanted to take a different angle. Through the 1990s and first decade of the 2000s, I believed human-or-
better general artificial intelligence was far, far away. The reason was that over that time researchers 
made only slow progress building systems to do intuitive pattern matching, of the kind that underlies
human sight and hearing, as well as in playing games such as Go. Despite enormous effort by AI researchers,
many pattern-matching feats which humans find effortless remained impossible for machines.

While we made only very slow progress on this set of problems for a long time, around 2011 progress began
to speed up, driven by advances in deep neural networks. For instance, machine vision systems rapidly went
from being terrible to being comparable to human beings for certain limited tasks. By the time AlphaGo was
released, it was no longer correct to say we had no idea how to build computer systems to do intuitive 
pattern matching. While we hadn't yet nailed the problem, we were making rapid progress. AlphaGo was a big
part of that story, and I wanted my article to explore this notion of building computer systems to capture 
human intuition.

While I was excited, writing such an article was going to be difficult. It was going to require a deeper
understanding of the technical details of AlphaGo than a typical journalistic article. Fortunately, I knew
a fair amount about neural networks – I'd written a book about them. But I knew nothing about the game of 
Go, or about many of the ideas used by AlphaGo, based on a field known as reinforcement learning. I was 
going to need to learn this material from scratch, and to write a good article I was going to need to really
understand the underlying technical material.

Here's how I went about it.

I began with the AlphaGo paper itself. I began reading it quickly, almost skimming. I wasn't looking for a 
comprehensive understanding. Rather, I was doing two things. One, I was trying to simply identify the most 
important ideas in the paper. What were the names of the key techniques I'd need to learn about? Second, 
there was a kind of hoovering process, looking for basic facts that I could understand easily, and that
would obviously benefit me. Things like basic terminology, the rules of Go, and so on.

Here's a few examples of the kind of question I entered into Anki at this stage: “What's the size of a Go
board?”; “Who plays first in Go?”; “How many human game positions did AlphaGo learn from?”; “Where did 
AlphaGo get its training data?”; “What were the names of the two main types of neural network AlphaGo used?”

As you can see, these are all elementary questions. They're the kind of thing that are very easily picked
up during an initial pass over the paper, with occasional digressions to search Google and Wikipedia, and
so on. Furthermore, while these facts were easy to pick up in isolation, they also seemed likely to be 
useful in building a deeper understanding of other material in the paper.

I made several rapid passes over the paper in this way, each time getting deeper and deeper. At this stage 
I wasn't trying to obtain anything like a complete understanding of AlphaGo. Rather, I was trying to build 
up my background understanding. At all times, if something wasn't easy to understand, I didn't worry about 
it, I just keep going. But as I made repeat passes, the range of things that were easy to understand grew 
and grew. I found myself adding questions about the types of features used as inputs to AlphaGo's neural 
networks, basic facts about the structure of the networks, and so on.

After five or six such passes over the paper, I went back and attempted a thorough read. This time the 
purpose was to understand AlphaGo in detail. By now I understood much of the background context, and it was
relatively easy to do a thorough read, certainly far easier than coming into the paper cold. Don't get me
wrong: it was still challenging. But it was far easier than it would have been otherwise.

After doing one thorough pass over the AlphaGo paper, I made a second thorough pass, in a similar vein. Yet 
more fell into place. By this time, I understood the AlphaGo system reasonably well. Many of the questions I
was putting into Anki were high level, sometimes on the verge of original research directions. I certainly 
understood AlphaGo well enough that I was confident I could write the sections of my article dealing with it.
(In practice, my article ranged over several systems, not just AlphaGo, and I had to learn about those as well,
using a similar process, though I didn't go as deep.) I continued to add questions as I wrote my article, 
ending up adding several hundred questions in total. But by this point the hardest work had been done.

Of course, instead of using Anki I could have taken conventional notes, using a similar process to build up an
understanding of the paper. But using Anki gave me confidence I would retain much of the understanding over the
long term. A year or so later DeepMind released papers describing followup systems, known as AlphaGo Zero and
AlphaZero. Despite the fact that I'd thought little about AlphaGo or reinforcement learning in the intervening
time, I found I could read those followup papers with ease. While I didn't attempt to understand those papers 
as thoroughly as the initial AlphaGo paper, I found I could get a pretty good understanding of the papers in less
than an hour. I'd retained much of my earlier understanding!

By contrast, had I used conventional note-taking in my original reading of the AlphaGo paper, my understanding
would have more rapidly evaporated, and it would have taken longer to read the later papers. And so using Anki
in this way gives confidence you will retain understanding over the long term. This confidence, in turn, makes
the initial act of understanding more pleasurable, since you believe you're learning something for the long haul,
not something you'll forget in a day or a week.

This entire process took a few days of my time, spread over a few weeks. That's a lot of work. However, the 
payoff was that I got a pretty good basic grounding in modern deep reinforcement learning. This is an immensely 
important field, of great use in robotics, and many researchers believe it will play an important role in
achieving general artificial intelligence. With a few days work I'd gone from knowing nothing about deep 
reinforcement learning to a durable understanding of a key paper in the field, a paper that made use of many 
techniques that were used across the entire field. Of course, I was still a long way from being an expert. There 
were many important details about AlphaGo I hadn't understood, and I would have had to do far more work to build
my own system in the area. But this foundational kind of understanding is a good basis on which to build deeper
expertise.
```

This quote is key -- it jives with my own experience trying to memorize random disconnected facts (along with other failure modes):

```markdown
It's notable that I was reading the AlphaGo paper in support of a creative project of my own, namely,
writing an article for Quanta Magazine. This is important: I find Anki works much better when used in 
service to some personal creative project.

It's tempting instead to use Anki to stockpile knowledge against some future day, to think “Oh, I should
learn about the geography of Africa, or learn about World War II, or […]”. These are goals which, for 
me, are intellectually appealing, but which I'm not emotionally invested in. I've tried this a bunch of 
times. It tends to generate cold and lifeless Anki questions, questions which I find hard to connect to 
upon later review, and where it's difficult to really, deeply internalize the answers. The problem is 
somehow in that initial idea I “should” learn about these things: intellectually, it seems like a good 
idea, but I've little emotional commitment.

By contrast, when I'm reading in support of some creative project, I ask much better Anki questions. I 
find it easier to connect to the questions and answers emotionally. I simply care more about them, and 
that makes a difference. So while it's tempting to use Anki cards to study in preparation for some 
(possibly hypothetical) future use, it's better to find a way to use Anki as part of some creative project.
```

But what about shallow reads of papers? Does Anki-based reading help? Yes, says Nielsen:

```markdown
Most of my Anki-based reading is much shallower than my read of the AlphaGo paper. Rather than spending 
days on a paper, I'll typically spend 10 to 60 minutes, sometimes longer for very good papers. Here's a 
few notes on some patterns I've found useful in shallow reading.

As mentioned above, I'm usually doing such reading as part of the background research for some project.
I will find a new article (or set of articles), and typically spend a few minutes assessing it. Does the
article seem likely to contain substantial insight or provocation relevant to my project – new questions,
new ideas, new methods, new results? If so, I'll have a read.

This doesn't mean reading every word in the paper. Rather, I'll add to Anki questions about the core
claims, core questions, and core ideas of the paper. It's particularly helpful to extract Anki questions
from the abstract, introduction, conclusion, figures, and figure captions. Typically I will extract anywhere
from 5 to 20 Anki questions from the paper. It's usually a bad idea to extract fewer than 5 questions – 
doing so tends to leave the paper as a kind of isolated orphan in my memory. Later I find it difficult to 
feel much connection to those questions. Put another way: if a paper is so uninteresting that it's not 
possible to add 5 good questions about it, it's usually better to add no questions at all. ...

Really good resources are worth investing time in. But most papers don't fit this pattern, and you quickly 
saturate. If you feel you could easily find something more rewarding to read, switch over. It's worth 
deliberately practicing such switches, to avoid building a counter-productive habit of completionism in your
reading. It's nearly always possible to read deeper into a paper, but that doesn't mean you can't easily be 
getting more value elsewhere. It's a failure mode to spend too long reading unimportant papers.
```

Nielsen says you can also do 'syntopic' reading of entire subfields' research literature,thereby allowing mortals you and me to become Luke Muehlhauser:

```markdown
There's also a sense in which it's possible to use Anki not just to read papers, but to “read” the entire
research literature of some field or subfield. Here's how to do it.

You might suppose the foundation would be a shallow read of a large number of papers. In fact, to really
grok an unfamiliar field, you need to engage deeply with key papers – papers like the AlphaGo paper. What
you get from deep engagement with important papers is more significant than any single fact or technique:
you get a sense for what a powerful result in the field looks like. It helps you imbibe the healthiest norms
and standards of the field. It helps you internalize how to ask good questions in the field, and how to put
techniques together. You begin to understand what made something like AlphaGo a breakthrough – and also its 
limitations, and the sense in which it was really a natural evolution of the field. Such things aren't 
captured individually by any single Anki question. But they begin to be captured collectively by the questions
one asks when engaged deeply enough with key papers.

So, to get a picture of an entire field, I usually begin with a truly important paper, ideally a paper 
establishing a result that got me interested in the field in the first place. I do a thorough read of that 
paper, along the lines of what I described for AlphaGo. Later, I do thorough reads of other key papers in
the field – ideally, I read the best 5-10 papers in the field. But, interspersed, I also do shallower reads
of a much larger number of less important (though still good) papers. In my experimentation so far that
means tens of papers, though I expect in some fields I will eventually read hundreds or even thousands of
papers in this way.

You may wonder why I don't just focus on only the most important papers. Part of the reason is mundane: it
can be hard to tell what the most important papers are. Shallow reads of many papers can help you figure out
what the key papers are, without spending too much time doing deeper reads of papers that turn out not to be
so important. But there's also a culture that one imbibes reading the bread-and-butter papers of a field: a
sense for what routine progress looks like, for the praxis of the field. That's valuable too, especially for 
building up an overall picture of where the field is at, and to stimulate questions on my own part. Indeed, 
while I don't recommend spending a large fraction of your time reading bad papers, it's certainly possible to
have a good conversation with a bad paper. Stimulus is found in unexpected places.

Over time, this is a form of what Mortimer Adler and Charles van Doren dubbed *syntopic reading*. I build up
an understanding of an entire literature: what's been done, what's not yet been done. Of course, it's not 
literally reading an entire literature. But functionally it's close. I start to identify open problems, 
questions that I'd personally like answered, but which don't yet seem to have been answered. I identify tricks,
observations that seem pregnant with possibility, but whose import I don't yet know. And, sometimes, I 
identify what seem to me to be field-wide blind spots. I add questions about all these to Anki as well. In 
this way, Anki is a medium supporting my creative research. It has some shortcomings as such a medium, since
it's not designed with supporting creative work in mind – it's not, for instance, equipped for lengthy, 
free-form exploration inside a scratch space. But even without being designed in such a way, it's helpful as
a creative support.
```

<a name="#research-tactics"></a>
## Research tactics
([overview](#overview))

Scott Aaronson, in response to Luke Muehlhauser's interview question "what are some object-level research tactics you use (more specific than your general “bait and switch” strategy)?" in the [MIRI Conversations series](https://intelligence.org/2013/12/13/aaronson/):

```markdown
(1) Any time you find yourself in a philosophical disagreement with a fellow scientist, don’t be 
content just to argue philosophically — even if you’re sure you can win the argument! Instead, think
hard about whether you can go further, and find a concrete technical question that captures some 
little piece of what you’re disagreeing about. Then see if you can answer that technical question.
Of course, any time you do this, you have to be prepared for the possibility that the answer will go 
your opponent’s way, rather than yours! But what’s nice is that you get to publish a paper even then.
(One of the best ways to tell whether a given enterprise is scientific at all, rather than ideological,
is by asking whether the participants will opportunistically “go to bat for the opposing side” whenever
they find a novel truth on that side.) I’d estimate that up to half the papers I’ve written had their 
origin in my reading or overhearing some claim — for example, “Grover’s algorithm obviously can’t work
for searching actual physical databases, since the speed of light is finite,” or “the quantum states 
arising in Shor’s algorithm are obviously completely different from anything anyone has ever seen in the
lab,” or “the interactive proof results obviously make oracle separations completely irrelevant” — and 
getting annoyed, either because I thought the claim was false, or because I simply didn’t think it had
been adequately justified. The cases where my annoyance paid off are precisely the ones where, rather 
than just getting mad, I managed to get technical!

(2) Often, the key to research is figuring out how to redefine failure as success. Some stories: when Alan
Turing published his epochal 1936 paper on Turing machines, he did so with great disappointment: he 
had recently learned that Alonzo Church had independently arrived at similar results using lambda 
calculus, and he didn’t know whether anyone would still be interested in his alternative, machine-based
approach. In the early 1970s, Leonid Levin delayed publishing about NP-completeness for several years:
apparently, his “real” goal was to prove graph isomorphism was NP-complete (something we now know is 
almost certainly false), and in his mind, he had failed. Instead, he merely had a few “trivialities,” 
like the definitions of P, NP, and NP-completeness, and the proof that satisfiability was NP-complete. 
And Levin’s experience is far from unique: again and again in mathematical research, you’ll find yourself
saying something like: “goddammit, I’ve been trying for six months to prove Y, but I can only prove the
different/weaker statement X! And every time I think I can bridge the gap between X and Y, yet another 
difficulty rears its head!” Any time that happens to you, think hard about whether you can write a 
compelling paper that begins: “Y has been a longstanding open problem. In this work, we introduce a new 
idea: to make progress on Y by shifting attention to the more tractable X.” More broadly, experience has 
shown that scientists are terrible judges of which of their ideas will be interesting or important to 
others. Pick any scientist’s most cited paper, and there’s an excellent chance that the scientist herself,
at one point, considered it a “little recreational throwaway project” that was barely worth writing up. 
After you’ve seen enough examples of that, you learn you should always err on the side of publishing, and 
let posterity sort out which of your ideas are most important. (Yet another advantage of this approach is
that, the more ideas you publish, the less emotionally invested you are in any one of them, so the less
crushed you are when a few turn out to be wrong or trivial or already known.)

(3) Sometimes, when you set out to prove some mathematical conjecture, your first instinct is just to throw
an arsenal of theory at it. “Hey, what if I try a topological fixed-point theorem? What if I translate the
problem into a group-theoretic language? If neither of those works, what if I try both at once?” Sometimes, 
you rise so quickly this way into a stratosphere of generality that the original problem is barely a speck on
the ground. And yes, some problems can be beaten into submission using high-powered theory. But in my 
experience, there are two enormous risks with this approach. First, you’re liable to get lost on a wild
goose chase, where you get so immersed in theory and techniques that you lose sight of your original goal. 
It’s as if your efforts to break into a computer network lead you to certain complicated questions about 
the filesystem, which in turn lead you to yet more complicated questions about the kernel… and in the 
meantime someone else breaks in by guessing people’s birthdays for their passwords. Second, you’re also
liable to fool yourself this way into thinking you’ve solved the problem when you haven’t. When you let 
high-powered machinery take the place of hands-on engagement with the problem, a single mistake in applying 
the machinery can creep in unbelievably easily. These risks are why I’ve learned over time to work in an 
extremely different way. Rather than looking for “general frameworks,” I look for easy special cases and
simple sanity checks, for stuff I can try out using high-school algebra or maybe a five-line computer program, 
just to get a feel for the problem. Even more important, when I’m getting started, I don’t think about proof
techniques at all: I think instead about obstructions. That is, I ask myself, “what would the world have to 
be like for the conjecture to be false? what goes wrong if I try to invent a simple counterexample? does 
anything go wrong? it does? OK then, what obstruction keeps me from proving this conjecture in the simplest,
dumbest way imaginable?” I find that, after you’ve felt out the full space of obstructions and
counterexamples, and really honestly convinced yourself of why the conjecture should be true, finding the 
proof techniques by which to convince everyone else is often a more-or-less routine exercise.

Finally, you ask about tactics that I suspect might be helpful, but that I haven’t used much myself. One that
springs to mind is to really master a tool like Mathematica, MATLAB, Maple, or Magma — that is, to learn it 
so well that I can code as fast as I think, and just let it take over all the routine / calculational /
example-checking parts of my work. As it is, I use pretty much the same antiquated tools that I learned as
an adolescent, and I rely on students whenever there’s a need for better tools. A large part of the problem
is that, as a “tenured old geezer,” I no longer have the time or patience to learn new tools just for the 
sake of learning them: I’m always itching just to solve the problem at hand with whatever tools I know. (The
same issue has kept me from learning new mathematical tools, like representation theory, even when I can
clearly see that they’d benefit me.)
```

Luke himself:

```markdown
1. When you’re confused about a fuzzy, slippery concept, try to build a simple formal model and push on it 
with the new tools then available to you. Even if the model doesn’t capture the complexity of the world,
pushing things into the mathematical realm can lead to progress. E.g. the VNM axioms don’t exactly capture
“rationality,” but it sure is easier to think clearly about rationality once you have them. Or: we’re 
confused about how to do principled reflective reasoning within an agent, so even though advanced AIs 
are unlikely to literally run into a “Löbian obstacle” to self-reflection, setting up the problem that 
way (in mathematical logic) can lead to some interesting insights in (e.g.) probabilistic metamathematics
for reflective reasoning.

2. Look for tools from other fields that appear to directly map onto the phenomena you’re studying. E.g. model
moral judgment as an error process amenable to Bayesian curve fitting.

3. Try to think of how your concept could be instantiated with infinite computing power. If you can’t do that,
your concept might be fundamentally confused.

4. If you’re pretty familiar with modern psychology, then… When using your intuitions to judge between options,
try to think about which cognitive algorithms could be generating those intuitions, and whether they are
cognitive algorithms whose outputs you reflectively endorse.

5. To make the thing you’re studying clearer, look just next to it, and around it. Foer (2009) explains this
nicely in the context of thinking about one’s values and vegetarianism: “A simple trick from the backyard
astronomer: if you are having trouble seeing something, look slightly away from it. The most light-sensitive 
parts of our eyes (those we need to see dim objects) are on the edges of the region we normally use for 
focusing. Eating animals has an invisible quality. Thinking about dogs, and their relationship to the animals 
we eat, is one way of looking askance and making something invisible visible.
```

Carl Shulman's [research advice](https://docs.google.com/document/d/1_yuuheVqp1quDfkuRcpoW_HO7jPaI7QnRjF1zl_VovU/edit) Google doc is great stuff. Here's some stuff I liked. 

Thinking habits:

```markdown
Frequently imagine what someone you respect, thinking you were wrong, would say/try to make the 
best argument against what you are currently thinking.

Pay attention to the use of contradictory epistemic standards and premises on different arguments/pattern
recognize them. Reconcile them or adjust your confidence in them.

I have gotten a fair amount out of trying to understand the epistemology and basic worldview of multiple
movements. I like ideological turing tests, mainly because they will highlight the best evidence for the
things they like, and against the things they hate, which helps in identifying areas to look into.

Make a habit of checking factual claims that you hear with a short Google search, and/or Wikipedia.

Use basic arithmetic and statistics frequently and briefly as part of thinking rather than as occasional
or separate exercises.

Try to convert qualitative claims into quantitative Fermi estimates whenever possible. Fermi calculations
with quick Wikipedia/Google/Wolfram/standard sources go far, and one can get into the habit and see how 
they typically evolve with different levels of depth.
```

Research management:

```markdown
Make a bookmarks folder to note critical arguments against positions you hold, and read it, so you don't
get isolated from different views.

Write casual thoughts up in explicit emails or blog posts to get feedback from people.

Have a giant folder of hundreds of blog post drafts to throw interesting ideas, citations, and links to.
I may not have published anything about X, but I have a draft in my blogging folder where I have stored 
assorted information about it.

Write down your views and check against your old views to see when you were wrong and when you were right.

Offer and accept bets about observables or change your predictions.
```

Information exposure:

```markdown
Reading broadly using multiple separate quality filters, that are independent, at least partially so, to
escape systematic biases of one or the other. For example, use multiple good link aggregation sites with
different authors and biases.

Look up expert opinion data (favoring subject expertise, science, IQ, incentives, track records), with an 
emphasis on trends as one looks at more elite groups (one has to go famous scientists to find really low 
belief in religion and psychic powers, so I try to predict what a better expert class would believe when 
there is a consistent trend).

Try to get datasets (Wikipedia lists, World Bank info, USDA, etc.) as a primary step in thinking about a 
question.

Use Google Scholar, and especially the ability to search for papers citing influential papers in a field.
```

Process for research project:

```markdown
You can quickly generate ideas by explaining to a questioner (GW style conversation notes, online 
conversations.)

I also like making hopefully-comprehensive taxonomies that one can work through in full to avoid selection
biases, e.g. looking through all the sectors of the economy, or all the major categories of philanthropy,
or all the major academic fields or think tanks. These are tools for hypothesis generation, and hitting 
on low-hanging fruit knowledge sources.

Thinking about end-goals and back-chaining to see things that would be relevant, rather than just using 
vague correlational criteria.

Look for high order bits, the biggest effects, as first priority, then incrementally add lower order 
refinements in accord with value of information.

Don't be too easily satisfied with cluster thinking.
```

<a name="#why-academic-writing-sucks"></a>
## Why academic writing sucks
([overview](#overview))

My favorite academic(ish) writers — like Baez for math, Aaronson for CS, Simler for postrationality, Nerst for erisology — are all guided by the spirit of *“hey, there’s something exciting I wanna show you!”*. Their words *get out of the way*, and you see the distilled essence of the thing that’s taken their breath away, and has now snatched yours too. It’s a tremendously heady experience. A longstanding dream of mine is to write a piece that captures that same spirit in explaining a difficult idea.

From Steven Pinker's essay [Why academics stink at writing](https://stevenpinker.com/files/pinker/files/why_academics_stink_at_writing.pdf), which you should read in its entirety for the beautifully clear writing and guffaw-inducing anecdotes. 

Pinker says these answers are wrong, or at least incommensurate with his own experience:

```markdown
(1) The most popular answer outside the academy is the cynical one:
Bad writing is a deliberate choice. Scholars in the softer fields
spout obscure verbiage to hide the fact that they have nothing to
say. They dress up the trivial and obvious with the trappings of
scientific sophistication, hoping to bamboozle their audiences
with highfalutin gobbledygook.

Though no doubt the bamboozlement theory applies to some
academics some of the time, in my experience it does not ring true.
I know many scholars who have nothing to hide and no need to
impress. They do groundbreaking work on important subjects,
reason well about clear ideas, and are honest, down-to-earth
people. Still, their writing stinks.

(2) The most popular answer inside the academy is the self-serving
one: Difficult writing is unavoidable because of the abstractness
and complexity of our subject matter. Every human pastime—
music, cooking, sports, art—develops an argot to spare its
enthusiasts from having to use a long-winded description every
time they refer to a familiar concept in one another’s company. It
would be tedious for a biologist to spell out the meaning of the
term transcription factor every time she used it, and so we should
not expect the tête-à-tête among professionals to be easily
understood by amateurs.

But the insider-shorthand theory, too, doesn’t fit my experience. I
suffer the daily experience of being baffled by articles in my field,
my subfield, even my sub-sub-subfield. The methods section of an
experimental paper explains, "Participants read assertions whose
veracity was either affirmed or denied by the subsequent
presentation of an assessment word." After some detective work, I
determined that it meant, "Participants read sentences, each
followed by the word true or false." The original academese was
not as concise, accurate, or scientific as the plain English
translation. So why did my colleague feel compelled to pile up the
polysyllables?

(3) A third explanation shifts the blame to entrenched authority.
People often tell me that academics have no choice but to write
badly because the gatekeepers of journals and university presses
insist on ponderous language as proof of one’s seriousness. This
has not been my experience, and it turns out to be a myth. In 
Stylish Academic Writing (Harvard University Press, 2012), Helen
Sword masochistically analyzed the literary style in a sample of 500
scholarly articles and found that a healthy minority in every field
were written with grace and verve. 
```

So if bamboozlement, insider-shorthand and journal gatekeeping are wrong, what's really at fault? Pinker’s answer is two-pronged: the self-conscious style, and the curse of knowledge. The latter I’ve covered in previous posts, so the summary below concentrates on the former. 

First, Thomas and Turner on how to understand writing styles:

```markdown
Every style of writing, quoting Francis-Noel Thomas and Mark Turner’s book *Clear and Simple 
as the Truth*, can be understood as “a model of the communication scenario that an author 
simulates in lieu of the real-time give-and-take of a conversation”. They distinguish five 
styles, depending on how the writer imagines themselves to be related to the reader, and what
the writer is trying to accomplish:

1. romantic
2. oracular
3. prophetic
4. plain
5. practical

A particular style they single out as an aspiration for writers of expository prose is the 
*classic style*, its invention credited to 17th-century French essayists such as Descartes 
and La Rochefoucauld.
```

The guiding metaphor of classical style is “seeing the world”:

```markdown
The writer can see something that the reader has not yet noticed, and he orients the reader 
so she can see for herself. The purpose of writing is presentation, and its motive is disinterested
truth. It succeeds when it aligns language with truth, the proof of success being clarity and 
simplicity. The truth can be known and is not the same as the language that reveals it; prose 
is a window onto the world. The writer knows the truth before putting it into words; he is not
using the occasion of writing to sort out what he thinks. The writer and the reader are equals:
The reader can recognize the truth when she sees it, as long as she is given an unobstructed view.
And the process of directing the reader’s gaze takes the form of a conversation.
```

See also [The art of plain talk](#the-art-of-plain-talk).

Most academic writing is the opposite of classic style. It’s a blend of two styles: *practical* and *self-conscious* (or ironic, postmodern, relativistic).

Practical style:

```markdown
…the writer’s goal is to satisfy a reader’s need for a particular kind of information, and the form
of the communication falls into a fixed template, such as the fiveparagraph student essay or the 
standardized structure of a scientific article.
```

Self-conscious style:

```markdown
…the writer’s chief, if unstated, concern is to escape being convicted of philosophical naïveté 
about his own enterprise.

It’s easy to see why academics fall into self-conscious style. Their goal is not so much 
communication as self-presentation—an overriding defensiveness against any impression that they
may be slacker than their peers in hewing to the norms of the guild.
```

Pinker says that many of the hallmarks of “academese” are symptoms of the self-conscious style. Here's my abridged version of his explanation:

```markdown
1. Meta-discourse: verbiage about verbiage. Paraphrasing Pinker: “Thoughtless writers think 
they’re doing the reader a favor by guiding her through the text with stuff like previews, 
summaries, and signposts. Actually it helps the writer more than the reader: the reader has
to put more work into understanding the signposts than she saves in seeing what they point to,
like directions for a shortcut that take longer to figure out than the time the shortcut would
save. The art of classic prose is to use signposts sparingly, as we do in conversation… Instead 
of dry metadata: pose a question, co-opt the guiding metaphor behind classic style (vision — 
“as we have seen”), use we.”

2. Professional narcissism: Pinker: “Academics live in two universes: the world of the thing they
stud, and the world of their profession. Most of a researcher’s waking hours are spent in the 
second world, and it’s easy for him to confuse the two. The result is the typical opening of an
academic paper: ‘In recent years, an increasing number of psychologists and linguists have turned
their attention to the problem of child language acquisition…’ No offense, but few people are 
interested in how professors spend their time. Classic style ignores the hired help and looks 
directly at what they are being paid to study: ‘All children acquire the ability to speak a language
without explicit lessons. How do they accomplish this feat?’”

3. Apologizing: Pinker: “Self-conscious writers are also apt to kvetch about how what they’re about
to do is so terribly difficult and complicated and controversial. In the classic style, the writer
credits the reader with enough intelligence to realize that many concepts aren’t easy to define, 
and that many controversies aren’t easy to resolve. She is there to see what the writer will do 
about it.”

4. Shudder quotes: Pinker: “Academics often use quotation marks to distance themselves from a common
idiom, as in "She is a ‘quick study’ and has been able to educate herself in virtually any area that
interests her." They seem to be saying, "I couldn’t think of a more dignified way of putting this, 
but please don’t think I’m a flibbertigibbet who talks this way; I really am a serious scholar." The
problem goes beyond the nose-holding disdain for idiomatic English: it confuses the reader by 
introducing ambiguity. Quotation marks have a number of legitimate uses — squeamishness about one’s 
own choice of words is not among them.”

5. Hedging: Pinker: “Academics mindlessly cushion their prose with wads of fluff that imply they are
not willing to stand behind what they say, like “apparently” etc. The worst is “I would argue”. 
Writers use hedges in the vain hope that it will get them off the hook, or at least allow them to
plead guilty to a lesser charge, should a critic ever try to prove them wrong. A classic writer, in
contrast, counts on the common sense and ordinary charity of his readers, just as in everyday 
conversation we know when a speaker means in general or all else being equal — any adversary who is 
intellectually unscrupulous enough to give the least charitable reading to an unhedged statement will
find an opening to attack the writer in a thicket of hedged ones anyway. Also instead of hedging, 
qualify the statement — spell out the circumstances in which it does not hold rather than leaving
himself an escape hatch or being coy as to whether he really means it. It’s not that good writers 
never hedge their claims. It’s that their hedging is a choice, not a tic.”

6. Metaconcepts and nominalizations: concepts about concepts, vacuous words that don’t add content.
Pinker: “It’s easy to see why metaconcepts tumble so easily from the fingers of academics. Professors 
really do think about "issues" (they can list them on a page), "levels of analysis" (they can argue 
about which is most appropriate), and "contexts" (they can use them to figure out why something works
in one place but not in another). But after a while those abstractions become containers in which 
they store and handle all their ideas, and before they know it they can no longer call anything by 
its name. "Reducing prejudice" becomes a "prejudice-reduction model"… English grammar is an enabler
of the bad habit of writing in unnecessary abstractions because it includes a dangerous tool for 
creating abstract terms. A process called nominalization takes a perfectly spry verb and embalms it
into a lifeless noun by adding a suffix like –ance, –ment, or –ation. Instead of affirming an idea,
you effect its affirmation…
```

Pinker argues that the theory that “academese is the opposite of classic style” explains the following paradox of academic writing:

```markdown
Many of the most stylish writers who cross over to a general audience are scientists (together with
some philosophers who are fans of science), while the perennial winners of the Bad Writing Contest 
are professors of English. That’s because the ideal of classic prose is congenial to the worldview
of the scientist. Contrary to the common misunderstanding in which Einstein proved that everything
is relative and Heisenberg proved that observers always affect what they observe, most scientists 
believe that there are objective truths about the world, and that they can be discovered by a 
disinterested observer.

By the same token, this guiding image of classic prose could not be farther from the worldview of 
relativist academic ideologies such as postmodernism, poststructuralism, and literary Marxism, which
took over many humanities departments in the 1970s. Many of the winning entries in the Dutton contest
(such as Judith Butler’s "The move from a structuralist account in which capital is understood to
structure social relations in relatively homologous ways to a view of hegemony in which power relations
are subject to repetition, convergence, and rearticulation brought the question of temporality into the 
thinking of structure ….") consist almost entirely of metaconcepts.
```

See also [why math writing sucks](https://github.com/monastri/monastri.github.io/blob/master/notes-math-physics.md#why-math-is-boring).

<a name="#research-in-industry"></a>
## Research in industry
([overview](#overview))

Simon DeDeo is a professor at the Santa Fe Institute, that interdisciplinary haven of complexity science that Cosma Shalizi is affiliated with. Here’s a tweetstorm by Simon on science in large corporate organizations like Google / Facebook, which runs counter to my previous impression (I’d like to see a contrary perspective actually), which I’m crossposting here for ease of personal reference:

```markdown
I grew up in the Bayesian era—I watched @DavidSpergel and his band of merry scientists change
our view of the world with a few simple, theoretically-motivated equations.

That's what I brought to the table when I went out to study living and thinking systems. 
Around 2010, of course, the deep learning revolution became impossible to ignore.

It was exciting stuff. We'd have people visit the Institute and tell us about decision trees, 
random forests,—all sorts of wonderful things. I tried to get a handle on it but (honestly) 
there was so much we could do with simple tools that it was never a priority.

When I got to IU, I was hired as a prof in the informatics department, @IUSoICE (informatics==the
future of CS—i.e., forget quicksort, let's work out what these machines are doing to human life).
I was on a hiring committee, and we were keen to get a deep learning hire.

I took all the candidates out to breakfast (I was a naughty hire, and skipped meetings and
committees to spend my time with research students and undergrads, this was the one gap I had).

I tried to work out what deep learning was about. Most of the candidates were too sleep deprived 
to dissemble. Basic answer: every sexy project we do—flying quadcopters, getting another 0.1% on 
the MNIST—is basically one graduate student.

You work out the topology of the neural net. Then you find the weights. How? The answer: "graduate
student descent", a little pun to giggle over floppy croissants at the student cafe—in short, 
there's no good answer, a human being sits there and twiddles things about.

Machine learning is an amazing accomplishment of engineering. But it's not science. Not even close.
It's just 1990, scaled up. It has given us literally no more insight than we had twenty years ago.

"Deep learning implements the renormalization group!" Yeah, I heard that too. If you have a system 
where information is organized spatially, is it really a surprise that the neurons group information
together spatially?

I'd get invited to meetings at Google Research, or wherever. They had security like crazy—worse than 
a hedge fund. A security guard would follow you to the bathroom.

Each scientist at my "grade"—i.e., the equivalent of a junior faculty member, someone who should be
out on the edge of knowledge—was, instead, managing a team of ten people doing graduate student 
descent.

Google can beat University of Kansas for the sole reason that they can hire ten times more graduate
students per researcher. The difference, of course, is that a graduate student at UK has the chance
to do something intellectually significant. Not true at GR.

They had no idea what they were doing. They had the manpower (word chosen advisedly) to apply deep 
learning to anything, simulating the Schrodinger equation, drug design, anything. Their main goal
was to find the scientific field they could have the maximum impact on.

I've visited probably fifty Universities. I love it. Everywhere I go, I get new ideas. It's one of
the best features of my job. There's one exception: commercial "research" labs.

If you want to build machines that monitor people and sell them more ads faster, go for it. If you
want to find problem where you can take a working-class job, model the man or woman who does it, and
build a net to put them out of a job without compensation, be my guest.

Have we done science with something Google Research has built? Absolutely. We have a great paper 
coming out where we use word2vec to help build a theory of puzzle solving.

But we could have built a system of equal utility ourselves. There's zero intellectual contribution
there. I'm not joking, and I'll go head-to-head with anyone who says I am.

I got a nice cold-call from a top-flight Masters' student in CS, as I do sometimes (please keep them
coming, I can pay). I flew him out and we started working on a problem in the emergence of social 
cooperation. He wanted to do DL.

Two weeks in we were a step beyond what Google Brain was doing. I don't mean technically—they had 
amazing YouTube videos of sprites in a landscape. I do mean intellectually. Their demos were like 
2018 meets something out of the 1980s.

They said they did social science, but it was nothing of the sort. It was homo economicus spread out
over 50 GPUs. At best, a devastating proof-by-example of need for academia. Buy a copy of Bowles and
Ginits, Cooperative Species, and you'll learn more than they did, in a week.

Can you do cool research at Google Brain? Honest answer: no. You will be on the cutting edge of 
machine learning, yes—an engineering discipline whose basic goals are set by large corporations.
But you will not be a scientist.

I get that you may need to make money. You can make a lot there, and all the jobs at Renaissance
Technology are taken. Go for it—you have all my respect. Academia sucks.

But if you want, at some point in your flourishing career, with your mind and your soul, to join
the two-thousand year old parade of intellectual progress, you are not going to do it at Google.
Certainly not at Facebook.

If you want to do that, I have a suggestion. It's not the only path, by any means, and I've had 
amazing fellow-travellers who haven't. But here it is.

Go to graduate school. Do a PhD. With us, here at CMU/SDS, if you like—but we're not the only place
that does computational social or cognitive science. You won't get paid much, but you will mentors
who legitimately care about the development of your mind.

It's difficult to overestimate the difference between a good PhD program and industry. It is 
literally shameful, if you're a good PhD advisor, to interfere with the intellectual development
of a student. At Google, it's a business plan.

None of this is a joke. This is ten years of experience. Graduate school applications are coming 
up in the Fall. Think about it. Make sure you're getting a good deal (you shouldn't go into debt
for a PhD, and you should get healthcare).

In short: corporate "research" is a business proposition. Whatever true intellectual progress 
comes out of there happens in spite of management. Given how good these companies are at monitoring
their employees, that gap is now miniscule.

Last anecdote, then I'm done. We visited Google Research, arranged by a contact. The people were
unbelievably smart. We brainstormed all sorts of wonderful things to work on. The last day of the
meeting, the academics were like, OK! Let's go to the pub! Let's hash this out!

Their response: this was vacation for us. We're behind on our real work. We have to work this 
weekend. (Not "we feel guilty", but "we have to".) For the academics in the room, this was work.
Suddenly, I realized that this was vacation for them.
```

This happened to generate lots of heated discussion on [the ML subreddit](https://www.reddit.com/r/MachineLearning/comments/8yvlzy/d_debate_about_science_at_organizations_like/). Example counterargument from harharveryfunny:

```markdown
It's a bit of a straw man attack to complain that Google Brain (an engineering division) isn't doing
research, while ignoring Google DeepMind - their research division!

The argument that industry is all about money also ignores the grand history of corporate research
labs such as Bell Labs (thanks for the transistor!), Watson Labs, Xerox Parc (you could hardly
complain about them being too commercial!). I don't see any reason to suppose that Google, FaceBook
or Microsoft's research divisions are any less pure.
```

kendallpark:

```markdown
I've worn both the "industry" and "researcher" hat. In my particular field (ML + medicine) research,
we've had a solid 3+ decade parade of "intellectual progress" in the form of academic papers about ML 
+ medicine. You know how many of these promising ideas have made it into the clinic? Pretty much none.
Why? Well, there are a lot of reasons. But one of the big ones is PRODUCT.

Academic researchers often don't want to deal with nuts and bolts of actual implementation of their
project into a real system. Academic researchers often lack the software development know-how to 
implement their project into a real system. (Or at least, this has definitely been what I've witnessed
during graduate study.)

And you know what? It's totally fine to be a non-translational ML + medicine researcher. Maybe 
productization isn't their thing. I appreciate the papers; they should keep trying new things and
writing about their results.

But at the same I see way too many ML + medicine researchers patting themselves on the back for 'making 
a difference' in medicine when all they're doing is adding another paper to the mountain of "great ideas 
that could save patient lives but never will because no one will implement them."

I understand that this is not the situation all ML + [some other field] fall into, perhaps not at all for
pure ML, but this has been my experience in ML + medicine. We have more than enough research. We need more
product.

For the record: this is my own opinion and not that of any of my current or previous institutions/employers.
```

<a name="#role-of-intellectual-traditions"></a>
## Role of intellectual traditions
([overview](#overview))

From Cosma Shalizi's [review](http://bactra.org/reviews/error/) of Deborah Mayo's book *Error and the Growth of Experimental Knowledge*:

```markdown
Then, too, there is the interesting, and I think absolutely correct, view of the purpose and utility
of a theory of experiment: "It changes fortuitous events, which may take weeks or may take many decennia,
into an operation governed by intelligence, which will be finished within a month" (7.78, quoted p. 434).

This is of a piece with the general function of intellectual traditions. Genius can, perhaps, get by on
its wits, make things up from scratch, etc. Intellect serves the rest of us, by codifying, by setting up
standards and procedures which can be followed with only (as a friend once happily put it) "a mediocum of
intelligence," so that what might have taken genius can be (at least partially) achieved through the
application of rules. Among those rules, "normal tests" or "standard tests" --- tests which have proved to
be reliable detectors of specific errors --- take a special place. Traditions of inquiry which incorporate
and use a family of normal tests may fail to produce reliable knowledge, but those which don't can hardly
hope even to produce interesting mistakes.
```

<a name="#Productivity"></a>
## Productivity
([overview](#overview)) 

<a name="#Resize-value-batches"></a>
### Resize value batches
([overview](#overview))

This complements [batching low-intensity tasks](#Batch-low-intensity-tasks). All this from productivity guru Tiago Forte's [Bending the curves of productivity](https://evernote.com/blog/bending-the-curves-of-productivity/). 

Time (which costs money) passes at the same pace:

![time](https://s24953.pcdn.co/blog/wp-content/uploads/2018/01/1_Bending_Productivity_graphs.001-e1484172491340.jpeg)

Flow is preceded by struggle:

![flow](https://s24953.pcdn.co/blog/wp-content/uploads/2018/01/1_Bending_Productivity_graphs.002-e1484172319804.jpeg)

Energy level drops. Too low and you can't hop onto the flow plateau:

![energy](https://s24953.pcdn.co/blog/wp-content/uploads/2018/01/1_Bending_Productivity_graphs.004-e1484172389812.jpeg)

Value (in a single working session) is created towards the end -- e.g. one minute before you send that preprint for peer review, no value has been created:

![value](https://s24953.pcdn.co/blog/wp-content/uploads/2018/01/1_Bending_Productivity_graphs.005-e1484172400609.jpeg)

Tiago claims that "every school of productivity thought can be defined in terms of which curve it attempts to bend, and how":

```markdown
The “Energy School” offers a variety of ways to get that energy curve higher. Better
diet, more or different exercises, stretching and yoga, better sleep. If you can just
keep your energy level high enough, their argument goes, your productivity will be 
great.

The “Focus School” is all about getting into and staying in flow. Meditation, goal-
setting exercises, prioritizing schemes, avoiding distractions, no-meeting or no-phone
days, accountability mechanisms, noise-canceling headphones, and many others. They argue
that the best strategy is to pick a task and then hammer away at it until it’s finished,
extending that flow curve as long as possible.

The “Efficiency School” is obsessed with the logistics of work. It advocates using 
technology or other people to automate tasks, learning keyboard shortcuts, improving 
reading and writing speed, ruthlessly cutting out all unnecessary activities, moving to
Bali to cut down expenses, and other methods of cramming more productivity into the given
amount of time and money represented by the time/money curve.
```

So far, so neat. I like systematizing models like that. 

This is what happens when work gets interrupted constantly -- all struggle, no flow, and the impression that nothing got done despite a full day of work:

![interrupt](https://s24953.pcdn.co/blog/wp-content/uploads/2018/01/1_Bending_Productivity_graphs.008-e1484172446152.jpeg)

Tiago says "don't fight the interruptions, change the value curve shape/size to fit":

![value change](https://s24953.pcdn.co/blog/wp-content/uploads/2018/01/1_Bending_Productivity_graphs.009-e1484172478278.jpeg)

This is standard in manufacturing/software/startups:

```markdown
This idea, of course, isn’t new. In the world of manufacturing, it is the equivalent
of small batch sizes, a key part of the Just-In-Time vision that has propelled Toyota
through 7 decades of growth to become the world’s largest automaker. 

In the world of software, it is known as continuous integration and deployment, a 
practice that has revolutionized the speed and quality with which the software we use
every day is developed. 

In the startup world, Eric Ries has shown us in his book The Lean Startup how delivering
value quickly in small chunks is essential for learning and innovation.
```

But how can individual employees resize value batches delivered? 

```markdown
Reducing our batch sizes requires changing not how we manage tasks and projects, but how 
we manage the information content of those projects.

We need to change our conception of what we are producing, from final deliverables to 
what I will call “intermediate packets.” Instead of seeing the final product (the 
deliverable we sell to the client) as the only repository of value, we package up all the
intermediate steps — the research, notes, brainstorms, examples, outlines, prototypes, 
drafts, and even crazy ideas we choose not to pursue — as reusable components for later
consumption.

At the end of the project, instead of making one final crazy all-night push to load every
single part of the project into our brain for final delivery, our task is much easier: 
final assembly of the previously built packets.
```

The benefit of modularizing is later reusability. Taken to its ultimate conclusion, you get what Tiago calls a "flywheel" (or productivity):

```markdown
After you’ve been working this way for awhile, there is a final benefit: you gain the
ability to complete entire projects merely by assembling previously created packets. 
There seems to be a critical mass in a given industry or area — once you reach that mass,
each additional packet added creates exponential value in the connections it creates with
others.

This is the mythical productivity flywheel—a system that produces value almost on its own,
while you take a back seat as curator, manager, and gatekeeper.
```

So like modules/packages in software development. The followup claim I'm less sure/convinced of:

```markdown
So what is required to make this new approach a reality? It requires us to get much, 
much better at packaging our work mid-stream. Here’s what makes it difficult: we can’t
afford to do this packaging during the project, because every spare moment is needed to
race toward the deadline. And we can’t do it after the project ends, because by then 
we’re already off to the next one. No, this packaging has to be embedded into the actual
way we work moment to moment, so that it doesn’t take any extra time whatsoever.

This need for a new way of defining, packaging, and delivering knowledge work is why I 
believe the humble category of note-taking apps represents the next frontier of 
productivity. Their purpose is much different from file storage services like Box, 
Dropbox, and iCloud, as well as cloud-based suites like Google Drive and Microsoft Office
360. They don’t optimize for finished documents ready to be printed, or for convenient 
groupings of project files, or storage space or speed or collaboration or any of the other
things one could optimize for. Instead, they optimize for *productive randomness*, for
serendipity, for seemingly bizarre juxtapositions of apparently unconnected information to
train our capacity for connecting it. Each person possesses a unique lifestream of 
information from numerous sources, and success increasingly depends on curating, tweaking,
redirecting, and capturing value from this stream to use in our work. Instead of hiding 
our insights and learnings in neatly labeled folders and files, we want to expose them as
intermediate packets of ever-evolving, intermediate work.
```

I think I'm mainly unconvinced because I'm unfamiliar enough with note-taking apps to see how they're qualitatively different from what I already do in this living document (aside from lower note-taking friction/activation energy). 

<a name="#Batch-low-intensity-tasks"></a>
### Batch low-intensity tasks
([overview](#overview)) 

This is mainly from Terry Tao's [eponymous article](https://terrytao.wordpress.com/career-advice/batch-low-intensity-tasks-together/). I liked it a lot, and find myself doing it all the time. 

```markdown
The tasks one is faced with in work can be broadly divided into two categories:

1. “high-intensity” tasks, which are complex and require your full concentration and 
focus (e.g. writing a research paper; preparing for a class or talk; writing a lengthy,
detailed, and careful email; thinking about a mathematical problem; reading a research 
paper or text), and

2. “low-intensity” tasks, which are routine (but can be time-consuming) and do not
require much mental energy (e.g. filling out paperwork; teaching a class or giving a talk
that you have already prepared; writing a short email response; errands and appointments;
reading email or browsing the web).

Working with high-intensity requires a rather different “mode” of thought than with low-
intensity tasks.  (For instance, I find it can take a good half-hour or so of uninterrupted
thinking before I am fully focused on a maths problem, with all the relevant background at
my fingertips.) To reduce the mental fatigue of transitioning from one “mode” to another,
I find it useful to batch similar low-intensity tasks together, and to separate them in time 
(or space) from the high-intensity ones.

If one has a batch of tasks that are both low-intensity and low-priority, then it is probably
a good idea to set it aside until one really needs a break from more high-intensity work; for
instance, if I get too frustrated on an obstacle in my research, I find this to be a good 
time to go do some accumulated errands or paperwork, or even just to catch up on my email and
web browsing.  Having some easy tasks of this nature lying around is then handy for killing 
time in a reasonably productive fashion until one’s creative energies return.

Note that batching only works well for *low-intensity* tasks.  A high-intensity task requires so
much focus, and exhausts so much of one’s mental stamina, that it can be counterproductive or 
distracting to mix this activity with other low or high intensity tasks.
```

In his [time management post](https://terrytao.wordpress.com/2008/08/07/on-time-management/), Terry adds:

```markdown
Another thing is that my ability to do any serious mathematics fluctuates greatly from day to
day; sometimes I can think hard on a problem for an hour, other times I feel ready to type up 
the full details of a sketch that I or my coauthors already wrote, and other times I only feel
qualified to respond to email and do errands, or just to take a walk or even a nap. I find it
very helpful to organise my time to match this fluctuation: for instance, if I have a free 
afternoon, and feel inspired to do so, I might close my office door, shut off the internet,
and begin typing on a languishing paper; or if not, I go and work on a week’s worth of email,
referee a paper, write a blog article, or whatever else seems suited to my current levels of
energy and enthusiasm. It is fortunate in mathematics that a large fraction of one’s work 
(with the notable exception of teaching, which one then has to build one’s schedule around)
can be flexibly moved from one time slot to another in this manner. (A corollary to this is 
that one should deal with tasks before they become so urgent that they have to be done 
immediately, thus disrupting one’s time flexibility.)

It helps a lot here to be able to honestly and accurately evaluate your work potential 
(a function of your location, your current level of motivation and energy, your upcoming 
duties and commitments, availability of resources, and the expected level of distraction)
for a given period of time into the future (e.g. the rest of the day): being either
overconfident or underconfident about what you can achieve leads to taking on either more or
less than you can properly handle, both of which lead to inefficiencies (I have learned both 
sides of this from direct experience).
```

You can block out in both space and time:

```markdown
For example, you can devote a block of time to clearing a lot of “trivial” tasks off of your
plate.  Schedule all the “distracting” tasks (e.g. office hours and other appointments) in a
single day; try to bunch up teaching days; etc.  (I found, for instance, that teaching two 
sections of a large calculus class back to back (e.g. at 9am and then at 10am) led to 
significant time savings in class preparation (as well as savings in mental energy), when
compared to teaching two different classes, or the same class at very different times.)

One can also do this blocking off in space as well as in time.  For instance, with regards to
keeping track of paperwork, I have one small area of my office for “important” forms and 
records that I am likely to need to deal with again in the future, and a larger area in
another part of my office for “mundane” paperwork which have a low (but non-zero) probability
of being needed again in the future.  I don’t organise or file the latter set of papers very
much, given how rarely I need to retrieve files from it; it tends to accumulate in a pile, 
which I sort through (and mostly discard) every few months or so.  (But I do make an effort
to keep the “important” forms relatively organised, and to not have them be cluttered by the 
much larger set of “mundane” forms.)

In a somewhat analogous fashion, one can have an “out” tray for low-priority physical mail, 
and send them all out at once, rather than making multiple trips to the office mail room in 
one day.  (While doing so, of course, that would be a good time to check one’s mailbox, or any 
other task that requires walking around the department.)
```

Email (see also [email](#email)):

```markdown
With regards to email, an assembly line approach seems to be efficient: wait until it builds
up, and then (a) pass through deleting spam, (b) pass through again dealing with easily dealt
with emails (ones that need to be read once and discarded or filed, or require a very brief 
response, or pushed into some sort of “pending” folder; and then (c) deal with one or more of
the emails that demand a longer response, if you feel that this is an appropriate time to do so.
```

Even browsing can be batched:

```markdown
If you like to browse multiple web sites during the course of the day, I recommend using a 
feed aggregator (I myself use Google Reader) so that you can do all your browsing at once, 
so that they do not distract you from your other tasks.
```

This post of Terry's does show its age, since Google Reader [was discontinued in 2013](https://googleblog.blogspot.com/2013/03/a-second-spring-of-cleaning.html) due to declining usage and Google's own stated imperative to "focus so as to make the most of the opportunities afforded by the new multiple-device-per-person computing environment" instead of "spreading themselves too thin":

```markdown
We launched Google Reader in 2005 in an effort to make it easy for people to discover and 
keep tabs on their favorite websites. While the product has a loyal following, over the 
years usage has declined. So, on July 1, 2013, we will retire Google Reader.
```

This is related to, but not the same as, [structured procrastination](#structured-procrastination).

<a name="#Tactical-procrastination"></a>
### Tactical procrastination
([overview](#overview))  

From Terry Tao's pretty comprehensive post on [various time management tricks](https://terrytao.wordpress.com/2008/08/07/on-time-management/):

```markdown
There are also many situations in which it makes tactical sense to defer, delay, delegate, 
or procrastinate on any given task, and go work on something else instead in the meantime;
not everything is equally important, and also a given task may in fact become much easier 
(and be completed in a much better way) if one waits for one’s own skills to get stronger,
or for other events to happen that reduce the importance or need for the task in the first 
place.

My current papers on wave maps, for instance, have been delayed for years, much to my own 
personal frustration, but in retrospect I can see that it was actually a good idea to let 
those papers sit for a while, as the project as I had originally conceived it was a 
technical nightmare, and it really was necessary to wait for the technology and 
understanding in the field to improve before being able to tackle it in a relatively 
civilised manner.  
```

<a name="#Structured-procrastination"></a>
### Structured procrastination
([overview](#overview))  

There's a great essay by Stanford professor John Perry, [Structured Procrastination](http://www.structuredprocrastination.com/), which I just found today in the comments section of [this 2009 Scott Aaronson post](https://www.scottaaronson.com/blog/?p=388). I'll quote the parts that I liked below, trying to not just reproduce the whole shebang.

What is structured procrastination?

```markdown
All procrastinators put off things they have to do. Structured procrastination is
the art of making this bad trait work for you. 

The key idea is that procrastinating does not mean doing absolutely nothing. 
Procrastinators seldom do absolutely nothing; they do marginally useful things,
like gardening or sharpening pencils or making a diagram of how they will reorganize
their files when they get around to it. 

Why does the procrastinator do these things? Because they are a way of not doing 
something more important. If all the procrastinator had left to do was to sharpen
some pencils, no force on earth could get him do it. However, the procrastinator 
can be motivated to do difficult, timely and important tasks, as long as these tasks 
are a way of not doing something more important.

Structured procrastination means shaping the structure of the tasks one has to do in
a way that exploits this fact. The list of tasks one has in mind will be ordered by 
importance. Tasks that seem most urgent and important are on top. But there are also
worthwhile tasks to perform lower down on the list. Doing these tasks becomes a way 
of not doing the things higher up on the list. With this sort of appropriate task 
structure, the procrastinator becomes a useful citizen. Indeed, the procrastinator can
even acquire, as I have, a reputation for getting a lot done.

Procrastinators often follow exactly the wrong tack. They try to minimize their
commitments, assuming that if they have only a few things to do, they will quit 
procrastinating and get them done. But this goes contrary to the basic nature of the
procrastinator and destroys his most important source of motivation. The few tasks on
his list will be by definition the most important, and the only way to avoid doing them
will be to do nothing. This is a way to become a couch potato, not an effective human being.
```

So the important tasks never get done? What the hell??

```markdown
The trick is to pick the right sorts of projects for the top of the list. 

The ideal sorts of things have two characteristics, First, they seem to have clear
deadlines (but really don't). Second, they seem awfully important (but really aren't). 

Luckily, life abounds with such tasks. In universities the vast majority of tasks fall
into this category, and I'm sure the same is true for most other large institutions. 

Take for example the item right at the top of my list right now. This is finishing an 
essay for a volume in the philosophy of language. It was supposed to be done eleven months
ago. I have accomplished an enormous number of important things as a way of not working on
it. A couple of months ago, bothered by guilt, I wrote a letter to the editor saying how 
sorry I was to be so late and expressing my good intentions to get to work. Writing the 
letter was, of course, a way of not working on the article. It turned out that I really
wasn't much further behind schedule than anyone else. And how important is this article 
anyway? Not so important that at some point something that seems more important won't come
along. Then I'll get to work on it.
```

Example of John as excellent Resident Fellow in Soto House:

```markdown
The most perfect situation for structured procrastination that I ever had was when my
wife and I served as Resident Fellows in Soto House, a Stanford dormitory. In the evening,
faced with papers to grade, lectures to prepare, committee work to be done, I would leave
our cottage next to the dorm and go over to the lounge and play ping-pong with the 
residents, or talk over things with them in their rooms, or just sit there and read the 
paper. I got a reputation for being a terrific Resident Fellow, and one of the rare profs 
on campus who spent time with undergraduates and got to know them. What a set up: play ping
pong as a way of not doing more important things, and get a reputation as Mr. Chips.
```

A wry final remark:

```markdown
The observant reader may feel at this point that structured procrastination requires a 
certain amount of self-deception, since one is in effect constantly perpetrating a pyramid
scheme on oneself. Exactly. One needs to be able to recognize and commit oneself to tasks
with inflated importance and unreal deadlines, while making oneself feel that they are 
important and urgent. This is not a problem, because virtually all procrastinators have 
excellent self-deceptive skills also. And what could be more noble than using one character
flaw to offset the bad effects of another?
```

The 2009 Scott Aaronson post I linked to above, by the way, is just as funny in its own inimitably Aaronsonian way, so I had to [save it here](#email). 

<a name="#Email"></a>
### Email
([overview](#overview))      

The main impetus for creating this subsection was Scott Aaronson's joke post [The Email Event Horizon](https://www.scottaaronson.com/blog/?p=388), written way back in 2009, which is too funny (and short enough anyway) not to reproduce in full:

```markdown
I know I’ve been gone from the shtetl too long—I even stood by as a P=NP goon performed
a drive-by shooting through my comments section.  Part of the explanation, I’m ashamed 
to admit, is that I’ve been procrastinating by proving theorems and writing papers,
rather than building up the massive corpus of blog entries on which my tenure case will 
undoubtedly rest.

But most of my absence has an unhappier source.  At an unknown time about three weeks ago,
I crossed the Email Event Horizon—defined in General Unproductivity as the point beyond 
which you could *literally spend your entire day answering emails*, yet still have more 
emails at the end of the day demanding immediate attention than you had at the beginning. 
Not spam or crank mail, but worthy missives from students, prospective students, high-
school students, secretaries, TAs, fellow committee members, conference organizers, visit 
hosts, speakers, editors, co-editors, grant officers, referees, colleagues … everything, 
always, requiring you to do something, commit to some decision, send a title and abstract,
pick dates for the trip, exercise Genuine Conscious Thought.  No one ever writes:

	Please respond to the situation described above by cracking a joke, the less tasteful
	the better.  You will never need to deal with this matter again.

I don’t know the precise moment when I crossed the EEH—there was nothing to herald it, it
felt like any other moment—but it’s obvious now that I’m in a new, unfamiliar causal region
(and that, while I might have thought I’d crossed years ago, I hadn’t).  Communication from
inside the EEH to the external universe is theoretically possible, but like Hawking
radiation, it tends to be excruciatingly slow—and when it finally arrives, might simply
regurgitate the incoming information in garbled form.

When I was a student, I used to wonder constantly about the professors who’d ignore my long,
meticulously-crafted emails or fire off one-word replies, yet who might suddenly have an hour
for me if I walked into their offices.  Were they senile?  Rude?  Did they secretly despise
me?  *Now* I get it, now I understand—yet I doubt I could explain the warped spacetime
Gmailometry I now inhabit to my own past self.  On the other hand, the recognition of what’s
happened is itself a sort of liberation.  I’m starting to grasp what’s long been obvious to 
many of you, those who crossed the EEH before I got my first AOL account in seventh grade: 
that it’s useless to struggle.  By definition, the speed required to escape the EEH exceeds
that of typing, while the mental energy required to accelerate a massive, resting theorist to 
such a speed is infinite.  So there’s nothing to do but blog, goof off, prove theorems, let 
the starred-but-unanswered inquiries pile higher and higher, and await the Email Singularity
in my causal future.
```

Okay, a bit more seriously -- here's what Terry Tao does:

```markdown
With regards to email, an assembly line approach seems to be efficient: wait until it builds
up, and then (a) pass through deleting spam, (b) pass through again dealing with easily dealt
with emails (ones that need to be read once and discarded or filed, or require a very brief 
response, or pushed into some sort of “pending” folder; and then (c) deal with one or more of
the emails that demand a longer response, if you feel that this is an appropriate time to do so.
```

See also [structured procrastination](#structured-procrastination).

<a name="#general-statistics"></a>
## General statistics
([overview](#overview))

Piet Hein:

```markdown
The road to wisdom? --- Well, it's plain
and simple to express:

 Err
 and err
 and err again
 but less
 and less
 and less.
```

Peter Medawar:

```markdown
Most scientists receive no tuition in scientific method, but those who have been instructed perform 
no better as scientists than those who have not. Of what other branch of learning can it be said that 
it gives its proficients no advantage; that it need not be taught or, if taught, need not be learned?
```

Cosma Shalizi:

```markdown
It’s much easier to get rid of wrong notions than it is to find correct ones, if the latter is 
possible at all.
```

Cosma Shalizi again, this time on an interesting argument for how “good statistics” should be defined (cf. [Properties versus Principles debate](http://bactra.org/notebooks/properties-vs-principles-for-statistics.html)):

```markdown
In his book The Theory of Literary Criticism, John Ellis argues that it's a mistake to try to define 
many categories in terms of criteria which are applicable to the objects of the categories in themselves; 
they are rather defined (in large part) by their relations to us and to our purposes. The really persuasive 
(to me) example is "weed": a weed is simply an obnoxious plant. Plants may be obnoxious because they are 
fast-growing, hardy, perennial, etc., etc., but none of these properties, or any Boolean combination 
thereof, *defines* weeds; their relation to our purposes in gardening does. It's perfectly sensible to say 
"kudzu is a weed, and one of the reasons why is that it grows so fast", but fast growth doesn't define weeds. 
The quest for criteria or defining principles of weed-hood is (if I may put it this way) fruitless.

I wonder if one can't say something similar about good statistics? What makes something a good method of 
statistical inference is that it gives us a reliable, low-error way of drawing conclusions from data. The 
reasons why a given procedure is reliable, and the ways we find them, are many and various. In the case of 
the Neyman-Pearson lemma, we directly minimize error probabilities; but sometimes we maximize likelihood, 
sometimes we use conditioning to update prior probability distributions, etc. None of these --- particularly 
the last --- *defines* a reliable way of learning from data.
```

<a name="#the-role-of-statistics-in-science"></a>
## The role of statistics in science
([overview](#overview))

This quote from Cosma's [book review](http://bactra.org/reviews/error/) of Deborah Mayo's *Error and the Growth of Experimental Knowledge* contains the most inventive and *original* description of Popperian falsification I’ve ever seen:

```markdown
In our own time, Medawar's friend Karl Popper achieved (fully deserved) eminence by tenacious 
insistence on the importance of this point, becoming a sort of Lenin of the philosophy of science. 
Instead of conferring patents of epistemic nobility, lawdoms and theoryhoods, on certain hypotheses, 
Popper hauled them all before an Anglo-Austrian Tribunal of Revolutionary Empirical Justice.

The procedure of the court was as follows: the accused was blindfolded, and the magistrates then formed 
a firing squad, shooting at it with every piece of possibly-refuting observational evidence they could 
find. Conjectures who refused to present themselves might lead harmless lives as metaphysics without 
scientific aspirations; conjectures detected peaking out from under the blindfold, so as to dodge the 
Tribunal's attempts at refutation, were declared pseudo-scientific and exiled from the Open Society of 
Science. Our best scientific theories, those Stakhanovites of knowledge, consisted of those conjectures 
which had survived harsh and repeated sessions before the Tribunal, demonstrated their loyalty to the 
Open Society by appearing before it again and again and offering the largest target to refutation that 
they could, and so retained their place in the revolutionary vanguard until they succumbed, or were 
displaced by another conjecture with even greater zeal for the Great Purge.

As Popper famously said, better our hypotheses die for our errors than ourselves... It's an answer with 
nice, clean lines, and makes lots of sense to the scientist-at-the-bench, like Medawar.

Alas, the Revolution runs into trouble on several fronts, for instance statistics.
```

Say more words? 

```markdown
Suppose I tell you that a certain slot machine will pay out money 99% of the time.
Being credulous, unnaturally patient, and abundantly supplied with coins, you play 
it 10,000 times and find that it pays out only twice. This is sufficient for you to
tell me to get stuffed, if not to sue, and one would think that it would be enough
for the Tribunal to shoot my poor conjecture dead, but actually it escapes unharmed.
The problem for Uncle Karl is that getting two successes in ten thousand trials is
possible given my assertion, and the Tribunal is only authorized to eliminate
conjectures in actual contradiction to the facts, as "no mammals lay eggs" is 
contradicted by the platypus. Popper realized this, and worried about it, eventually 
saying that we just have to make "risky decisions" about when to reject statistical 
hypotheses.

But the challenges facing the Tribunal in the execution of its duty mount: another
"risky decision" is required, about what ammunition the firing squad can legitimately
use, i.e., about what evidence will be accepted when we see whether or not a hypothesis
stands up. (The number of times my students have apparently refuted physical laws gives
me great sympathy for the European naturalists who refused to accept reports of the 
platypus's peculiarities for decades.) 

Then there is the problem of conjectural conspiracy: an isolated hypothesis almost never
leads to anything we can test observationally; it is only in combination with "auxiliary"
hypotheses, sometimes very many of them indeed, that is gives us actionable predictions.
But then if a prediction proves false, all we learn is that at least one of our
hypotheses is wrong, not which ones are the saboteurs. So far as deductive rectitude is 
concerned, we are free to frame whichever auxiliaries we like least, and save our
favorite hypothesis from execution at the hands of the Tribunal.

The Tribunal even, for all its appearance of salutary rigor, lets far too many suspects
go: every conjecture which is compatible with the evidence. These last two problems,
respectively those of Quine-Duhem and of methodological underdetermination, are so severe 
that they form the core of the (intellectually respectable) argument for the counter-
revolutionary deviation of scientific relativism. (The argument throttles itself neatly,
but that's a subject for another essay.) 

Yet in ordinary life, never mind science, we evade these problems --- those of testing
statistical hypotheses, of selecting evidence, of Quine-Duhem, of methodological
underdetermination --- every time we change a light-bulb, so something has clearly gone
very wrong here (as, in revolutions, things are wont to do).
```

Deborah Mayo on Popper being too soft with conjectures:

```markdown
Although Popper's work is full of exhortations to put hypotheses through the wringer, to make them "suffer 
in our stead in the struggle for the survival of the fittest," the tests Popper sets out are white-glove 
affairs of logical analysis. If anomalies are approached with white gloves, it is little wonder that they 
seem to tell us only that there is an error somewhere and that they are silent about its source. We have 
to become shrewd inquisitors of errors, interact with them, simulate them (with models and computers), 
amplify them: we have to learn to make them talk.
```

Where does Mayo come into the picture?

```markdown
Fortunately, scientists have not only devoted much effort to making errors talk, they have even developed
a theory of inquisition, in the form of mathematical statistics, especially the theory of statistical
inference worked out by Jerzy Neyman and Egon Pearson in the 1930s. Mayo's mission is largely to show how
this very standard mathematical statistics justifies a very large class of scientific inferences, those 
concerned with "experimental knowledge," and to suggest that the rest of our business can be justified on
similar grounds. Statistics becomes a kind of applied methodology, as well as the "continuation of 
experiment by other means."

Mayo's key notion is that of a severe test of a hypothesis, one with "an overwhelmingly good chance of
revealing the presence of a specific error, if it exists --- but not otherwise" (p. 7). More formally
(when we can be this formal), the severity of a passing result is the probability that, if the hypothesis
is false, our test would have given results which match the hypothesis less well than the ones we actually
got do, taking the hypothesis, the evidence used in the test, and the way of calculating fit between
hypothesis and evidence to be fixed. If a severe test does not turn up the error it looks for, it's good
grounds for thinking that the error is absent. By putting our hypotheses through a battery of severe 
tests, screening them for the members of our "error repertoire," our "canonical models of error," we can 
come to have considerable confidence that they are not mistaken in those respects. Instead of a method for
infallibly or even reliably finding truths, we have a host of methods for reliably finding errors: which
turns out to be good enough.

Experimental inquiry, for Mayo, consist of breaking down the question at hand into a series of small bits, 
each of which is relatively easily subjected to severe tests for error, or (depending on how you look at
it) is itself a severe probe for a certain error. In doing this we construct a "hierarchy of models" (an 
idea of Patrick Suppes's, here greatly elaborated). In particular, we need data models, models of how the
data are collected and massaged. "Error" here, as throughout Mayo's work, must be understood in a rather
catholic sense: any deviation from the conditions we assumed in our reasoning about what the experimental
outcomes should be. If we guess that a certain effect (the bending of spoons, let us say) is due to a
certain cause (e.g., the psychic powers of Mr. Uri Geller), it is not enough that spoons bend reliably in
his presence: we must also rule out other mechanisms which would produce the same effect (Mr. Geller's 
bending the spoons with his hands while we're not looking, his substituting pre-bent spoons for unbent 
ones ditto, etc., through material for several lawsuits for libel). But this solves the Quine-Duhem problem.

In fact, it gets better. Recall that methodological underdetermination (which goes by the apt name of MUD 
in Error) is the worry that no amount or quality of evidence will suffice to pick out one theory as the best,
because there are always indefinitely many others which are in equal accord with that evidence, or, to use 
older language, equally well save the phenomena. But saving the phenomena is not the same as being subjected
to a severe test: and, says Mayo, the point is severe testing. While I'm mostly persuaded by this argument,
I'm less sanguine than Mayo is about our ability to always find experimental tests which will let us
discriminate between two hypotheses. I'm fully persuaded that this kind of testing really does underwrite 
our knowledge of phenomena, of (in Nancy Cartwright's phrase) "nature's capacities and their measurement," 
and Mayo herself insists on the importance of experimental knowledge in just this sense (e.g., the remarks 
on "asking the wrong question," pp. 188--9). I'm less persuaded that we can usually or even often make 
justified inferences from this "formal" sort of experimental knowledge, knowledge of the distribution of 
experimental outcomes, to "substantive" statements about objects, processes and the like (e.g., from the
experimental success of quantum mechanics to wave-functions). As an unreconstructed (undeconstructed?) 
scientific realist, I make such inferences, and would like them to be justified, but find myself left hanging.

Distributions of experimental outcomes, then, are the key objects for Mayo's tests, especially the standard 
Neyman-Pearson statistical tests. The kind of probabilities Mayo, and Neyman and Pearson, use are
probabilities of various things happening: meaning that the probability of a certain result, p(A), is the 
proportion of times A occurs in many repetitions of the experiment, its frequency. This is a very familiar 
sense of probability; it's the one we invoke when we say that a fair coin has a 50% probability of coming up
heads, that the chance of getting three sixes with fair (six-sided!) dice is 1 in 216, that a certain 
laboratory procedure will make an indicator chemical change from red to blue 95% of the time when a toxin 
is present. Or, more to the present point: "the hypothesis is significant at the five percent level" means 
"the hypothesis passed the test, and the probability of its doing so, if it were false, is no more than five
percent," which means "if the hypothesis is false, and we repeated this experiment many times, we would
expect to get results inside our passing range no more than five percent of the time."
```

So Mayo is a frequentist. 

<a name="#statistical-literacy"></a>
## Statistical literacy
([overview](#overview))

Carl Shulman's [Research advice](https://docs.google.com/document/d/1_yuuheVqp1quDfkuRcpoW_HO7jPaI7QnRjF1zl_VovU/edit) has the following bit on statistical literacy which I feel really strongly about and wholeheartedly endorse:

```markdown
Use basic arithmetic and statistics frequently and briefly as part of thinking rather than as occasional or 
separate exercises. … Try to convert qualitative claims into quantitative Fermi estimates whenever possible.

In my experience people almost never do enough Fermis with look-ups from Wiki//government sources. And 
especially they have too high a barrier to doing it and won't do it in casual conversation or exploration.

Sometimes it's because talking is not about information and other things are shinier. Some people are afraid 
they'll be wrong, and don't trust their ability to do it (and don't test that). Sometimes it’s because of a 
lack of affordance/habit/knowing about the bigger and standard resources or the basic toolkits of Fermis: 
prices, populations, sales. Sometimes it’s issues with arithmetic and basic statistics fluency/aversion. 
Sometimes because it gives an unwelcome answer.

Worked examples with numbers and realistic figures erode plausible deniability and attractive lies, and force 
explicit claims, use of evidence, and argument.
```

Razib Khan:

```markdown
But, there's another problem, and that is the fact that statistical and probabilistic thinking is a real 
damper on "intellectual" conversation. By this, I mean that there are many individuals who wish to make 
inferences about the world based on data which they observe, or offer up general typologies to frame a 
subsequent analysis. These individuals tend to be intelligent and have college degrees. Their discussion 
ranges over topics such as politics, culture and philosophy. But, introduction of questions about the 
moments about the distribution, or skepticism as to the representativeness of their sample, and so on, tends 
to have a chilling affect on the regular flow of discussion. While the average human being engages mostly 
in gossip and interpersonal conversation of some sort, the self-consciously intellectual interject a bit of 
data and abstraction (usually in the form of jargon or pithy quotations) into the mix. But the raison d'etre 
of the intellectual discussion is basically signaling and cuing; in other words, social display. No one 
really cares about the details and attempting to generate a rigorous model is really beside the point. Trying 
to push the N much beyond 2 or 3 (what you would see in a college essay format) will only elicit eye-rolling 
and irritation.
```

From [Marc Andreessen gives the career advice that nobody wants to hear](https://www.businessinsider.com/andreessen-whatever-you-do-dont-follow-your-passion-2014-5/?IR=T):

```markdown
"Do what you love" / "Follow your passion" is dangerous and destructive career advice. We tend to hear it 
from (a) Highly successful people who (b) Have become successful doing what they love. The problem is that 
we do NOT hear from people who have failed to become successful by doing what they love. Particularly pernicious 
problem in tournament-style fields with a few big winners lots of losers: media, athletics, startups. Better 
career advice may be "Do what contributes" -- focus on the beneficial value created for other people vs just 
one's own ego. People who contribute the most are often the most satisfied with what they do -- and in fields 
with high renumeration, make the most $. Perhaps difficult advice since requires focus on others vs oneself -- 
perhaps bad fit with endemic narcissism in modern culture? Requires delayed gratification -- may toil for many 
years to get the payoff of contributing value to the world, vs short-term happiness.
```
