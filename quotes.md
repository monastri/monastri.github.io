I like a lot of quotes. 

<a name="#overview"></a>

## Overview

I've sorted the quotes below into the following provisional categories:

1. [Research](#research)
   1. [Debt, interpretive labor, distillation](#distillation-and-research-debt)
2. [Erisology](#erisology)
   1. [Argumentative charity](#argumentative-charity)
2. [Teaching and learning](#teaching-and-learning)
   1. [Errors vs bugs](#errors-vs-bugs)
   2. [Polymathy](#polymathy)
2. [Psychology](#psychology)
2. [Philosophy](#philosophy)
   1. [General philosophy](#general-philosophy)
   2. [Diseased philosophy](#diseased-philosophy)
   2. [Morality](#morality)
   3. [Slack and deliberate mediocrity](#slack-and-deliberate-mediocrity) 
2. [Statistics](#statistics)
   1. [General stats](#general-stats)
   2. [Statistical literacy](#statistical-literacy)
2. [Math](#math)
   1. [Solving famous open problems](#solving-famous-open-problems)
   2. [Mathematical maturity](#mathematical-maturity)
   3. [Good mathematics](#good-mathematics)
   4. [What every mathematician should know](#what-every-mathematician-should-know)
2. [General intelligence](#general-intelligence) 
   1. [LOGI](#logi)
2. [Miscellaneous](#miscellaneous)

Have fun reading them! I certainly did.

<a name="#erisology"></a>

## Research
([overview](#research))

<a name="#distillation-and-research-debt"></a>

### Distillation and research debt
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

<a name="#erisology"></a>

## Erisology
([overview](#overview))

<a name="#argumentative-charity"></a>

### Argumentative charity
([overview](#overview))

My go-to text for charity is Scott Alexander's [founding post](https://slatestarcodex.com/2013/02/12/youre-probably-wondering-why-ive-called-you-here-today/) for his blog SSC. Here's the part I liked, which is pretty much all of the 'transferable' part:

```markdown
Absurdity is the natural human tendency to dismiss anything you disagree with as so stupid it doesn’t
even deserve consideration. In fact, you are virtuous for not considering it, maybe even heroic! You’re
refusing to dignify the evil peddlers of bunkum by acknowledging them as legitimate debate partners.

Charity is the ability to override that response. To assume that if you don’t understand how someone
could possibly believe something as stupid as they do, that this is more likely a failure of understanding 
on your part than a failure of reason on theirs.
```

Charity should be thought of like Chesterton's fence:

```markdown
There are many things charity is not. Charity is not a fuzzy-headed caricature-pomo attempt to say no one 
can ever be sure they’re right or wrong about anything. Once you understand the reasons a belief is 
attractive to someone, you can go ahead and reject it as soundly as you want. Nor is it an obligation to
spend time researching every crazy belief that might come your way. Time is valuable, and the less of it
you waste on intellectual wild goose chases, the better.

It’s more like Chesterton’s Fence. G.K. Chesterton gave the example of a fence in the middle of nowhere. A
traveller comes across it, thinks “I can’t think of any reason to have a fence out here, it sure was dumb 
to build one” and so takes it down. She is then gored by an angry bull who was being kept on the other side
of the fence.

Chesterton’s point is that “I can’t think of any reason to have a fence out here” is the worst reason to 
remove a fence. Someone had a reason to put a fence up here, and if you can’t even imagine what it was, it
probably means there’s something you’re missing about the situation and that you’re meddling in things you
don’t understand. None of this precludes the traveller who knows that this was historically a cattle farming
area but is now abandoned – ie the traveller who understands what’s going on – from taking down the fence.

As with fences, so with arguments. If you have no clue how someone could believe something, and so you decide
it’s stupid, you are much like Chesterton’s traveler dismissing the fence (and philosophers, like travelers, 
are at high risk of stumbling across bull.)
```

Charity as default, because even when it's uncalled for or ostensibly unnecessary it can be advantageous:

```markdown
The most effective way to learn any subject is to try to figure out exactly why a wrong position is wrong. 
And sometimes even a complete disaster of a theory will have a few salvageable pearls of wisdom that can’t 
be found anywhere else. The rationalist forum Less Wrong teaches the idea of steelmanning, rebuilding a 
stupid position into the nearest intelligent position and then seeing what you can learn from it.
```

<a name="#teaching-and-learning"></a>

## Teaching and learning
([overview](#overview))

<a name="#errors-vs-bugs"></a>

## Errors vs bugs
([overview](#overview))

Sarah Constantin is one of my favorite writers. She has a blog, [Otium](https://srconstantin.wordpress.com/), and goes by 
celandine13 on LiveJournal. This quote on the _error vs bug model of learning_ comes from her LJ essay 
[Errors vs Bugs and the End of Stupidity](https://celandine13.livejournal.com/33599.html).

```markdown
A common mental model for performance is what I'll call the "error model."  In the error model, a person's 
performance of a musical piece (or performance on a test) is a perfect performance plus some random error.  
You can literally think of each note, or each answer, as x + c times epsilon_i, where x is the correct note 
/ answer, and epsilon_i is a random variable, iid Gaussian or something.  Better performers have a lower 
error rate c.  Improvement is a matter of lowering your error rate.  This, or something like it, is the model 
that underlies school grades and test scores. Your grade is based on the percent you get correct.  Your 
performance is defined by a single continuous parameter, your accuracy.

But we could also consider the "bug model" of errors.  A person taking a test or playing a piece of music is 
executing a program, a deterministic procedure.  If your program has a bug, then you'll get a whole class of 
problems wrong, consistently.  Bugs, unlike error rates, can't be quantified along a single axis as less or 
more severe.  A bug gets everything that it affects wrong.  And fixing bugs doesn't improve your performance 
in a continuous fashion; you can fix a "little" bug and immediately go from getting everything wrong to 
everything right.  You can't really describe the accuracy of a buggy program by the percent of questions it 
gets right; if you ask it to do something different, it could suddenly go from 99% right to 0% right.  You 
can only define its behavior by isolating what the bug does.

Often, I think mistakes are more like bugs than errors.  My clinkers weren't random; they were in specific 
places, because I had sub-optimal fingerings in those places.  A kid who gets arithmetic questions wrong 
usually isn't getting them wrong at random; there's something missing in their understanding, like not 
getting the difference between multiplication and addition.  Working generically "harder" doesn't fix bugs 
(though fixing bugs does require work). 

Once you start to think of mistakes as deterministic rather than random, as caused by "bugs" (incorrect 
understanding or incorrect procedures) rather than random inaccuracy, a curious thing happens.

You stop thinking of people as "stupid."

Tags like "stupid," "bad at X", "sloppy," and so on, are ways of saying "You're performing badly and I 
don't know why." Once you move it to "you're performing badly because you have the wrong fingerings," or 
"you're performing badly because you don't understand what a limit is," it's no longer a vague personal 
failing but a causal necessity. Anyone who never understood limits will flunk calculus. 

It's not you, it's the bug.
```

The rest of the linked article is _fantastic_. I had trouble quoting it because I felt like quoting everything.

<a name="#polymathy"></a>

### Polymathy
([overview](#overview))

Here's Eric Drexler on [how to understand everything](http://metamodern.com/2009/05/17/how-to-understand-everything-and-why/) and [how to learn about everything](http://metamodern.com/2009/05/27/how-to-learn-about-everything/).

I feel a sort of kinship with what people like Drexler are trying to do here, albeit for different reasons. To oversimplify by mapping my motivations in doing the same to the ‘carrot-and-stick’ model: my carrot is this intrinsic need to ‘see the Systems of the World’ (paraphrasing Neal Stephenson, evoking the unnamed protagonist in Ted Chiang’s Understand, etc); my stick is the pain of being blindsided by unknown unknowns (so I have to at least know the outlines of everything, if not their contents, and how they all fit together). A deeper understanding than the “teacher’s password” awareness of trivia competition champions and my high school self, but not much deeper, not so deep as to sacrifice breadth.

But I digress. Eric contends that we need "knowledge of extent and structure of human knowledge on a trans-disciplinary scale":

```markdown
Formal education in science and engineering centers on teaching facts and problem-solving skills in a 
series of narrow topics. It is true that a few topics, although narrow in content, have such broad 
application that they are themselves integrative: These include (at a bare minimum) substantial chunks 
of mathematics and the basics of classical mechanics and electromagnetism, with the basics of 
thermodynamics and quantum mechanics close behind.

Most subjects in science and engineering, however, are narrower than these, and advanced education 
means deeper and narrower education. What this kind of education omits is knowledge of extent and 
structure of human knowledge on a trans-disciplinary scale. This means understanding — in a particular,
limited sense — everything.
```

How to figure out the outlines of a field, and knowledge about knowledge:

```markdown
To avoid blunders and absurdities, to recognize cross-disciplinary opportunities, and to make sense of
new ideas, requires knowledge of at least the outlines of every field that might be relevant to the 
topics of interest. By knowing the outlines of a field, I mean knowing the answers, to some reasonable
approximation, to questions like these:

What are the physical phenomena?
What causes them?
What are their magnitudes?
When might they be important?
How well are they understood?
How well can they be modeled?
What do they make possible?
What do they forbid?

And even more fundamental than these are questions of knowledge about knowledge:

What is known today?
What are the gaps in what I know?
When would I need to know more to solve a problem?
How could I find what I need?

This sort of knowledge is a kind of specialty, really — a limited slice of learning, but oriented
crosswise. Because of this orientation, though, it provides leverage in integrating knowledge from
diverse sources.
```

Why care? Problem recognition is very important:

```markdown
It takes far less knowledge to recognize a problem than to solve it, yet in key respects, that bit 
of knowledge is more important: With recognition, a problem may be avoided, or solved, or an idea 
abandoned. Without recognition, a hidden problem may invalidate the labor of an hour, or a lifetime.
Lack of a little knowledge can be a dangerous thing.
```

Eric distinguishes between learning everything (which is impossible) and learning *about* everything (which is not):

```markdown
Note that the title above isn’t “how to learn everything”, but “how to learn about everything”. The 
distinction I have in mind is between knowing the inside of a topic in deep detail — many facts and 
problem-solving skills — and knowing the structure and context of a topic: essential facts, what 
problems can be solved by the skilled, and how the topic fits with others.

This knowledge isn’t superficial in a survey-course sense: It is about both deep structure and practical
applications. Knowing about, in this sense, is crucial to understanding a new problem and what must be 
learned in more depth in order to solve it. The cross-disciplinary reach of nanotechnology almost
demands this as a condition of competence.
```

Some advice on going about it:

```markdown
To intellectually ambitious students I recommend investing a lot of time in a mode of study that may 
feel wrong. An implicit lesson of classroom education is that successful study leads to good test 
scores, but this pattern of study is radically different. It cultivates understanding of a kind that 
won’t help pass tests — the classroom kind, that is:

Read and skim journals and textbooks that (at the moment) you only half understand. Include Science 
and Nature.

Don’t halt, dig a hole, and study a particular subject as if you had to pass a test on it.

Don’t avoid a subject because it seems beyond you — instead, read other half-understandable journals 
and textbooks to absorb more vocabulary, perspective, and context, then circle back.

Notice that concepts make more sense when you revisit a topic.

Notice which topics link in all directions, and provide keys to many others. Consider taking a class.

Continue until almost everything you encounter in Science and Nature makes sense as a contribution to 
a field you know something about.
```

<a name="#psychology"></a>

## Psychology
([overview](#overview))

Keith E. Stanovich, [How to Think Straight About Psychology](http://www.pearsonhighered.com/assets/hip/us/hip_us_pearsonhighered/samplechapter/0205914128.pdf):

```markdown
Often a person uses some folk proverb to explain a behavioral event even though, on an earlier occasion, this 
same person used a directly contradictory folk proverb to explain the same type of event. For example, most of 
us have heard or said, “look before you leap.” Now there’s a useful, straightforward bit of behavioral advice—
except that I vaguely remember admonishing on occasion, “he who hesitates is lost.” And “absence makes the heart 
grow fonder” is a pretty clear prediction of an emotional reaction to environmental events. But then what about 
“out of sight, out of mind”? And if “haste makes waste,” why do we sometimes hear that “time waits for no man”? 
How could the saying “two heads are better than one” not be true? Except that “too many cooks spoil the broth.” 
If I think “it’s better to be safe than sorry,” why do I also believe “nothing ventured, nothing gained”? And if 
“opposites attract,” why do “birds of a feather flock together”? I have counseled many students to “never to put 
off until tomorrow what you can do today.” But I hope my last advisee has never heard me say this, because I just 
told him, “cross that bridge when you come to it.”

The enormous appeal of clichés like these is that, taken together as implicit “explanations” of behavior, they 
cannot be refuted. No matter what happens, one of these explanations will be cited to cover it. No wonder we all 
think we are such excellent judges of human behavior and personality. We have an explanation for anything and 
everything that happens. Folk wisdom is cowardly in the sense that it takes no risk that it might be refuted.

That folk wisdom is “after the fact” wisdom, and that it actually is useless in a truly predictive sense, is why 
sociologist Duncan Watts titled one of his books: Everything Is Obvious—Once You Know the Answer (2011). Watts 
discusses a classic paper by Lazarsfeld (1949) in which, over 60 years ago, he was dealing with the common 
criticism that “social science doesn’t tell us anything that we don’t already know.” Lazarsfeld listed a series 
of findings from a massive survey of 600,000 soldiers who had served during World War II; for example, that men 
from rural backgrounds were in better spirits during their time of service than soldiers from city backgrounds. 
People tend to find all of the survey results to be pretty obvious. In this example, for instance, people tend 
to think it obvious that rural men would have been used to harsher physical conditions and thus would have 
adapted better to the conditions of military life. It is likewise with all of the other findings—people find them 
pretty obvious. Lazarsfeld then reveals his punchline: All of the findings were the opposite of what was originally 
stated. For example, it was actually the case that men from city backgrounds were in better spirits during their 
time of service than soldiers from rural backgrounds. The last part of the learning exercise is for people to 
realize how easily they would have explained just the opposite finding. In the case of the actual outcome, people 
tend to explain it (when told of it first) by saying that they expected it because city men are used to working 
in crowded conditions and under hierarchical authority. They never realize how easily they would have concocted an 
explanation for exactly the opposite finding.
```

<a name="#philosophy"></a>

## Philosophy
([overview](#overview))

<a name="#general-philosophy"></a>

### General philosophy
([overview](#overview))

Scott Aaronson, in response to Luke Muehlhauser's interview question "why be interested in philosophy?" in the [MIRI Conversations series](https://intelligence.org/2013/12/13/aaronson/):

```markdown
I’ve always been reflexively drawn to the biggest, most general questions that it seemed possible to 
ask. You know, like are we living in a computer simulation? if not, could we upload our consciousnesses
into one? are there discrete “pixels” of spacetime? why does it seem impossible to change the past? 
could there be different laws of physics where 2+2 equaled 5? are there objective facts about morality?
what does it mean to be rational? is there an explanation for why I’m alive right now, rather than some
other time? What are explanations, anyway? In fact, what really perplexes me is when I meet a smart, 
inquisitive person—let’s say a mathematician or scientist—who claims NOT to be obsessed with these huge
issues! I suspect many MIRI readers might feel drawn to such questions the same way I am, in which case
there’s no need to belabor the point.

From my perspective, then, the best way to frame the question is not: “why be interested in philosophy?” 
Rather it’s: “why be interested in anything else?”

But I think the latter question has an excellent answer. A crucial thing humans learned, starting around 
Galileo’s time, is that even if you’re interested in the biggest questions, usually the only way to make
progress on them is to pick off smaller subquestions: ideally, subquestions that you can attack using 
math, empirical observation, or both. For again and again, you find that the subquestions aren’t nearly
as small as they originally looked! Much like with zooming in to the Mandelbrot set, each subquestion has 
its own twists and tendrils that could occupy you for a lifetime, and each one gives you a new perspective 
on the big questions. And best of all, you can actually answer a few of the subquestions, and be the first
person to do so: you can permanently move the needle of human knowledge, even if only by a minuscule amount.
As I once put it, progress in math and science — think of natural selection, Godel’s and Turing’s theorems,
relativity and quantum mechanics — has repeatedly altered the terms of philosophical discussion, as
philosophical discussion itself has rarely altered them! (Of course, this is completely leaving aside math
and science’s “fringe benefit” of enabling our technological civilization, which is not chickenfeed either.)


On this view, philosophy is simply too big and too important to be confined to philosophy departments! Of 
course, the word “philosophy” used to mean the entire range of fundamental inquiry, from epistemology and
metaphysics to physics and biology (which were then called “natural philosophy”), rather than just close
textual analysis, or writing papers with names like “A Kripkean Reading of Wittgenstein’s Reading of Frege’s
Reading of Kant.” And it seems clear to me that there’s enormous scope today for “philosophy” in the former 
sense — and in particular, for people who love working on the subquestions, on pushing the frontiers of
neuroscience or computer science or physics or whatever else, but who also like to return every once in a
while to the “deep” philosophical mysteries that motivated them as children or teenagers. Admittedly, there
have been many great scientists who didn’t care at all about philosophy, or who were explicitly anti-philosophy.
But there were also scientists like Einstein, Schrodinger, Godel, Turing, or Bell, who not only read lots of
philosophy but (I would say) used it as a sort of springboard into science — in their cases, a wildly successful
one. My guess would be that science ultimately benefits from both the “pro-philosophical” and the
“anti-philosophical” temperaments, and even from the friction between them.
```

Scott on making progress on big problems:

```markdown
Pick off smaller subquestions: ideally, subquestions that you can attack using math, empirical observation, 
or both.

whenever it’s been possible to make definite progress on ancient philosophical problems, such progress has 
almost always involved a [kind of] “bait-and-switch.” In other words: one replaces an unanswerable
philosophical riddle Q by a “merely” scientific or mathematical question Q′, which captures part of what 
people have wanted to know when they’ve asked Q. Then, with luck, one solves Q′.

Of course, even if Q′ is solved, centuries later philosophers might still be debating the exact relation 
between Q and Q′! And further exploration might lead to other scientific or mathematical questions — Q′′, Q′′′,
and so on — which capture aspects of Q that Q′ left untouched. But from my perspective, this process of 
“breaking oﬀ” answerable parts of unanswerable riddles, then trying to answer those parts, is the closest thing
to philosophical progress that there is.

…A good replacement question Q′ should satisfy two properties: (a) Q′ should capture some aspect of the original
question Q — so that an answer to Q′ would be hard to ignore in any subsequent discussion of Q, [and] (b) Q′
should be precise enough that one can see what it would mean to make progress on Q′: what experiments one would
need to do, what theorems one would need to prove, etc.
```

<a name="#diseased-philosophy"></a>

### Diseased philosophy

From Scott Aaronson's [Quantum Computing Since Democritus](https://slatestarcodex.com/2014/09/01/book-review-and-highlights-quantum-computing-since-democritus/):

```markdown
The third thing that annoys me about the Chinese Room argument is the way it gets so much mileage from 
a possibly misleading choice of imagery, or, one might say, by trying to sidestep the entire issue of 
computational complexity purely through clever framing. We’re invited to imagine someone pushing around 
slips of paper with zero understanding or insight, much like the doofus freshmen who write 
(a + b)^2 = a^2 + b^2 on their math tests. 

But how many slips of paper are we talking about! How big would the rule book have to be, and how 
quickly would you have to consult it, to carry out an intelligent Chinese conversation in anything 
resembling real time? If each page of the rule book corresponded to one neuron of a native speaker’s 
brain, then probably we’d be talking about a “rule book” at leas the size of the Earth, its pages 
searchable by a swarm of robots traveling at close to the speed of light. When you put it that way, 
maybe it’s not so hard to imagine this enormous Chinese-speaking entity that we’ve brought into being 
might have something we’d be prepared to call understanding or insight.

Philosophers are so good at pure qualitative distinctions that it’s easy to slip the difference between 
“guy in a room” and “planet being processed by lightspeed robots” under the rug.
```

Brandon Watson, [The Success and Failure of Arguments](http://branemrys.blogspot.com/2010/09/success-and-failure-of-arguments.html):

```markdown
Sometimes you hear philosophers bemoaning the fact that philosophers tend not to form consensuses 
like certain other disciplines do (sciences in particular). 

But there is no great mystery to this. The sciences reward consensus-forming as long as certain 
procedures are followed: agreements through experimental verification, processes of peer review, etc. 
Philosophy has nothing like this. Philosophers are rewarded for coming up with creative reasons not to 
agree with other people. The whole thrust of professional philosophy is toward inventing ways to regard 
opposing arguments as failure, as long as those ways don't exhibit any obvious flaws. However much 
philosophers are interested in the truth, philosophy as a profession is not structured so as to converge 
on it; it is structured so as to have the maximal possible divergence that can be sustained given common 
conventions. 

We are not trained to find ways to come to agree with each other; we are trained to find ways to 
disagree with each other.
```

John Perry, from the introduction to *Identity, Personal Identity, and the Self*:

```markdown
There is something about practical things that knocks us off our philosophical high horses. Perhaps Heraclitus 
really thought he couldn't step in the same river twice. Perhaps he even received tenure for that contribution 
to philosophy. But suppose some other ancient had claimed to have as much right as Heraclitus did to an ox 
Heraclitus had bought, on the grounds that since the animal had changed, it wasn't the same one he had bought 
and so was up for grabs. Heraclitus would have quickly come up with some ersatz, watered-down version of 
identity of practical value for dealing with property rights, oxen, lyres, vineyards, and the like. And then 
he might have wondered if that watered-down vulgar sense of identity might be a considerably more valuable 
concept than a pure and philosophical sort of identity that nothing has.
```

<a name="#morality"></a>

### Morality
([overview](#overview))

Scott Alexander on the distinction between axiology, morality, and law, from [this essay](https://slatestarcodex.com/2017/08/28/contra-askell-on-moral-offsets/):

```markdown
Axiology is the study of what’s good. If you want to get all reductive, think of it as comparing the 
values of world-states. A world-state where everybody is happy seems better than a world-state where 
everybody is sad. A world-state with lots of beautiful art is better than a world-state containing only 
featureless concrete cubes. Maybe some people think a world-state full of people living in harmony with
nature is better than a world-state full of gleaming domed cities, and other people believe the opposite; 
when they debate the point, they’re debating axiology.

Morality is the study of what the right thing to do is. If someone says “don’t murder”, they’re making a 
moral commandment. If someone says “Pirating music is wrong”, they’re making a moral claim. Maybe some 
people believe you should pull the lever on the trolley problem, and other people believe you shouldn’t; 
when they debate the point, they’re debating morality.

(this definition elides a complicated distinction between individual conscience and social pressure; 
fixing that would be really hard and I’m going to keep eliding it)

Law is – oh, come on, you know this one. If someone says “Don’t go above the speed limit, there’s a 
cop car behind that corner”, that’s law. If someone says “my state doesn’t allow recreational marijuana,
but it will next year”, that’s law too. Maybe some people believe that zoning restrictions should ban 
skyscrapers in historic areas, and other people believe they shouldn’t; when they debate the point, 
they’re debating law.

These three concepts are pretty similar; they’re all about some vague sense of what is or isn’t desirable. 
But most societies stop short of making them exactly the same. Only the purest act-utilitarianesque 
consequentialists say that axiology exactly equals morality, and I’m not sure there is anybody quite that
pure. And only the harshest of Puritans try to legislate the state law to be exactly identical to the moral
one. To bridge the whole distance – to directly connect axiology to law and make it illegal to do anything 
other than the most utility-maximizing action at any given time – is such a mind-bogglingly bad idea that 
I don’t think anyone’s even considered it in all of human history.

These concepts stay separate because they each make different compromises between goodness, implementation, 
and coordination.

One example: axiology can’t distinguish between murdering your annoying neighbor vs. not donating money to 
savea child dying of parasitic worms in Uganda. To axiology, they’re both just one life snuffed out of the 
world beforeits time. If you forced it to draw some distinction, it would probably decide that saving the
child dying of parasitic worms was more important, since they have a longer potential future lifespan.

But morality absolutely draws this distinction: it says not-murdering is obligatory, but donating money to
Ugandais supererogatory. Even utilitarians who deny this distinction in principle will use it in everyday 
life: if theirfriend was considering not donating money, they would be a little upset; if their friend was
considering murder, they would be horrified. If they themselves forgot to donate money, they’d feel a little
bad; if they committedmurder in the heat of passion, they’d feel awful.

A final example: axiology tells us a world without alcohol would be better than our current world: ending
alcoholism could avert millions of deaths, illnesses, crimes, and abusive relationships. Morality only tells
us that we should be careful drinking and stop if we find ourselves becoming alcoholic or ruining our
relationships. And the law protests that it tried banning alcohol once, but it turned out to be unenforceable
and gave too many new opportunities to organized crime, so it’s going to stay out of this one except to say
you shouldn’t drink and drive.

So fundamentally, what is the difference between axiology, morality, and law?

Axiology is just our beliefs about what is good. If you defy axiology, you make the world worse.

At least from a rule-utilitarianesque perspective, morality is an attempt to triage the infinite demands 
of axiology, in order to make them implementable by specific people living in specific communities. It 
makes assumptions like “people have limited ability to predict the outcome of their actions”, “people 
are only going to do a certain amount and then get tired”, and “people do better with bright-line rules
than with vague gradients of goodness”. It also admits that it’s important that everyone living in a 
community is on at least kind of the same page morally, both in order to create social pressure to follow 
the rules, and in order to build the social trust that allows the community to keep functioning. If you 
defy morality, you still make the world worse. And you feel guilty. And you betray the social trust that
lets your community function smoothly. And you get ostracized as a bad person.

Law is an attempt to formalize the complicated demands of morality, in order to make them implementable
by a state with police officers and law courts. It makes assumptions like “people’s vague intuitive moral 
judgments can sometimes give different results on the same case”, “sometimes police officers and
legislators are corrupt or wrong”, and “we need to balance the benefits of laws against the cost of
enforcing them”. It also tries to avert civil disorder or civil war by assuring everybody that it’s in 
their best interests to appeal to a fair universal law code rather than try to solve their disagreements
directly. If you defy law, you still get all the problems with defying axiology and morality. And you 
make your country less peaceful and stable. And you go to jail.

In a healthy situation, each of these systems reinforces and promotes the other. Morality helps you 
implement axiology from your limited human perspective, but also helps prevent you from feeling guilty
for not being God and not being able to save everybody. The law helps enforce the most important moral
and axiological rules but also leaves people free enough to use their own best judgment on how to pursue
the others. And axiology and morality help resolve disputes about what the law should be, and then lend
the support of the community, the church, and the individual conscience in keeping people law-abiding.

In these healthy situations, the universally-agreed priority is that law trumps morality, and morality
trumps axiology. First, because you can’t keep your obligations to your community from jail, and you 
can’t work to make the world a better place when you’re a universally-loathed social outcast. But also,
because you can’t work to build strong communities and relationships in the middle of a civil war, and
you can’t work to make the world a better place from within a low-trust defect-defect equilibrium. But
also, because in a just society, axiology wants you to be moral (because morality is just a 
more-effective implementation of axiology), and morality wants you to be law-abiding (because law is 
just a more-effective way of coordinating morality). So first you do your legal duty, then your moral 
duty, and then if you have energy left over, you try to make the world a better place.

In unhealthy situations, you can get all sorts of weird conflicts. Most “moral dilemmas” are 
philosophers trying to create perverse situations where axiology and morality give opposite answers.
For example, the fat man version of the trolley problem sets axiology (“it’s obviously better to 
have a world where one person dies than a world where five people die”) against morality (“it’s a
useful rule that people generally shouldn’t push other people to their deaths”). And when morality 
and state law disagree, you get various acts of civil disobedience, from people hiding Jews from the
Nazis all the way down to Kentucky clerks refusing to perform gay marriages.

I don’t have any special insight into these. My intuition (most authoritative source! is never wrong!)
says that we should be very careful reversing the usual law-trumps-morality-trumps-axiology order, 
since the whole point of having more than one system is that we expect the systems to disagree and we 
want to suppress those disagreements in order to solve important implementation and coordination problems.
But I also can’t deny that for enough gain, I’d reverse the order in a heartbeat. If someone told me 
that by breaking a promise to my friend (morality) I could cure all cancer forever (axiology), then f@$k 
my friend, and f@$k whatever social trust or community cohesion would be lost by the transaction.
```

<a name="#slack-and-deliberate-mediocrity"></a>

### Slack and deliberate mediocrity
([overview](#overview))

The basic idea of Slack comes from the [eponymous LW post](https://www.lesswrong.com/posts/yLLkWMDbC9ZNKbjDG/slack). Quotes I liked, or that made sense to me:

```markdown
Definition: Slack. The absence of binding constraints on behavior.
Poor is the person without Slack. Lack of Slack compounds and traps.

Slack means margin for error. You can relax.

Slack allows pursuing opportunities. You can explore. You can trade.

Slack prevents desperation. You can avoid bad trades and wait for better spots. You can be efficient.

Slack permits planning for the long term. You can invest.

Slack enables doing things for your own amusement. You can play games. You can have fun.

Slack enables doing the right thing. Stand by your friends. Reward the worthy. Punish the wicked. 
You can have a code.

Slack presents things as they are without concern for how things look or what others think. You can 
be honest. ...

Slack in project management is the time a task can be delayed without causing a delay to either 
subsequent tasks or project completion time. The amount of time before a constraint binds.

A slacker is one who has a lazy work ethic or otherwise does not exert maximum effort. They slack off. 
They refuse to be bound by what others view as hard constraints.
```

On things being Out To Get You:

```markdown
Many things in this world are Out to Get You. Often they are Out to Get You for a lot, usually 
but not always your time, attention and money.

If you Get Got for compact amounts too often, it will add up and the constraints will bind.

If you Get Got even once for a non-compact amount, the cost expands until the you have no Slack 
left. The constraints bind you.

You might spend every spare minute and/or dollar on politics, advocacy or charity. You might think 
of every dollar as a fraction of a third-world life saved. Racing to find a cure for your daughter’s
cancer, you already work around the clock. You could have an all-consuming job or be a soldier 
marching off to war. It could be a quest for revenge, for glory, for love. Or you might spend every
spare minute mindlessly checking Facebook or obsessed with your fantasy football league.

You cannot relax. Your life is not your own.

It might even be the right choice! Especially for brief periods. When about to be run over by a truck
or evicted from your house, Slack is a luxury you cannot afford. Extraordinary times call for 
extraordinary effort.

Most times are ordinary. Make an ordinary effort.
```

Can you afford to lose Slack?

```markdown
No, you can’t. This is the most famous attack on Slack. Few words make me angrier.

The person who says “You Can Afford It” is saying to ignore constraints that do not bind you. If you 
do, all constraints soon bind you.

Those who do not value Slack soon lose it. Slack matters. Fight to keep yours!

Ask not whether you can afford it. Ask if it is Worth It.

Unless you can’t afford it. Affordability is invaluable negative selection. Never positive selection.

The You Can Afford It tax on Slack quickly approaches 100% if unchecked.

If those with extra resources are asked to share the whole surplus, all are poor or hide their wealth.
Wealth is a burden and makes you a target. Those visibly flush rush to spend their bounty.

Where those with free time are given extra work, all are busy or look busy. Those with copious free time
seek out relatively painless time sinks they can point to.

When looking happy means you deal with everything unpleasant, no one looks happy for long.
```

Venkat Rao's Maya Millennial is an example of someone who lacks Slack:

```markdown
Constraints bind her every action. Her job in life is putting up a front of the person she wants to 
show people that she wants to be. If her constraints noticeably failed to bind the illusion would fail.

Every action is being watched. If no one is around to watch her, the job falls to her. She must post 
all to Facebook, to Snapchat, to Instagram. Each action and choice signals who she is and her loyalty
to the system. Not doing that this time could mean missing her one chance to make it big.

Maya never has free time. There is signaling to do! At a minimum, she must spend such time on alert and
on her phone lest she miss something.

Maya never has spare cash. All must be spent to advance and fit her profile.

Maya lacks free speech, free association, free taste and free thought. All must serve.

Maya is in a world where she must signal she has no Slack. Slack means insufficient dedication and 
loyalty. Slack cannot be trusted. Slack now means slack later, which means failure. Future failure means 
no opportunity.
```

G Gordon Worley III comments on how Slack relates to distributed systems:

```markdown
If you work with distributed systems, by which I mean any system that must pass information between
multiple, tightly integrated subsystems, there is a well understood concept of maximum sustainable load
and we know that number to be roughly 60% of maximum possible load for all systems.

I don't have a link handy to show you the math, but the basic idea is that the probability that one 
subsystem will have to wait on another increases exponentially with the total load on the system and 
the load level that maximizes throughput (total amount of work done by the system over some period of
time) comes in just above 60%. If you do less work you are wasting capacity (in terms of throughput);
if you do more work you will gum up the works and waste time waiting even if all the subsystems are
always busy.

We normally deal with this in engineering contexts, but as is so often the case this property will hold 
for basically anything that looks sufficiently like a distributed system. Thus the "operate at 60% 
capacity" rule of thumb will maximize throughput in lots of scenarios: assembly lines, service-oriented
architecture software, coordinated work within any organization, an individual's work (since it is 
normally made up of many tasks that information must be passed between with the topology being spread
out over time rather than space), and perhaps most surprisingly an individual's mind-body.

"Slack" is a decent way of putting this, but we can be pretty precise and say you need ~40% slack to
optimize throughput: more and you tip into being "lazy", less and you become "overworked".
```

Some things that give Slack also take it away, per commenter elizabeth:

```markdown
The obvious example is cell phones. Especially at first they gave slack by letting you leave the house 
while you were waiting for an important phone call, but eventually ate it by creating an expectation 
that you'd always be available.
```

ialdabaoth contends that "this is because social structures strive to keep slack homeostatic at your level. As soon as you have more slack than you need to service your superiors in the social hierarchy, they will take that slack for themselves" but I'm not convinced of this argument. 

It's possible to have too much Slack -- I relate to this, as someone who's always subconsciously optimized for Slack myself. Per JacekLach:

```markdown
I often find myself with free time, and 'waste it away'. I don't really do anything on most weekends.
Having more constraints as guidance for behaviour in free time could likely remediate that; but I seem 
to be very good at talking myself out of any recurrent commitments, saying that they would reduce my 
freedom/flexibility/slack.

At the same time, it seems to me that I'm happiest, most 'alive', most in the 'flow', in situations with
exactly the kind of binding constraints this post talks of avoiding. The constraints focus you on the 
present, on the very moment, on being. For me this is clearest in sailing regattas - a clear purpose that
acts as a binding constraint (to go as fast as possible while staying safe - a safety margin does not for 
slack make, since you are not willing to ignore crossing it), consuming all your attention (at least during
the time you're responsible for the ship, and often more).

I suppose one can stretch the metaphor and say that having no slack on too many dimensions is likely to 
squash you; but having slack everywhere leaves you floating around aimlessly. Keeping most constraints 
slack and choosing only a couple aligned ones to bind against is possibly a way to find purpose.
```

Frustrated-demiurge talks about the same concept in her post [Affordance widths](https://frustrateddemiurge.tumblr.com/post/144927712238/affordance-widths). I *think* Venkat Rao talks about this same thing too in [this post](https://www.ribbonfarm.com/2019/03/07/mediocratopia-3/), except he comes at it from a different angle. 

```markdown
There is a paradox at the heart of mediocrity studies: excellence is not actually exceptional. If 
you see an excellent behavior or thing, it’s likely to be a middling instance at its level. The 
perception of exceptionalism is an illusion caused by inappropriate comparisons: you think it is a
99 percentile example of Level 3 performance, but it’s really a median example of Level 4 performance.

Changing levels of performance is self-disruption. The moment you hit, say, the 60% performance 
point on the current S-curve of learning, you start looking for ways to level up. This is the basic 
point in Daniel F. Chambliss’ classic paper, The Mundanity of Excellence. People who rise through 
the levels of a competitive sport do so by making discrete qualitative changes to level up before 
they hit diminishing returns from the current level. This process of leveling up, has less to do 
with striving for excellence in the sense of exceptional performance, and more to do with repeatedly
growing past limits. The visibly excellent are never at a local optimum.

In Age of Speed, skier Vince Poscente claims he won primarily by practicing his skills at a level 
above the one he was competing at. So during actual competition, he could win with less than 100% 
effort.

Making winning a habit is about making sure you’re always operating at a level where you have slack;
where you are in fact mediocre. If you’re being pushed towards excellence, it’s time to find a new 
level.
```

"Leveling up before hitting diminishing returns reminds me of another great essay I recently read, Eugene Wei's [Invisible Asymptotes](https://www.eugenewei.com/blog/2018/5/21/invisible-asymptotes) post from his blog [Remains of the Day](https://www.eugenewei.com/). It's pretty long, but full of great stuff. The relevant part is this:

```markdown
Every successful business goes through the famous S-curve, and most companies, and their investors,
spend a lot of time looking for that inflection point towards hockey-stick growth. But just as 
important, and perhaps less well studied, is that unhappy point later in the S-curve, when you hit
a shoulder and experience a flattening of growth. ...

For so many startups and even larger tech incumbents, the point at which they hit the shoulder in
the S-curve is a mystery, and I suspect the failure to see it occurs much earlier. The good thing is
that identifying the enemy sooner allows you to address it. We focus so much on product-market fit,
but once companies have achieved some semblance of it, most should spend much more time on the 
problem of product-market unfit.

For me, in strategic planning, the question in building my forecast was to flush out what I call the
invisible asymptote: a ceiling that our growth curve would bump its head against if we continued down
our current path. It's an important concept to understand for many people in a company, whether a CEO, 
a product person, or, as I was back then, a planner in finance. ...

An obvious problem for many companies, however, is that they are creating new types of businesses and 
services that don't lend themselves to easily identifying such invisible asymptotes. Many are not like
Amazon where there are readily tracked metrics like the size of the global book market with which to
peg their TAM (total addressable market).

Some of the limits to their growth are easier to spot than others. For messaging and some more general
social networking apps, for example, in many cases network effects are geographical. Since these apps 
build on top of real-world social graphs, and many of those are geographically clustered, there are 
winner-take-all dynamics such that in many countries one messaging app dominates, like Kakao in Korea 
or Line in Taiwan. There can be geo-political considerations, too, that help ensure that that WeChat 
will dominate in China to the exclusion of all competitors, for example.

For others, though, it takes a bit more product insight, and some might say intuition, to see the 
ceiling before you bump into it. For both employees and investors, understanding product-market unfit 
follows very closely on identifying product-market fit as an existential challenge.
```

<a name="#statistics"></a>

## Statistics
([overview](#overview))

<a name="#general-stats"></a>

### General stats
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

Deborah Mayo on Popper being too soft with conjectures:

```markdown
Although Popper's work is full of exhortations to put hypotheses through the wringer, to make them "suffer 
in our stead in the struggle for the survival of the fittest," the tests Popper sets out are white-glove 
affairs of logical analysis. If anomalies are approached with white gloves, it is little wonder that they 
seem to tell us only that there is an error somewhere and that they are silent about its source. We have 
to become shrewd inquisitors of errors, interact with them, simulate them (with models and computers), 
amplify them: we have to learn to make them talk.
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

<a name="#statistical-literacy"></a>

### Statistical literacy
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

<a name="#mathematical-maturity"></a>

## Math
([overview](#overview))

<a name="#solving-famous-open-problems"></a>

### How famous open problems get solved

From Terry Tao's post [Be sceptical of your own work](https://terrytao.wordpress.com/career-advice/be-sceptical-of-your-own-work/):

```markdown
Actual solutions to a major problem tend to be arrived at by a process more like the following (often 
involving several mathematicians over a period of years or decades, with many of the intermediate steps 
described here being significant publishable papers in their own right):

1. Isolate a toy model case x of major problem X.
2. Solve model case x using method A.
3. Try using method A to solve the full problem X.
4. This does not succeed, but method A can be extended to handle a few more model cases of X, such as 
x’ and x”.
5. Eventually, it is realised that method A relies crucially on a property P being true; this property is 
known for x, x’, and x”, thus explaining the current progress so far.
6. Conjecture that P is true for all instances of problem X.
7. Discover a family of counterexamples y, y’, y”, … to this conjecture. This shows that either method A 
has to be adapted to avoid reliance on P, or that a new method is needed.
8. Take the simplest counterexample y in this family, and try to prove X for this special case. Meanwhile, 
try to see whether method A can work in the absence of P.
9. Discover several counterexamples in which method A fails, in which the cause of failure can be 
definitively traced back to P. Abandon efforts to modify method A.
10. Realise that special case y is related to (or at least analogous to) a problem z in another field 
of mathematics. Look up the literature on z, and ask experts in that field for the latest perspectives on 
that problem.
11. Learn that z has been successfully attacked in that field by use of method B. Attempt to adapt method 
B to solve y.
12. After much effort, an adapted method B’ is developed to solve y.
13. Repeat the above steps 1-12 with A replaced by B’ (the outcome will of course probably be a little different 
from the sample storyline presented above). Continue doing this for a few years, until all model special cases 
can be solved by one method or another.
14. Eventually, one possesses an array of methods that can give partial results on X, each of having their 
strengths and weaknesses. Considerable intuition is gained as to the circumstances in which a given method 
is likely to yield something non-trivial or not.
15. Begin combining the methods together, simplifying the execution of these methods, locating new model 
problems, and/or finding a unified and clarifying framework in which many previous methods, insights, 
results, etc. become special cases.
16. Eventually, one realises that there is a family of methods A^* (of which A was the first to be discovered) 
which, roughly speaking, can handle all cases in which property P^* (a modern generalisation of property P) 
occurs. There is also a rather different family of methods B^* which can handle all cases in which Q^* occurs.
17. From all the prior work on this problem, all known model examples are known to obey either P^* or Q^*. 
Formulate Conjecture C: all cases of problem X obey either P^* or Q*^.
18. Verify that Conjecture C in fact implies the problem. This is a major reduction!
19. Repeat steps 1-18, but with problem X replaced by Conjecture C. (Again, the storyline may be different from 
that presented above.) This procedure itself may iterate a few times.
20. Finally, the problem has been boiled down to its most purified essence: a key conjecture K which (morally, 
at least) provides the decisive input into the known methods A^*, B^*, etc. which will settle conjecture C 
and hence problem X.
21. A breakthrough: a new method Z is introduced to solve an important special case of K.
22. The endgame: method Z is rapidly developed and extended, using the full power of all the intuition, experience, 
and past results, to fully settle K, then C, and then at last X.
23. The technology developed to solve major problem X is adapted to solve other related problems in the 
field. But now a natural successor question X’ to X arises, which lies just outside of the reach of the 
newly developed tools… and we go back to Step 1.
```

Greg Kuperberg stresses Terry’s point regarding “personal fallibility in the face of open problems”:

```markdown
If you think that you have solved an open problem, you should keep trying to understand it better for a 
while, because there is a good chance that you will find a mistake. This is still good advice even if it’s 
a run-of-the-mill open problem, not an incredibly hard open problem like Fermat’s Last Theorem.

Here is the sort of intuitive fallacy that can come up in a geometry argument: “If I lengthen all three 
sides of a triangle, its area will go up.” It sounds believable, and it even works in a few examples — but 
it’s not always true for obtuse triangles. Of course if you view this example in isolation, it seems 
boneheaded. But when working on an open problem, most people have to make intuitive leaps of this sort. If 
you think that you have a new result, that’s a great time to go back and debug your intuition at each step.

Terry also makes the more specific point that you should know the difference between climbing the mountain 
and marching around it. Restating a problem several times, or reducing it to another problem, is actually 
very good practice. But solving an open problem usually takes more than that. A few problems can be solved 
that way. Also, a few people have at times brilliantly transformed a broad set of problems by generalizing 
and restating them — this was Grothendieck’s work philosophy. But a more common outcome is that if you
restate a question too many times, eventually you will make it “easier” by restating it erroneously.

An example problem that can be solved almost entirely with restatement: Counting problems where the answer 
is the Catalan numbers, for example the number of lists of 2n balanced parentheses. However, this is only
medium-hard as counting problems go, and the restatements have to be somewhat clever to work.

An example where restatements are not known to work by themselves: Counting alternating-sign matrices, or 
ASMs. There are a dozen or so interesting-looking encodings of alternating-sign matrices. You can spend ages
rummaging through them in search of a simple counting principle to count ASMs. In fact, restatements of the
ASM problem have been important, for instance the description of ASMs in terms of square ice. But even the
important restatements do not solve this problem; rather they only give you access to substantive methods 
such as the Yang-Baxter equation.
```

(Tangent: I half-remember a discrete math HW assignment, a counting problem, regarding the number of lists of balanced parentheses. Puzzled for hours over that one until I thought of viewing it from (yet) another angle, after which it became much more tractable, if not exactly trivial. Point of view, as Alan Kay will tell you, is worth 80 IQ points; in this case the restatement I found was probably worth more like 10, but that was enough.)

Qiaochu asks:

```markdown
I’m quite curious – can you give an example where that process actually occurred, preferably multiple 
times? I’m not really aware of any resources for finding out the full story behind how a conjecture – 
especially not a particularly well-known, but still important, one – was proven, so I (and I hope others 
as well) would find such an example quite valuable.

Really the only good example I know of is the writeup of the Polymath project!
```

Terry’s response:

```markdown
Dear Qiaochu,

Actually most solutions to major problems (e.g. Poincare conjecture, Fermat’s last theorem, etc.) have 
this sort of history – a painstaking series of explorations, conjectures, setbacks, steady accumulation
of intuition and insights, realisation of the naivete of earlier approaches, etc. It is indeed difficult
though to find a coherent narrative for any given one of these problems (except perhaps at conference 
talks, or an advanced survey article); usually the story is spread throughout a dozen papers, and one has
to have a fair amount of familiarity with the problem to really appreciate the unfolding of progress.

For some problems, though, there are some good surveys that focus on exactly this sort of narrative, e.g.
Goldston-Pintz-Yildirim’s “The path to recent progress on small gaps between primes”. Milnor’s Clay article 
on the Poincare conjecture covers the topological phase of the attacks on that problem fairly well, and 
the important discovery of the geometrisation conjecture, though it is rather light on the Ricci flow approach 
which is of course at the heart of Perelman’s solution (but it is fair to say that this geometric approach 
would only have been seriously attempted after it became abundantly clear that the topological methods had 
fallen quite short of what was needed to settle the conjecture). Morgan’s BAMS survey article on the subject 
covers the latter quite thoroughly, though the focus is more on the technical details than on the development
of ideas. Finally, I discuss the narrative surrounding Szemeredi’s theorem in my article “What is good 
mathematics?” (linked to on the sidebar of this blog).
```

<a name="#mathematical-maturity"></a>

### Mathematical maturity

([overview](#overview))

From Redditor [man_after_midnight](https://www.reddit.com/user/man_after_midnight), answering Mathematicians of Reddit: [Is there some point where you see a big picture and everything "clicks"?](https://www.reddit.com/r/math/comments/1mtian/mathematicians_of_reddit_is_there_some_point/):

```markdown
The way it was described to me when I was in high school was in terms of 'levels'.

Sometimes, in your mathematics career, you find that your slow progress, and careful accumulation of tools 
and ideas, has suddenly allowed you to do a bunch of new things that you couldn't possibly do before. Even 
though you were learning things that were useless by themselves, when they've all become second nature, a 
whole new world of possibility appears. You have "leveled up", if you will. Something clicks, but now there 
are new challenges, and now, things you were barely able to think about before suddenly become critically 
important.

It's usually obvious when you're talking to somebody a level above you, because they see lots of things 
instantly when those things take considerable work for you to figure out. These are good people to learn 
from, because they remember what it's like to struggle in the place where you're struggling, but the things 
they do still make sense from your perspective (you just couldn't do them yourself).

Talking to somebody two or levels above you is a different story. They're barely speaking the same language, 
and it's almost impossible to imagine that you could ever know what they know. You can still learn from them, 
if you don't get discouraged, but the things they want to teach you seem really philosophical, and you don't 
think they'll help you—but for some reason, they do.

Somebody three levels above is actually speaking a different language. They probably seem less impressive to 
you than the person two levels above, because most of what they're thinking about is completely invisible to 
you. From where you are, it is not possible to imagine what they think about, or why. You might think you can, 
but this is only because they know how to tell entertaining stories. Any one of these stories probably contains 
enough wisdom to get you halfway to your next level if you put in enough time thinking about it.

What follows is my rough opinion on how this looks in a typical path towards a Ph.D. in math. Obviously this 
is rather subjective, and makes math look too linear, but I think it's a useful thought experiment.

Consider the change that a person undergoes in first mastering elementary algebra. Let's say that that's one 
level. This student is now comfortable with algebraic manipulation and the idea of variables.

The next level may come somewhere during a first calculus course. The student now understands the concept of 
the infinitely small, of slope at a point, and can reason about areas, physical motion, and optimization.

Many stop here, believing that they have finally learned math. Those who do not stop, might proceed through 
multivariable calculus and perhaps a basic linear algebra course with the tools they currently possess. Their 
next level comes when they find themselves suffering through an abstract algebra course, and have to once 
again reshape their whole thought process just to squeak by with a C.

Once this student masters all of that, the rest of the undergraduate curriculum at their university might be a 
breeze. But not so with graduate school. They gain a level their first year. They gain another their third year. 
And they are horrified to discover that they are expected to gain a third level before they graduate. This 
level is the hardest of them all, because it is the first one that consists in mastering material that has been 
created largely by the student.

I don't know how many levels there are after that. At least three.

So, the bad news is, you never do see the whole picture (though you see the old picture shrink down to a tiny 
point), and you can't really explain what you do see. But the good news is that the world of mathematics is so 
rich and exciting and wonderful that even your wildest dreams about it cannot possibly compare. It is not like 
seeing the Matrix—it is like seeing the Matrix within the Matrix within the Matrix within the Matrix within the
Matrix.
```

John Baez shared it on Google+ and [added](https://plus.google.com/+johncbaez999/posts/36g9jx54nni):

```markdown
As he points out, this talk of 'levels' is too linear. You can be much better at algebraic geometry than 
your friend, but way behind them in probability theory. Or even within a field like algebraic geometry, 
you might be able to understand sheaf cohomology better than your friend, yet still way behind in some 
classical topic like elliptic curves.

To have worthwhile conversations with someone who is not evenly matched with you in some subject, it's 
often good for one of you to play 'student' while the other plays 'teacher'. Playing teacher is an ego 
boost, and it helps organize your thoughts - but playing student is a great way to amass knowledge and 
practice humility... and a good student can help the teacher think about things in new ways.

Taking turns between who is teacher and who is student helps keep things from becoming unbalanced. And it's 
especially fun when some subject can only be understood with the combined knowledge of both players.

I have a feeling good mathematicians spend a lot of time playing these games - we often hear of famous 
teams like Atiyah, Bott and Singer, or even bigger ones like the French collective called 'Bourbaki'. For 
about a decade, I played teacher/student games with James Dolan, and it was really productive. I should 
probably find a new partner to learn the new kinds of math I'm working on now. Trying to learn things by 
yourself is a huge disadvantage if you want to quickly rise to higher 'levels'.
```

I also found Baez’s comment on how this relates to his experience ‘preaching’ category theory to ‘the masses’ interesting:

```markdown
To me category theory seems like a great branch of math for seeing how people climb up levels. Perhaps 
this because I've studied it a bunch and know a lot of people who think about it. But perhaps it's also 
because category theory is extremely conceptual, so lots of things of things seem obvious when you 
understand them, with no need for calculation to prove them - just a verbal argument will do - while the 
same verbal arguments seem cryptic and baffling before you understand them.

The point is that one needs to really understand the concepts used in these verbal arguments. One puts 
in a lot of sweat to understand them, but after one has, one can often use them with an ease that seems 
magical to people at lower levels. This is probably why lots of people get annoyed with category 
theorists, calling them 'too abstract'.

But it's also good to remember that category theory is just one portion of math, so people at a high 
level in category theory can still be embarrassingly clueless and awkward in other branches of math.
```

And to Toby Bartels’ suggestion that these ‘levels’ consist mostly of increasing abstraction:

```markdown
There are importantly different levels of competence in doing mathematics other than levels of 
abstraction: for example, levels of skill in devising proofs, levels of skill in inventing research 
program, and levels of understanding the 'big picture' of mathematics: what the big problems are and 
why they're interesting.

I often run into freshly-minted category theory postdocs who initially impress me with their ability 
to throw around (infinity,1)-categories, stacks, topoi and the like... but then amuse me because they 
don't know enough math to apply these concepts in powerful ways, or even understand where they fit into 
the grand scheme of things. They just haven't had time to learn the logic, algebra, topology, geometry, 
analysis, physics, and so on that these abstract concepts were designed to help us with. So they may 
seem superficially to be at a 'high level', but in a lot of ways they're not. (I don't think 'level' is 
quite the right word for what I mean, since it's too linear.)
```

Gary Ray R on how it pertains to engineering:

```markdown
I think the idea of levels also applies to Mechanical Engineering. I remember really having difficulty 
with Thermodynamics. I spent hours and hours on the homework, and never though I got any better, I was 
so happy with a B-. At the end of the course the instructor asked if I wanted to be his TA and grader 
for the next year. I was flummoxed, me, I just barely got this stuff. He said, you can do it. Well the 
next year I graded Thermo and that was one of the very hardest things in my engineering studies. But I 
jumped a level and did not really realize it.

Later when I went back for grad school in Materials Engineering, the Thermo seemed so easy, I was surprised 
at what I was so hard now seemed so clear. I could explain almost anything with Gibbs Free Energy, and 
the math was not that hard. But the concept took a while to sink in.
```

<a name="#good-mathematics"></a>

### Good mathematics
([overview](#overview))

From Terry Tao's paper [What is good mathematics?](https://arxiv.org/pdf/math/0702396.pdf):

```markdown
There are many different types of mathematics which could be designated “good”. For instance, “good 
mathematics” could refer (in no particular order) to

(i) Good mathematical problem-solving (e.g. a major breakthrough on an important mathematical problem);
(ii) Good mathematical technique (e.g. a masterful use of existing methods, or the development of 
new tools);
(iii) Good mathematical theory (e.g. a conceptual framework or choice of notation which systematically 
unifies and generalises an existing body of results);
(iv) Good mathematical insight (e.g. a major conceptual simplification, or the realisation of a unifying
principle, heuristic, analogy, or theme);
(v) Good mathematical discovery (e.g. the revelation of an unexpected and intriguing new mathematical 
phenomenon, connection, or counterexample);
(vi) Good mathematical application (e.g. to important problems in physics, engineering, computer science,
statistics, etc., or from one field of mathematics to another);
(vii) Good mathematical exposition (e.g. a detailed and informative survey on a timely mathematical topic,
or a clear and well-motivated argument);
(viii) Good mathematical pedagogy (e.g. a lecture or writing style which enables others to learn and do
mathematics more effectively, or contributions to mathematical education);
(ix) Good mathematical vision (e.g. a long-range and fruitful program or set of conjectures);
(x) Good mathematical taste (e.g. a research goal which is inherently interesting and impacts important
topics, themes, or questions);
(xi) Good mathematical public relations (e.g. an effective showcasing of a mathematical achievement to 
non-mathematicians, or from one field of mathematics to another);
(xii) Good meta-mathematics (e.g. advances in the foundations, philosophy, history, scholarship, or
practice of mathematics);
(xiii) Rigorous mathematics (with all details correctly and carefully given in full);
(xiv) Beautiful mathematics (e.g. the amazing identities of Ramanujan; results which are easy (and pretty) 
to state but not to prove);
(xv) Elegant mathematics (e.g. Paul Erd˝os’ concept of “proofs from the Book”; achieving a difficult 
result with a minimum of effort);
(xvi) Creative mathematics (e.g. a radically new and original technique, viewpoint, or species of result);
(xvii) Useful mathematics (e.g. a lemma or method which will be used repeatedly in future work on the subject);
(xviii) Strong mathematics (e.g. a sharp result that matches the known counterexamples, or a result 
which deduces an unexpectedly strong conclusion from a seemingly weak hypothesis);
(xix) Deep mathematics (e.g. a result which is manifestly non-trivial, for instance by
capturing a subtle phenomenon beyond the reach of more elementary tools);
(xx) Intuitive mathematics (e.g. an argument which is natural and easily visualisable);
(xxi) Definitive mathematics (e.g. a classification of all objects of a certain type; the final word on
a mathematical topic); etc.

As the above list demonstrates, the concept of mathematical quality is a highdimensional one, and lacks an
obvious canonical total ordering. I believe this is because mathematics is itself complex and high-dimensional,
and evolves in unexpected and adaptive ways; each of the above qualities represents a different way in which we
as a community improve our understanding and usage of the subject. There does not appear to be universal
agreement as to the relative importance or weight of each of the above qualities. This is partly due to tactical
considerations: a field of mathematics at a given stage of development may be more receptive to one approach to 
mathematics than another. It is also partly due to cultural considerations: any given field or school of
mathematics tends to attract like-minded mathematicians who prefer similar approaches to a subject. It also 
reflects the diversity of mathematical ability; different mathematicians tend to excel in different mathematical 
styles, and are thus well suited for different types of mathematical challenges.
```

This multifaceted nature of "good math" is healthy for math as a whole, since desirable traits can be detrimental to a field if pursued at the expense of others, per the following (made up) scenarios:

```markdown
• A field which becomes increasingly ornate and baroque, in which individual
results are generalised and refined for their own sake, but the subject as a
whole drifts aimlessly without any definite direction or sense of progress;
• A field which becomes filled with many astounding conjectures, but with no
hope of rigorous progress on any of them;
• A field which now consists primarily of using ad hoc methods to solve a collection
of unrelated problems, which have no unifying theme, connections, or purpose;
• A field which has become overly dry and theoretical, continually recasting and
unifying previous results in increasingly technical formal frameworks, but not
generating any exciting new breakthroughs as a consequence; or
• A field which reveres classical results, and continually presents shorter, simpler,
and more elegant proofs of these results, but which does not generate any truly
original and new results beyond the classical literature.
```

<a name="#what-every-mathematician-should-know"></a>

### What every mathematician should know
([overview](#overview))

Timothy Chow is well worth reading. Here's his answer to the MO question [How has "what every mathematician should know" changed?](https://mathoverflow.net/questions/19356/how-has-what-every-mathematician-should-know-changed?rq=1):

```markdown
I believe that one shift is that "what every mathematician should know" is nowadays much less a 
specific body of mathematical facts and much more a facility with navigating the ocean of mathematical
knowledge.

For example, I might not need to have advanced computer programming skills, but I do need to have some
sense of what kinds of computations are feasible and when it is appropriate for me to do a computation.

I might not need to hold in my head everything that is known about a certain topic, even if that topic 
is close to my area of specialization, but I definitely need to have the ability to search the literature,
assess what is in a certain paper that my search turns up, and know when I should ask an expert and how 
to formulate a targeted question to ask.

Similarly, I might not need detailed knowledge of fields (seemingly) distant from my own, but I do need 
to be able to discern when those distant fields might provide relevant tools for my own work.

So far I have been focusing on what a mathematician needs to know in order to be an effective researcher.
However, the phrase "what every mathematician should know" carries overtones of what one should know if 
one wants to earn a reputation for being an educated, knowledgeable, respectable, and attractive 
representative of the profession. In my opinion this is quite a different question. For this, you need to
be fluent in the language of the hot topics du jour, and au courantwith flashy announcements of big
breakthroughs in all areas of mathematics. While there's some correlation between this kind of knowledge
and the knowledge I discussed above, I find it questionable whether, literally speaking, every 
mathematician should have it.
```

Here he echoes Barry Mazur, whose [writing on the subject](http://www.math.harvard.edu/~mazur/preprints/math_ed_2.pdf) is so beautiful and fulfilling I can't help but reproduce large parts of it wholesale here. 

Lingua franca, unifiers, ubiquitous:

```markdown
Certain fields of mathematics, at certain times, play the role of lingua franca in the sense that
mathematics from vastly different fields get formulated in the vocabulary, the terminology, or even 
more strikingly in the conceptual framework of that specific field. Weierstrass’s theory of functions,
Cantor’s Set Theory and Group Theory have played (and continue to play) such a role; the vocabulary 
of Category Theory has permeated disparate disciplines. These are some of the grand forces in mathematics
that shape our way of communicating to one another. Other fields formulate powerful viewpoints, templates,
that cross over to distant disciplines–let’s call these fields unifiers. Algebraic Topology has done 
service as a unifier, as has large aspects of Algebraic Geometry. Other fields are so ubiquitous that 
they cast light on all other disciplines of mathematics: measure theory, probability and statistics
come to mind; perhaps aspects of combinatorics.

In any epoch there will be the lingua franca, the unifiers and the ubiquitous of that epoch. A young
(or an old) mathematician, of no matter what specialty, would do well to be acquainted—at least a tiny
bit acquainted—with the mathematical goings-on in these fields. So which fields are of that sort these days?
```

Critical mass of learned info causing phase shift in POV of entire subject:

```markdown
Before offering a concrete list of good “fields of acquaintance” I want to convey an idea of a friend
of mine, who is a student of European History. He tells me that at one point in his career studying
European History, he experienced an abrupt phase shift. Once you’ve achieved—says my friend—a certain 
critical mass of historical information, all of a sudden your view of the entire subject changes. First,
your power of simply retaining information increases multifold; but more importantly, your way of thinking 
about the subject bears no relation to the way you approached things initially. My friend accounted for 
this surprising moment as a consequence of accumulation, perhaps to overload, of somehow-connected specifics
that forced him to involuntarily re-configure—in a more meaningful way— his modes of organization, and 
contemplation, of the entirety of this corpus of knowledge.

Well, it would be interesting if we could put our finger on the critical moments, the phase shifts—if they 
exist—in our mathematical education. If they do exist they may depend less on our having devoured any 
specific collection of mathematical ideas, and more on our having exposed ourselves to some un-specifiable
critical mass. With this in mind, I’ll end, below, with a list that nowadays, in my opinion, stands for 
“fields of acquaintance” any critical mass of them being a good choice for a good mathematical education.
```

A broad mathematical education should help a person achieve a predilection for the four (most classical, significantly overlapping) aspects of mathematical thought — Geometry, Algebra, Computation, and The mathematical intuition(s) derived from Physics — which aren’t the same as the traditional subject classifications, but rather should be thought of as highly developed ‘intuitions’:

```markdown
I say that these are “overlapping,’ but in reality, what makes mathematics one subject is that nothing 
that we do is entirely contained in one of these categories: they seem to stand for distinct intuitions,
and have given rise to distinct realms of thought, and yet they are inseparably welded together. These four
categories have been fused together so substantially in recent times that it may even be misleading to keep
bringing them up. For there are subjects of great importance such as the theory of modular (or automorphic) 
forms that defy this categorization completely, since they stretch their substance, their tools, and the 
intuition they rely on over all four of these items.

Nevertheless, Geometry, Algebra, Computation, and Mathematical Physics represent a recognizable, if wobbly, 
partition of mathematical sensibilities. Let us consider them as motivating intuitions rather than fixed 
repositories of knowledge; i.e., as fundamental types of highly developed senses that some mathematicians
enjoy: there are people with strong geometric intuitions; there are those with strong algebraic intuitions;
there are those who are very sensitive to various aspects of computation and estimation and then there are 
the lucky people who also bring into the mix some basic physical intuition. I also think that we all understand
what it means for some mathematician to have any one of these gifts—whether or not we ourselves possess it.

So, a broad mathematical education should, perhaps, aim to help a person achieve (at least somewhat) a 
predilection for each of these ways of thinking. I would like to view each of these intuitions as “core” 
rather than any particular conglomeration of subject matter as core.

In response to an earlier draft, David Mumford asked me where I would put the traditional, and grand, subject 
of Analysis in this classification, Analysis being a subject dealing with intuitions as fundamental as time, 
change, and continuity; my feeling is that the subject is so many-dimensional that it derives its inspiration
and intuitions from every, or any, direction: when you say that someone is a strong analyst, you might mean 
that this person has a keen sense of a priori estimates in PDE, which I would tag as computation and estimation;
or you might be talking of a good complex analyst dealing with dynamical systems which I would tag as geometry,
etc. I would probably want to spread Analysis over all four categories.
```

The four intuitions, “today’s list” per Mazur:

```markdown
• Geometry-in the broad sense: This can be experienced in so many different ways that any one person’s 
“critical mass” will be disjoint from another person’s. Our sense of geometry might go from knot theory
to differential geometry (and the related analysis; e.g., the spectrum of the Laplacian) to classification
of n-dimensional manifolds to symplectic geometry to dynamical systems to sphere-packing to fixed point
theorems to K-theory to systems of elliptic PDE’s in the large to the Index Theorem to Bott periodicity
to the homotopy groups of spheres. . . and here we would be moving into the more algebraic realms of 
algebraic topology, which nowadays is also commingling with algebraic geometry.

• Algebra-in the broad sense. This includes the ubiquitous notion of groups (say; finite, finitely presented,
Lie, algebraic, arithmetic, and adelic) and their linear and projective (finite- and infinite-dimensional)
representations. It includes elementary aspects of any of the subjects with “algebraic” as an adjective in
their name: algebraic topology, algebraic geometry, and algebraic number theory. It includes the entire 
basic vocabulary of very general languages such as category theory and more specific languages of use in 
traditional functional analysis such as the theory of Hilbert and Banach spaces.

• Computation–in the broad sense. This stretches from machine computation, algorithms, numerical analysis, 
estimation, and statistics, to combinatorics, analysis and probability; i.e., ways of dealing with data,
practically and/or theoretically.

• Mathematics related to Physics. Newtonian Mechanics, Optics, Maxwell’s Equations, Relativity, some Quantum
Mechanics and some physics related to field theories and string theory; and—of course—the mathematics that 
connects to this.
```

<a name="#general-intelligence"></a>

## General intelligence
([overview](#overview))

<a name="#logi"></a>

### *Levels of Organization in General Intelligence*

Here are some interesting passages from Eliezer Yudkowsky’s paper [Levels of Organization in General Intelligence](https://intelligence.org/files/LOGI.pdf).

On the what and why of intelligence:

```markdown
Intelligence is an evolutionary advantage because it enables us to model, predict, and manipulate reality. 
Evolutionary problems are not limited to stereotypical ancestral contexts such as fleeing lions or chipping 
spears; our intelligence includes the ability to model social realities consisting of other humans, and the 
ability to predict and manipulate the internal reality of the mind.

Philosophers of the mind sometimes define “knowledge” as cognitive patterns that map to external reality 
(Newell 1980), but a surface mapping has no inherent evolutionary utility. Intelligence requires more than 
passive correspondence between internal representations and sensory data, or between sensory data and reality. 
Cognition goes beyond passive denotation; it can predict future sensory data from past experience. Intelligence 
requires correspondences strong enough for the organism to choose between futures by choosing actions on the 
basis of their future results.

Intelligence in the fully human sense requires the ability to manipulate the world by reasoning backward from a 
mental image of the desired outcome to create a mental image of the necessary actions. (In Section 2, these 
ascending tests of ability are formalized as sensory, predictive, decisive, and manipulative bindings between a 
model and a referent.)
```

On the evolution of complex adaptations in general, and of intelligence in particular:

```markdown
A new adaptation requiring the presence of a previous adaptation cannot spread unless the prerequisite 
adaptation is present in the genetic environment with sufficient statistical regularity to make the new 
adaptation a recurring evolutionary advantage. Evolution uses existing genetic complexity to build new genetic 
complexity, but evolution exhibits no foresight. Evolution does not construct genetic complexity unless it 
is an immediate advantage, and this is a fundamental constraint on accounts of the evolution of complex systems.

Complex functional adaptations—adaptations that require multiple genetic features to build a complex 
interdependent system in the phenotype—are usually, and necessarily, universal within a species. Independent 
variance in each of the genes making up a complex interdependent system would quickly reduce to insignificance 
the probability of any phenotype possessing a full functioning system. To give an example in a simplified world, 
if independent genes for “retina,” “lens,” “cornea,” “iris,” and “optic nerve” each had an independent 20% 
frequency in the genetic population, the random-chance probability of any individual being born with a complete 
eyeball would be 3125:1.

…Because evolution lacks foresight, complex functions cannot evolve unless their prerequisites are evolutionary 
advantages for other reasons. The human evolutionary line did not evolve toward general intelligence; rather, 
the hominid line evolved smarter and more complex systems that lacked general intelligence, until finally the 
cumulative store of existing complexity contained all the tools and subsystems needed for evolution to stumble 
across general intelligence. Even this is too anthropocentric; we should say rather that primate evolution 
stumbled across a fitness gradient whose path includes the subspecies Homo sapiens sapiens, which subspecies 
exhibits one particular kind of general intelligence.
```

On AI being “not like” physics:

```markdown
I am admittedly biased against the search for a “single essence” of intelligence; I believe that the search for 
a single essence of intelligence lies at the center of AI’s previous failures. Simplicity is the grail of physics, 
not AI. Physicists win Nobel Prizes when they discover a previously unknown underlying layer and explain its 
behaviors. We already know what the ultimate bottom layer of an Artificial Intelligence looks like; it looks like 
ones and zeroes. Our job is to build something interesting out of those ones and zeroes. The Turing formalism does 
not solve this problem any more than quantum electrodynamics tells us how to build a bicycle; knowing the abstract 
fact that a bicycle is built from atoms doesn’t tell you how to build a bicycle out of atoms—which atoms to use and 
where to put them. Similarly, the abstract knowledge that biological neurons implement human intelligence does not 
explain human intelligence. The classical hype of early neural networks, that they used “the same parallel 
architecture as the human brain,” should, at most, have been a claim of using the same parallel architecture as an 
earthworm’s brain. (And given the complexity of biological neurons, the claim would still have been wrong.)
```

Or as Tooby and Cosmides (1992) put it:

```markdown
The science of understanding living organization is very different from physics or chemistry, where parsimony makes 
sense as a theoretical criterion. The study of organisms is more like reverse engineering, where one may be dealing 
with a large array of very different components whose heterogenous organization is explained by the way in which 
they interact to produce a functional outcome. Evolution, the constructor of living organisms, has no privileged 
tendency to build into designs principles of operation that are simple and general.
```

Here’s the more obvious kind of “physics envy” in AI:

```markdown
The field of Artificial Intelligence suffers from a heavy, lingering dose of genericity and black-box, blank-slate, 
tabula-rasa concepts seeping in from the Standard Social Sciences Model (SSSM) identified by Tooby and Cosmides 
(1992). The general project of liberating AI from the clutches of the SSSM is more work than I wish to undertake in 
this paper, but one problem that must be dealt with immediately is physics envy. The development of physics over the 
last few centuries has been characterized by the discovery of unifying equations which neatly underlie many complex 
phenomena. Most of the past fifty years in AI might be described as the search for a similar unifying principle 
believed to underlie the complex phenomenon of intelligence.

Physics envy in AI is the search for a single, simple underlying process, with the expectation that this one discovery 
will lay bare all the secrets of intelligence. The tendency to treat new approaches to AI as if they were new theories 
of physics may at least partially explain AI’s past history of overpromise and oversimplification. Attributing all 
the vast functionality of human intelligence to some single descriptive facet—that brains are “parallel,” or 
“distributed,” or “stochastic”; that minds use “deduction” or “induction”— results in a failure (an overhyped failure) 
as the project promises that all the functionality of human intelligence will slide out from some simple principle.
```

And here’s the more subtle one:

```markdown
The effects of physics envy can be more subtle; they also appear in the lack of interaction between AI projects. 
Physics envy has given rise to a series of AI projects that could only use one idea, as each new hypothesis for 
the one true essence of intelligence was tested and discarded.

Douglas Lenat’s AM and Eurisko programs (Lenat 1983)—though the results were controversial and may have been mildly 
exaggerated (Ritchie and Hanna 1984)—used nonetheless very intriguing and fundamental design patterns to deliver 
significant and unprecedented results. Despite this, the design patterns of Eurisko, such as self-modifying 
decomposable heuristics, have seen almost no reuse in later AIs. Even Lenat’s subsequent Cyc project (Lenat, Prakash, 
and Shepherd 1985) apparently does not reuse the ideas developed in Eurisko.

From the perspective of a modern-day programmer, accustomed to hoarding design patterns and code libraries, the 
lack of crossfertilization is a surprising anomaly. One would think that self-optimizing heuristics would be useful 
as an external tool, e.g. for parameter tuning, even if the overall cognitive architecture did not allow for the 
internal use of such heuristics.
```

A related point:

```markdown
Leaving out key design elements, without replacement, on the basis of the mistaken belief that they are not 
relevant to general intelligence, is an error that displays a terrifying synergy with “physics envy.” In extreme 
cases—and most historical cases have been extreme—the design ignores everything about the human mind except one 
characteristic (logic, distributed parallelism, fuzziness, etc.), which is held to be “the key to intelligence.” 
(On my more pessimistic days I sometimes wonder if successive fads are the only means by which knowledge of a 
given feature of human intelligence becomes widespread in AI.)
```

On the importance of emphasizing (the right kind of) “supersystem design” in developing general intelligence:

```markdown
I argue strongly for “supersystems,” but I do not believe that “supersystems” are the necessary and sufficient 
Key to AI. General intelligence requires the right supersystem, with the right cognitive subsystems, doing the 
right things in the right way. Humans are not intelligent by virtue of being “supersystems,” but by virtue of 
being a particular supersystem which implements human intelligence. I emphasize supersystem design because I 
believe that the field of AI has been crippled by the wrong kind of simplicity—a simplicity which, as a design 
constraint, rules out workable designs for intelligence; a simplicity which, as a methodology, rules out 
incremental progress toward an understanding of general intelligence; a simplicity which, as a viewpoint, renders 
most of the mind invisible except for whichever single aspect is currently promoted as the Key to AI.
```

On the need to focus on, not design simplicity, but “sufficiently complex explanations” and “usefully deep designs”:

```markdown
If the quest for design simplicity is to be “considered harmful,” what should replace it? I believe that rather 
than simplicity, we should pursue sufficiently complex explanations and usefully deep designs. In ordinary 
programming, there is no reason to assume a priori that the task is enormously large. In AI the rule should be 
that the problem is always harder and deeper than it looks, even after you take this rule into account.

Knowing that the task is large does not enable us to meet the challenge just by making our designs larger or more 
complicated; certain specific complexity is required, and complexity for the sake of complexity is worse than 
useless. Nonetheless, the presumption that we are more likely to underdesign than overdesign implies a different 
attitude towards design, in which victory is never declared, and even after a problem appears to be solved, we go 
on trying to solve it.

If this creed were to be summed up in a single phrase, it would be: “Necessary but not sufficient.” In accordance 
with this creed, it should be emphasized that supersystems thinking is only one part of a larger paradigm, and that 
an open-ended design process is itself “necessary but not sufficient.” These are first steps toward AI, but not 
the only first steps, and certainly not the last steps.
```

On his candidate for “the most debilitating mistake in AI”:

```markdown
If I had to pick one single mistake that has been the most debilitating in AI, it would be implementing a process 
too close to the token level—trying to implement a high-level process without implementing the underlying layers 
of organization. Many proverbial AI pathologies result at least partially from omitting lower levels of 
organization from the design.

Take, for example, that version of the “frame problem”—sometimes also considered a form of the “commonsense 
problem”—in which intelligent reasoning appears to require knowledge of an infinite number of special cases. 
Consider a CPU which adds two 32-bit numbers. The higher level consists of two integers which are added to produce 
a third integer. On a lower level, the computational objects are not regarded as opaque “integers,” but as ordered 
structures of 32 bits. When the CPU performs an arithmetic operation, two structures of 32 bits collide, under 
certain rules which govern the local interactions between bits, and the result is a new structure of 32 bits. Now 
consider the woes of a research team, with no knowledge of the CPU’s underlying implementation, that tries to 
create an arithmetic “expert system” by encoding a vast semantic network containing the “knowledge” that two and 
two make four, twenty-one and sixteen make thirty-seven, and so on. This giant lookup table requires eighteen 
billion billion entries for completion. 

In this hypothetical world where the lower-level process of addition is not 
understood, we can imagine the “common-sense” problem for addition; the launching of distributed Internet projects 
to “encode all the detailed knowledge necessary for addition”; the frame problem for addition; the philosophies of 
formal semantics under which the LISP token thirty-seven is meaningful because it refers to thirty-seven objects in 
the external world; the design principle that the token thirty-seven has no internal complexity and is rather given 
meaning by its network of relations to other tokens; the “number grounding problem”; the hopeful futurists arguing 
that past projects to create Artificial Addition failed because of inadequate computing power; and so on.
```

On the difference between human-written programs and computation in neurons:

```markdown
Another class of problem stems from “porting” across the extremely different programming styles of evolution 
versus human coding. Human-written programs typically involve a long series of chained dependencies that intersect 
at single points of failure— “crystalline” is a good term to describe most human code. Computation in neurons 
has a different character. Over time our pictures of biological neurons have evolved from simple integrators of 
synaptic inputs that fire when a threshold input level is reached, to sophisticated biological processors with 
mixed analog-digital logics, adaptive plasticity, dendritic computing, and functionally relevant dendritic and 
synaptic morphologies (Koch and Segev 2000). What remains true is that, from an algorithmic perspective, neural 
computing uses roughly arithmetical operations14 that proceed along multiple intertwining channels in which 
information is represented redundantly and processed stochastically. Hence, it is easier to “train” neural 
networks—even nonbiological connectionist networks—than to train a piece of human-written code. Flipping a random 
bit inside the state of a running program, or flipping a random bit in an assembly-language instruction, has a 
much greater effect than a similar perturbation of a neural network. For neural networks the fitness landscapes 
are smoother. Why is this? Biological neural networks need to tolerate greater environmental noise (data error) 
and processor noise (computational error), but this is only the beginning of the explanation.

Smooth fitness landscapes are a useful, necessary, and fundamental outcome of evolution. Every evolutionary 
success starts as a mutation—an error—or as a novel genetic combination. A modern organism, powerfully adaptive 
with a large reservoir of genetic complexity, necessarily possesses a very long evolutionary history; that is, 
the genotype has necessarily passed through a very large number of successful mutations and recombinations along 
the road to its current form… “Smooth fitness landscapes” imply, among other things, that a small perturbation in 
the program code (genetic noise), in the input (environmental noise), or in the state of the executing program 
(processor noise), is likely to produce at most a small degradation in output quality. In most human-written code, 
a small perturbation of any kind usually causes a crash. Genomes are built by a cumulative series of point 
mutations and random recombinations. Human-written programs start out as high-level goals which are translated, 
by an extended serial thought process, into code. A perturbation to human-written code perturbs the code’s final 
form, rather than its first cause, and the code’s final form has no history of successful mutation. The thoughts 
that gave rise to the code probably have a smooth fitness metric, in the sense that a slight perturbation to the 
programmer’s state of mind will probably produce code that is at most a little worse, and possibly a little better. 
Human thoughts, which are the original source of human-written code, are resilient; the code itself is fragile.
```

On why we’re trichromats, and not (say) tetrachromats like mantis shrimp (I honestly thought this was one of those unanswerable anthropic-style questions, so it was pretty surprising to find a naturalistic non-anthropic-flavored explanation):

```markdown
Among other questions, Roger Shepard’s truly elegant paper “The Perceptual Organization of Colors” seeks to answer 
the question of trichromancy: Why are there three kinds of cones in the human retina, and not two, or four? Why is 
human visual perception organized into a three-dimensional color space? Historically, it was often theorized that 
trichromancy represented an arbitrary compromise between chromatic resolution and spatial resolution; that is, 
between the number of colors perceived and the grain size of visual resolution. As it turns out, there is a more 
fundamental reason why three color channels are needed.

To clarify the question, consider that surfaces possess a potentially infinite number of spectral reflectance 
distributions. We will focus on spectral reflectance distributions, rather than spectral power distributions, 
because adaptively relevant objects that emit their own light are environmentally rare. Hence the physically 
constant property of most objects is the spectral reflectance distribution, which combines with the spectral power 
distribution of light impinging on the object to give rise to the spectral power distribution received by the human 
eye. The spectral reflectance distribution is defined over the wavelengths from 400 nm to 700 nm (the visible range), 
and since wavelength is a continuum, the spectral reflectance distribution can theoretically require an unlimited 
number of quantities to specify. Hence, it is not possible to exactly constrain a spectral reflectance distribution 
using only three quantities, which is the amount of information transduced by human cones.

The human eye is not capable of discriminating among all physically possible reflecting surfaces. However, it is 
possible that for “natural” surfaces—surfaces of the kind commonly encountered in the ancestral environment—reflectance 
for each pure frequency does not vary independently of reflectance for all other frequencies. For example, there might 
exist some set of basis reflectance functions, such that the reflectance distributions of almost all natural surfaces 
could be expressed as a weighted sum of the basis vectors. If so, one possible explanation for the trichromancy of 
human vision would be that three color channels are just enough to perform adequate discrimination in a “natural” color 
space of limited dimensionality.

The ability to discriminate between all natural surfaces would be the design recommended by the “environmental 
regularity” philosophy of sensory modalities. The dimensionality of the internal model would mirror the dimensionality 
of the environment. As it turns out, natural surfaces have spectral reflectance distributions that vary along roughly 
five to seven dimensions (Maloney 1986). There thus exist natural surfaces that, although appearing to trichromatic 
viewers as “the same color,” nonetheless possess different spectral reflectance distributions.

Shepard (1992) instead asks how many color channels are needed to ensure that the color we perceive is the same color 
each time the surface is viewed under different lighting conditions. The amount of ambient light can also potentially 
vary along an unlimited number of dimensions, and the actual light reaching the eye is the product of the spectral 
power distribution and the spectral reflectance distribution. A reddish object in bluish light may reflect the same 
number of photons of each wavelength as a bluish object in reddish light. Similarly, a white object in reddish light 
may reflect mostly red photons, while the same white object in bluish light may reflect mostly blue photons. And yet 
the human visual system manages to maintain the property of color constancy; the same object will appear to be the 
same color under different lighting conditions.

Judd et al. (1964) measured 622 spectral power distributions for natural lighting, under 622 widely varying natural 
conditions of weather and times of day, and found that variations in natural lighting reduce to three degrees of 
freedom. Furthermore, these three degrees of freedom bear a close correspondence to the three dimensions of color 
opponency that were proposed for the human visual system based on experimental examination (Hurvich and Jameson 1957). 
The three degrees of freedom are:

1. The light-dark variation, which depends on the total light reaching the object.

2. The yellow-blue variation, which depends on whether a surface is illuminated by direct sunlight or is in shade. In 
shade the surface is illuminated by the Raleigh-scattered blue light of the sky, but is not directly illuminated by the 
sun. The corresponding yellow extreme occurs when an object is illuminated only by direct sunlight; e.g., if sunlight 
enters through a small channel and skylight is cut off.

3. The red-green variation, which depends on both the elevation of the sun (how much atmosphere the sun travels through), 
and the amount of atmospheric water vapor. E.g., illumination by a red sunset versus illumination at midday. Red 
wavelengths are the wavelengths least scattered by dust and most absorbed by water.

The three color channels of the human visual system are precisely the number of channels needed in order to maintain 
color constancy under natural lighting conditions.18 Three color channels are not enough to discriminate between all
natural surface reflectances, but three color channels are the exact number required to compensate for ambient natural 
lighting and thereby ensure that the same surface is perceptually the “same color” on any two occasions. This 
simplifies the adaptively important task of recognizing a previously experienced object on future encounters.
```

On evolution vs deliberative design (“intelligent design” would be preferable if it weren’t already so loaded), featuring a notion new to me — the “evolution of evolvability” (Wagner and Altenberg 1996):

```markdown
There is a fundamental rift between evolutionary design and deliberative design. From the perspective of a 
deliberative intelligence—a human, for instance—evolution is the degenerate case of design-and-test where 
intelligence equals zero. Mutations are atomic; recombinations are random; changes are made on the genotype’s 
lowest level of organization (flipping genetic bits); the grain size of the component tested is the whole 
organism; and the goodness metric operates solely through induction on historically encountered cases, without 
deductive reasoning about which contextual factors may later change.

The evolution of evolvability (Wagner and Altenberg 1996) improves this picture somewhat. There is a tendency 
for low-level genetic bits to exert control over highlevel complexity, so that changes to those genes can 
create high-level changes. Blind selection pressures can create self-wiring and self-repairing systems that 
turn out to be highly evolvable because of their ability to phenotypically adapt to genotypical changes.

Evolution never refactors its code. It is far easier for evolution to stumble over a thousand individual 
optimizations than for evolution to stumble over two simultaneous changes which are together beneficial and 
separately harmful. The genetic code that specifies the mapping between codons (a codon is three DNA bases) and 
the 20 amino acids is inefficient; it maps 64 possible codons to 20 amino acids plus the stop code. Why hasn’t 
evolution shifted one of the currently redundant codons to a new amino acid, thus expanding the range of possible 
proteins? Because for any complex organism, the smallest change to the behavior of DNA—the lowest level of genetic 
organization— would destroy virtually all higher levels of adaptive complexity, unless the change were accompanied 
by millions of other simultaneous changes throughout the genome to shift every suddenly-nonstandard codon to one 
of its former equivalents. Evolution simply cannot handle simultaneous dependencies, unless individual changes can 
be deployed incrementally, or multiple phenotypical effects occur as the consequence of a single genetic change. 
For humans, planning coordinated changes is routine; for evolution, impossible. Evolution is hit with an enormous 
discount rate when exchanging the paper currency of incremental optimization for the hard coin of complex design.
```

<a name="#miscellaneous"></a>

## Miscellaneous
([overview](#overview))

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

David Wong:

```markdown
It's not that clean energy will never happen -- it totally will. It's just that it won't come from a 
wild-haired scientist running out of his basement screaming, "Eureka! I've discovered how to get limitless 
clean energy from common seawater!" Instead, it will come from thousands of scientists publishing unreadable 
studies with titles like "Assessing Effectiveness and Costs of Asymmetrical Methods of Beryllium Containment 
in Gen 4 Liquid Fluoride Thorium Reactors When Factoring for Cromulence Decay." The world will be saved by a 
series of boring, incremental advances that chip away at those technical challenges one tedious step at a time.

But nobody wants to read about that in their morning Web browsing. We want to read that while we were sleeping, 
some unlikely hero saved the world. Or at least cured cancer.
```

William T. Powers:

```markdown
One thing I have advocated, without much success, is that children be taught social rules (when they are 
ready) in exactly the same way they are taught and teach each other games. The point is not whether the 
rules are right or wrong. Are the rules of 5-card stud poker or hopscotch right or wrong? It's that we're 
playing a certain game here, and there are rules to this game just as in any other game. If you want to 
be in the game, then you have to learn how to play it. Different groups of people play different games 
(different rules = different game), so if you want to play in different groups, you have to learn the 
games they play. When you develop the levels of understanding above the rule level, you'll be able to 
understand all games, and be able to join in anywhere. You won't be stuck knowing how to play only one game.

My problem with selling this idea is that people tend to think that their game is the only right one. 
In fact, being told that they are playing a game with arbitrary rules is insulting or frightening. They 
want to believe that the rules they know are the ones that everyone ought to play by; they even set 
up systems of punishment and reward to make sure that nobody tries to play a different game. They turn 
the game into something that is deadly serious, and so my idea simply seems frivolous instead of liberating.
```

Patrick McKenzie, "Some Perspective on the Japan Earthquake":

```markdown
The story of Japanese railways during the earthquake and tsunami is the story of an unceasing drumbeat 
of everything going right [...] The overwhelming response of Japanese engineering to the challenge posed 
by an earthquake larger than any in the last century was to function exactly as designed. Millions of 
people are alive right now because the system worked and the system worked and the system worked.

That this happened was, I say with no hint of exaggeration, one of the triumphs of human civilization. 
Every engineer in this country should be walking a little taller this week. We can’t say that too loudly, 
because it would be inappropriate with folks still missing and many families in mourning, but it doesn’t 
make it any less true.
```

Bruce Schneier:

```markdown
In our large, anonymous society, it's easy to forget moral and reputational pressures and concentrate on 
legal pressure and security systems. This is a mistake; even though our informal social pressures fade 
into the background, they're still responsible for most of the cooperation in society.
```

Razib Khan, [Reification is alright by me](http://blogs.discovermagazine.com/gnxp/2012/05/reification-is-alright-by-me/):

```markdown
The categories and classes we construct are simply the semantic sugar which makes the reality go down 
easier. They should never get confused for the reality that is, the reality which we perceive but darkly 
and with biased lenses. The hyper-relativists and subjectivists who are moderately fashionable in some 
humane studies today are correct to point out that science is a human construction and endeavor. Where 
they go wrong is that they are often ignorant of the fact that the orderliness of many facets of nature 
is such that even human ignorance and stupidity can be overcome with adherence to particular methods and 
institutional checks and balances. The predictive power of modern science, giving rise to modern 
engineering, is the proof of its validity. No talk or argumentation is needed. Boot up your computer. 
Drive your car.
```

Paul Graham, [A student's guide to startups](http://www.paulgraham.com/mit.html):

```markdown
The market doesn't give a shit how hard you worked. Users just want your software to do what they need, 
and you get a zero otherwise. That is one of the most distinctive differences between school and the 
real world: there is no reward for putting in a good effort. In fact, the whole concept of a "good effort" 
is a fake idea adults invented to encourage kids. It is not found in nature. 
```

From *Cryptonomicon*, by Neal Stephenson:

```markdown
Your younger nerd takes offense quickly when someone near him begins to utter declarative sentences, 
because he reads into it an assertion that he, the nerd, does not already know the information being 
imparted. 

But your older nerd has more self-confidence, and besides, understands that frequently people need to 
think out loud. 

And highly advanced nerds will furthermore understand that uttering declarative sentences whose contents 
are already known to all present is part of the social process of making conversation and therefore 
should not be construed as aggression under any circumstances.
```

Hastie Dawes, *Rational Choice in an Uncertain World*, pp. 67-8:

```markdown
A lot of outcomes about which we care deeply are not very predictable. For example, it is not comforting 
to members of a graduate school admissions committee to know that only 23% of the variance in later 
faculty ratings of a student can be predicted by a unit weighting of the student's undergraduate GPA, 
his or her GRE score, and a measure of the student's undergraduate institution selectivity -- but that 
is opposed to 4% based on those committee members' global ratings of the applicant. We want to predict 
outcomes important to us. It is only rational to conclude that if one method (a linear model) does not 
predict well, something else may do better. What is not rational -- in fact, it's irrational -- is to 
conclude that this "something else" necessarily exists and, in the absence of any positive supporting 
evidence, is intuitive global judgment.
```

David Friedman, *The Machinery of Freedom*:

```markdown
The person who says, as almost everyone does say, that human life is of infinite value, not to be measured 
in mere material terms, is talking palpable, if popular, nonsense. If he believed that of his own life, he 
would never cross the street, save to visit his doctor or to earn money for things necessary to physical 
survival. He would eat the cheapest, most nutritious food he could find and live in one small room, saving 
his income for frequent visits to the best possible doctors. He would take no risks, consume no luxuries, 
and live a long life. If you call it living. If a man really believed that other people's lives were 
infinitely valuable, he would live like an ascetic, earn as much money as possible, and spend everything 
not absolutely necessary for survival on CARE packets, research into presently incurable diseases, and 
similar charities.

In fact, people who talk about the infinite value of human life do not live in either of these ways. They 
consume far more than they need to support life. They may well have cigarettes in their drawer and a sports 
car in the garage. They recognize in their actions, if not in their words, that physical survival is only 
  one value, albeit a very important one, among many.
```

Peter Watts, *Blindsight*:

```markdown
In the beginning were the gametes. And though there was sex, lo, there was no gender, and life was in 
balance.

And God said, "Let there be Sperm": and some seeds did shrivel in size and grow cheap to make, and they 
did flood the market.

And God said, "Let there be Eggs": and other seeds were afflicted by a plague of Sperm. And yea, few of 
them bore fruit, for Sperm brought no food for the zygote, and only the largest Eggs could make up the 
shortfall. And these grew yet larger in the fullness of time.

And God put the Eggs into a womb, and said, "Wait here: for thy bulk has made thee unwieldy, and Sperm 
must seek thee out in thy chambers. Henceforth shalt thou be fertilized internally." And it was so.

And God said to the gametes, "The fruit of thy fusion may abide in any place and take any shape. It may 
breathe air or water or the sulphurous muck of hydrothermal vents. But do not forget my one commandment 
unto you, which has not changed from the beginning of time: spread thy genes."

And thus did Sperm and Egg go into the world. And Sperm said, "I am cheap and plentiful, and if sowed 
abundantly I will surely fulfill God's plan. I shall forever seek out new mates and then abandon them 
when they are with child, for there are many wombs and little time."

But Egg said, "Lo, the burden of procreation weighs heavily upon me. I must carry flesh that is but half
mine, gestate and feed it even when it leaves my chamber" (for by now many of Egg's bodies were warm of 
blood, and furry besides). "I can have but few children, and must devote myself to those, and protect them 
at every turn. And I will make Sperm help me, for he got me into this. And though he doth struggle at my 
side, I shall not let him stray, nor lie with my competitors."

And Sperm liked this not.

And God smiled, for Its commandment had put Sperm and Egg at war with each other, even unto the day they 
made themselves obsolete.
```

From [Oglaf](http://oglaf.com/bugfuck/epilogue/):

```markdown
In some species of Anglerfish, the male is much smaller than the female and incapable of feeding 
independently. To survive he must smell out a female as soon as he hatches. He bites into her releasing 
an enzime which fuses him to her permanently. He lives off her blood for the rest of his life, providing 
her with sperm whenever she needs it. Females can have multiple males attached. 

The moral is simple: males are parasites, women are sluts. 

Ha! Just kidding! The moral is don't treat actual animal behavior like a fable. Generally speaking, 
animals have no interest in teaching you anything.
```

Terry Pratchett, *Unseen Academicals*:

```markdown
The Patrician took a sip of his beer. "I have told this to few people, gentlemen, and I suspect I never 
will again, but one day when I was a young boy on holiday in Uberwald I was walking along the bank of a 
stream when I saw a mother otter with her cubs. A very endearing sight, I'm sure you will agree, and even 
as I watched, the mother otter dived into the water and came up with a plump salmon, which she subdued 
and dragged onto a half-submerged log. As she ate it, while of course it was still alive, the body split 
and I remember to its day the sweet pinkness of its roes as they spilled out, much to the delight of the 
baby otters who scrambled over themselves to feed on the delicacy. 

One of nature's wonders, gentlemen: mother and children dining upon mother and children. 

And that's when I first learned about evil. It is built in to the very nature of the universe. Every world 
spins in pain. If there is any kind of supreme being, I told myself, it is up to all of us to become his 
moral superior."
```

Megan McArdle, [Only stupid people call people stupid](https://www.bloomberg.com/opinion/articles/2014-08-12/only-stupid-people-call-people-stupid):

```markdown
I’m always fascinated by the number of people who proudly build columns, tweets, blog posts or Facebook 
posts around the same core statement: “I don’t understand how anyone could (oppose legal abortion/support 
a carbon tax/sympathize with the Palestinians over the Israelis/want to privatize Social Security/insert 
your pet issue here)." It’s such an interesting statement, because it has three layers of meaning.

The first layer is the literal meaning of the words: *I lack the knowledge and understanding to figure this 
out*. But the second, intended meaning is the opposite: *I am such a superior moral being that I cannot even 
imagine the cognitive errors or moral turpitude that could lead someone to such obviously wrong conclusions*. 
And yet, the third, true meaning is actually more like the first: *I lack the empathy, moral imagination or 
analytical skills to attempt even a basic understanding of the people who disagree with me*.

In short, “I’m stupid.” Something that few people would ever post so starkly on their Facebook feeds.
```

Steven Pinker, [The trouble with Harvard](https://newrepublic.com/article/119321/harvard-ivy-league-should-judge-students-standardized-tests): 

```markdown
A skilled professional I know had to turn down an important freelance assignment because of a recurring 
commitment to chauffeur her son to a resumé-building “social action” assignment required by his high 
school. This involved driving the boy for 45 minutes to a community center, cooling her heels while he 
sorted used clothing for charity, and driving him back—forgoing income which, judiciously donated, could 
have fed, clothed, and inoculated an African village. The dubious “lessons” of this forced labor as an 
overqualified ragpicker are that children are entitled to treat their mothers’ time as worth nothing, 
that you can make the world a better place by destroying economic value, and that the moral worth of 
an action should be measured by the conspicuousness of the sacrifice rather than the gain to the beneficiary.
```

Douglas Hofstadter on the necessary strangeness of scientific explanations:

```markdown
It is no accident, I would maintain, that quantum mechanics is so wildly counterintuitive. Part of the 
nature of explanation is that it must eventually hit some point where further probing only increases 
opacity rather than decreasing it. 

Consider the problem of understanding the nature of solids. You might wonder where solidity comes form. 
What if someone said to you, "The ultimate basis of this brick's solidity is that it is composed of a 
stupendous number of eensy weensy bricklike objects that themselves are rock-solid"? You might be 
interested to learn that bricks are composed of micro-bricks, but the initial question - "What accounts 
for solidity?" - has been thoroughly begged. What we ultimately want is for solidity to vanish, to 
dissolve, to disintegrate into some totally different kind of phenomenon with which we have no experience. 
Only then, when we have reached some completely novel, alien level will we feel that we have really made 
progress in explaining the top-level phenomenon.

...

I first saw this thought expressed in the stimulating book Patterns of Discovery by Norwood Russell 
Hanson. Hanson attributes it to a number of thinkers, such as Isaac Newton, who wrote, in his famous 
work Opticks: "The parts of all homogeneal hard Bodies which fully touch one another, stick together 
very strongly. And for explaining how this may be, some have invented hooked Atoms, which is begging 
the Question." Hanson also quotes James Clerk Maxwell (from an article entitled "Atom"): "We may 
indeed suppose the atom elastic, but this is to endow it with the very property for the explanation 
of which... the atomic constitution was originally assumed." Finally, here is a quote Hanson provides 
from Werner Heisenberg himself: "If atoms are really to explain the origin of color and smell of 
visible material bodies, then they cannot possess properties like color and smell." 

So, although it is not an original thought, it is useful to bear in mind that "greenness disintegrates".
```

<a name="#back"></a>
