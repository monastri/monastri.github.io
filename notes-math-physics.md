*[Word count](https://wordcounter.net/): 35,100*

## What is this?

This is the "math and physics" section of [this notebook](https://monastri.github.io/). 

<a name="#overview"></a>

## Overview

I've sorted the quotes below into the following categories. This is a provisional taxonomy, subject to perpetual refactoring. The reason it has a [Borgesian flavor](https://github.com/monastri/monastri.github.io/blob/master/poetry.md#the-celestial-emporium-of-benevolent-knowledge) is that it's meant to aid recall and idea-building. The categories are ordered alphabetically; the actual quotes (the top-level categories that is) are chronologically added.

1. [Advice](#math-advice)
	1. [Asking the right question](#asking-the-right-question)
	2. [Go to seminars, even if they're ostensibly irrelevant](#go-to-seminars)
	2. [Why you should read the masters in math](#reading-the-masters-in-math)
	3. [Why most mathematical writing sucks, and how to write better](#why-math-is-boring)
2. [Common misconceptions](#Common-misconceptions)
	1. [Misconceptions about relativity](#Misconceptions-about-relativity)
2. [ELI5](#ELI5)
	1. [Grothendieck toposes](#Grothendieck-toposes)
2. [Opinions and observations](#math-opinions)
	1. [Defining combinatorics](##Defining-combinatorics)
	2. [Expositions should solve problems terribly](#Solving-math-problems-terribly)
	2. [Good mathematics](#good-mathematics)
	2. [How a 'Math Product Manager' would teach and do math](#product-management-of-math)
	2. [How famous open problems get solved](#solving-famous-open-problems)  
	2. [How mathematical structures are defined](#How-mathematical-structures-are-defined)
	2. [Mathematical maturity and understanding](#mathematical-maturity)
	2. [Thinking and explaining](#Thinking-and-explaining)
	3. [What every mathematician should know](#what-every-mathematician-should-know)
	3. [Why didn't the Tricki take off?](#why-tricki-failed)
	
----------------------------------

<a name="#ELI5"></a>
## ELI5
([overview](#overview)) 

<a name="#Grothendieck-toposes"></a>
### Grothendieck toposes
([overview](#overview)) 

These two attempts by Jon Sterling and Andrej Bauer are pretty funny, because they're *wide* off the mark re: five year olds (cf Eliezer Yudkowsky's [Explainers Shoot High. Aim Low!](https://www.lesswrong.com/posts/2TPph4EGZ6trEbtku/explainers-shoot-high-aim-low)), but at least I felt like I got a sliver more than nothing out of their efforts.

Before we go to the actual ELI5s themselves, here's Eliezer:

```markdown
A few years ago, Ralph Merkle once told me how he'd written an explanation of his
field aimed at a much lower technical level than usual.  He had thought it would be
useful to academics outside the field, or even reporters.  This ended up being one
of his most popular papers *within* his field, cited more often than anything else 
he'd written.

The lesson was not that his fellow scientists were stupid, but that we tend to 
*enormously underestimate* the effort required to properly explain things.

He told me this, because I'd just told him about my experience publishing "An 
Intuitive Explanation of Bayesian Reasoning".  This is still one of my most popular,
most blogged, and most appreciated works today.  I regularly get fan mail from 
formerly confused undergraduates taking statistics classes, and journalists, and
professors from outside fields.  In short, I successfully hit the audience the 
eminent scientist had thought *he* was aiming for.

*I'd* thought I was aiming for elementary school.

Explainers shoot way, way higher than they think they're aiming, thanks to the 
illusion of transparency and self-anchoring.  We miss the mark by several major 
grades of expertise.  Aiming for outside academics gets you an article that will be
popular among specialists in your field.  Aiming at grade school (admittedly, naively
so) will hit undergraduates.  This is not because your audience is more stupid than 
you think, but because your words are far less helpful than you think.  You're way 
*way* overshooting the target.  Aim *several major gradations lower*, and you may hit
your mark.
```

The paper by Ralph Merkle, by the way, is [Secure Communications Over Insecure Channels](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.364.5157&rep=rep1&type=pdf). 

Jon Sterling:

```markdown
Sets express a static mathematical concept—an idea that doesn't change, has always
been, and will always be. Now, a lot of math can be developed in this way, because
most math is about these ideal concepts that have no connection to time or space.

But what about concepts that are living, or in motion, or changing over time and 
space? What about concepts that come into existence at a certain time or location,
but not before (or elsewhere)? These kinds of things come up in physics quite a lot,
but also in logic and computer science. To account for CONCEPTS IN MOTION is the 
purpose of toposes.

The easiest kind of topos is called a "presheaf topos"; imagine that you are starting
with some form of space (like a shape or a blob, or even a map of the earth). Then, 
we want to define the math of concepts that are varying over this space; you can 
think of this thing as like shining a bright beam onto the space, and whenever you do
so, a whole world of math is reflected off of it.

To be precise, a "concept" (presheaf) in the presheaf topos is an assignment of sets
to every "region" in the space, such that when a region contains another region, 
there is a way to get to the set assigned to the former from the set assigned to the
latter. Now, suppose the space under consideration is the timeline: then this just
means that concepts are refined as time goes on.

Another important kind of topos is called a Grothendieck topos, or a sheaf topos. In
this case, we want the mathematical concepts not only to vary appropriately over 
space, but to do so in a continuous manner: that is, small perturbations in the
region of space should be reflected as small perturbations in the concept (sheaf) 
defined over that space.

To be precise, when you have a "cover" on a region U in the space (that is, a
collection of regions which is partly visible in every direction from U), if for 
every region in the cover you have an instance of the concept/sheaf over that region,
then these insights can be combined in a nice way to get an instance of the concept 
at U.

In logic, presheaves express how truth is preserved over time: if it is true now, it
is true later! What sheaves do is express how truth is "closed under" inevitability:
that is, if it will eventually become true no matter what happens, then it is 
considered true now.

Now, there are even more kinds of topos! Lawvere and Tierney summed up the 
characteristics of grothendieck and presheaf toposes into slogans which they used to 
abstractly define something called an "elementary topos". All toposes are elementary
toposes, but there are some elementary toposes which are not grothendieck toposes! An
example is the "effective topos", a topos that captures the idea of mathematical 
concepts being tracked by computer codes.
```

Andrej Bauer:

```markdown
A topos is a mathematical universe. You can imagine a mathematical universe as a possible
mathematical reality, a bit like Star Wars vs. Star Trek.

In order to do mathematics, we need some sort of a universe in which to do it. It has to
contain enough stuff to get us going: numbers, straight lines, circles, trigonometric
functions, and everything else that mathematicians usually use. The universe that most
mathematicians use, and that many people have heard of, is set theory. In this universe
all mathematical objects and constructions are made of sets which are made of sets which
are made of sets which are made of ...

But this is not the only possibility. Alexander Grothendieck discovered that in order to
do certain kinds of geometry (algebraic geometry), he needed a different kind of
mathematical universe in which things were not made of sets but of something that
mathematicians call "sheaves". You will learn about those when you turn 6, for now let
us just imagine them as kind of layered cakes. The point is that these layers bind
together the mathematical universe and all object within with a Force, whereas making 
things from sets is more like building castles from beach sand – they easily fall apart.

Grothendieck used his toposes to do geometry, but later logicians, in particular William
Lawvere, realized that the things he came up with were actually entire mathematical
universes. Not only did they contain the stuff that Grothendieck cared about, but also 
othe kinds of math: algebra, arithmetic, combinatorics, analysis, etc. Thus, instead of
having one universe they now had a multiverse of universes to explore.

Toposes turned out to be useful for many purposes. And they are not all of the kind that
Grothendieck discovered (his are pretty big). For instance, a realizability topos is a 
computer-science heaven: instead of having everything made of layered cakes, everything
is made of pieces of program code (this was invented in the 1980's).

The various toposes share many things in common, for instance simple stuff like "6 
divides 18". For fancy stuff they disagree. Mathematicians who live in a realizability 
topos will see that everything is computable, whereas those who live in a Grothendieck 
topos might say things like "you cannot split a straight line into two parts" (it's not
made of sand, you really can't, it's bound together with the Force).
```

<a name="#math-opinions"></a>
## Math opinions
([overview](#overview))

<a name="#Defining-combinatorics"></a>
### Defining combinatorics
([overview](#overview))

I took an introduction to combinatorics course with Igor Pak back in the day, and found him a fascinating character. Later Googling made me realize he was a pretty big-shot figure -- this gets lost in the Taos and Manolescus of the university, but he's still pretty influential in his subfield -- which made his pontifications somehow endearing. Here's his webpage [What is combinatorics?](https://igorpak.wordpress.com/2013/05/14/what-is-combinatorics/), where he first considers and dismisses popular definitions, and settles on the one given by Gian-Carlo Rota.

Igor rejects the usual "discrete stuff" approach:

```markdown
Few themes emerge.  First, that combinatorics is some kind of discrete universe which 
deals with discrete “configurations”, their existence and counting.  Where to begin?  
This is “sort of” correct, but largely useless.  Should we count logic, rectifiable 
knots and finite fields in, and things like Borsuk conjecture and algebraic combinatorics
out?  This is sort of like defining an elephant as a “large animal with a big trunk and
big ears”.  This “descriptive” definition may work for Webster’s dictionary, but if you 
have never seen an elephant, you really don’t know how big should be the ears, and have
a completely wrong idea about what is a trunk.  And if you have seen an elephant, this 
definition asks you to reject a baby elephant whose trunk and ears are smaller.  
Not good.
```

Igor rejects the "it's defined by its tools and methods, or lack of thereof" approach:

```markdown
Second theme: combinatorics is defined by its tools and methods, or lack of thereof.  
This is more of a wishful thinking than a working definition.  It is true that
practitioners in different parts of combinatorics place a great value on developing new
extensions and variations of the available tools, as well as ingenuous ad hoc arguments. 
But a general attitude, it seems, is basically “when it comes to problem solving, one 
can use whatever works”.  For example, our recent paper proves unimodality results for
the classical Gaussian coefficients and their generalizations via technical results for
Kronecker coefficients, a tool never been used for that before.  Does that make our 
paper “less combinatorial” somehow?  In fact, some experts openly advocate that the more 
advanced the tools are, the better, while others think that “term ‘combinatorial methods’,
has an oxymoronic character”.
```

Igor rejects the "it's ineffable" approach:

```markdown
Third theme: combinatorics is “special” and cannot be defined.  Ugh…  This reminds me of 
an old (1866), but sill politically potent Russian verse (multiple English translations)
by Tyutchev.  I can certainly understand the unwillingness to define combinatorics, but 
saying it is not possible is just not true.
```

Igor rejects the piecemeal approach:

```markdown
Either going over a long list of topics, or giving detailed and technical rules why 
something is and something isn’t combinatorics.  But this bound to raise controversy, 
like who decides?  For example, take PCM’s “few constraints” rule.  Really?  Somebody
thinks block designs, distance-regular graphs or coding theory have too few constraints? 
I don’t see it that way.  In general, this is an encyclopedia style approach.  It can 
work on Wikipedia which is constantly updated and the controversies are avoided by
constant search for a compromise (see also my old post), but it’s not a definition.
```

"Combinatorics is similarly formed by the (historical) battles, and can only be defined as such":

```markdown
After some reading and thinking, I concluded that Gian-Carlo Rota’s 44 y.o. explanation in 
“Discrete thoughts” is exactly right.  Let me illustrate it with my own (lame) metaphor.

Imagine you need to define Russia (not Tyutchev-style).  You can say it’s the largest country
by land mass, but that’s a description, not a definition.  The worst thing you can do is try
to define it as a “country in the North” or via its lengthy borders.  You see, Russia is huge, 
spead out and disconnected.  It lies to the North of China but has a disconnected common 
border, it has a 4253 mile border with Kazakhstan (longer than the US-Canada border excluding
Alaska), surrounding the country from three sides, it lies North-West of Japan, East of 
Latvia, South-West of Lithuania (look it up!), etc.  It even borders North Korea, not that 
this tiny border is much in use.  Basically, Russian borders are complicated and are a result
of numerous wars and population shifts; they have changed many times and might change again.

Now, Rota argues that Combinatorics is similarly formed by the battles, and can only be 
defined as such.  It is a large interconnected field concentrated (but not coinciding!) around
basic discrete tools and problems, but with tentacles reaching deep into “foreign territory”.
Its current shape is a result of numerous “wars” – the borderline problems are tested on which
tools are more successful, and whoever “wins”, gets to absorb a new subfield.  For example, in
its “war” with topology, combinatorics “won” graph theory and “lost” knot theory (despite a 
strong combinatorial influence).  In other areas, such as computer science and discrete 
probability, Rota argues there a lot of cooperation, a mutually beneficial “joint governance” 
(all lame metaphors are mine).  But as a consequence, if one is to define Combinatorics (or 
Russia), the historical-cultural approach would go best.  Not all that different from Sheldon’s
approach to define Physics “from the beginning”.

In conclusion, let’s acknowledge that Combinatorics can indeed be defined in the same (lengthy
historical) manner as a large diverse country, but such definition would be neither short nor
enlightening, more like a short survey.  As Danny Kleitman writes, in practice this lack of a
clear and meaningful definition of the subject “never bothered him”, and we agree.  I think 
it’s time to stop worrying about that.  But if someone makes blank general statements painting
all of combinatorics in a certain way, this is just indefensible.
```

There's also a huge collection of quotes by Igor [here](http://www.math.ucla.edu/~pak/hidden/papers/Quotes/Combinatorics-quotes.htm).

<a name="#two-cultures"></a>
### Two cultures
([overview](#overview))

There is already [an nLab note on this](https://ncatlab.org/davidcorfield/show/Two+Cultures) by the mathematical philosopher David Corfield summarizing most of what's been talked about online. I'll pick quotes I liked for my own worldview-training. 

In the [original essay](http://www.dpmms.cam.ac.uk/~wtg10/2cultures.pdf) (17 pages), Tim Gowers was drawing attention/pointing out a parallel to the following asymmetry in understanding due to lack of communication between science and the humanities as exemplified by the following quote by CP Snow in his "Two Cultures" Rede lecture in 1959: 

```markdown
A good many times I have been present at gatherings of people who, by the standards
of the traditional culture, are thought highly educated and who have with considerable
gusto been expressing their incredulity at the illiteracy of scientists. Once or twice I
have been provoked and have asked the company how many of them could describe
the Second Law of Thermodynamics. The response was cold: it was also negative.
Yet I was asking something which is about the scientific equivalent of: 
*Have you read a work of Shakespeare’s?*
```

Gowers claims that "a similar sociological phenomenon can be observed within pure mathematics":

```markdown
Loosely speaking, I mean the distinction between mathematicians who regard their central
aim as being to solve problems, and those who are more concerned with building and
understanding theories. ...

When I say that mathematicians can be classified into theory-builders and problem-solvers, 
I am talking about their priorities, rather than making the ridiculous claim that they are
exclusively devoted to only one sort of mathematical activity.

As with most categorizations, it involves a certain oversimplification, but not so much as 
to make it useless.
```

The oversimplification part shouldn't be a point of contention if you've internalized principal component analysis, or Box's "all models are wrong but some are useful" dictum. It is *understood* that the classification oversimplifies; the point is whether it's an illuminating classification.

Gowers notes that he isn't the first to point this out. Here's Gian-Carlo Rota in *Indiscrete Thoughts*:

```markdown
Mathematicians can be subdivided into two types: problem solvers and theorizers. Most 
mathematicians are a mixture of the two although it is easy to find extreme examples of both
types.

To the problem solver, the supreme achievement in mathematics is the solution to a problem
that has been given up as hopeless. It matters little that the solution may be clumsy; all
that counts is that it should be the first and that the proof be correct. Once the problem 
solver finds the solution, he will permanently lose interest in it, and will listen to new
simplified proofs with an air of condescension suffused with boredom.

The problem solver is a conservative at heart. For him, mathematics consists of a sequence
of challenges to be met, an obstacle course of problems. The mathematical concepts required
to state mathematical problems are tacitly assumed to be eternal and immutable.

Mathematical exposition is regarded as an inferior undertaking. New theories are viewed with
deep suspicion, as intruders who must prove their worth by posing challenging problems before
they can gain attention. The problem solver resents generalizations, especially those that 
may succeed in trivializing the solution of one of his problems.

The problem solver is the role model for budding young mathematicians. When we describe to the
public the conquests of mathematics, our shining heroes are the problem solvers.

To the theorizer, the supreme achievement of mathematics is a theory that sheds sudden light on
some incomprehensible phenomenon. Success in mathematics does not lie in solving problems but 
in their trivialization. The moment of glory comes with the discovery of a new theory that does
not solve any of the old problems but renders them irrelevant.

The theorizer is a revolutionary at heart. Mathematical concepts received from the past are
regarded as imperfect instances of more general ones yet to be discovered. Mathematical exposition
is considered a more difficult undertaking than mathematical research.

To the theorizer, the only mathematics that will survive are the definitions. Great definitions 
are what mathematicians contribute to the world. Theorems are tolerated as a necessary evil since
they play a supporting role — or rather, as the theorizer will reluctantly admit, an essential 
role — in the understanding of definitions.

Theorizers often have trouble being recognized by the community of mathematicians. Their 
consolation is the certainty, which may or may not be borne out by history, that their theories
will survive long after the problems of the day have been forgotten.

If I were a space engineer looking for a mathematician to help me send a rocket into space, I 
would choose a problem solver. But if I were looking for a mathematician to give a good education 
to my child, I would unhesitatingly prefer a theorizer.
```

Drossbucket quotes Poincare's [Intuition and logic in mathematics](http://www-history.mcs.st-andrews.ac.uk/Extras/Poincare_Intuition.html):

```markdown
It is impossible to study the works of the great mathematicians, or even those of the lesser,
without noticing and distinguishing two opposite tendencies, or rather two entirely different 
kinds of minds. 

The one sort are above all preoccupied with logic; to read their works, one is tempted to believe
they have advanced only step by step, after the manner of a Vauban who pushes on his trenches
against the place besieged, leaving nothing to chance.

The other sort are guided by intuition and at the first stroke make quick but sometimes 
precarious conquests, like bold cavalrymen of the advance guard.
```

Atiyah casts it in terms of dominant visual vs sequential thinking in [What is geometry?](http://www.jstor.org/discover/10.2307/3616542?sid=21105166613741&uid=4&uid=3738032&uid=2):

```markdown
Broadly speaking I want to suggest that geometry is that part of mathematics in which 
visual thought is dominant whereas algebra is that part in which sequential thought is
dominant. This dichotomy is perhaps better conveyed by the words “insight” versus “rigour”
and both play an essential role in real mathematical problems.
```

Mark Kac's "magician" quote:

```markdown
There are two kinds of geniuses: the ‘ordinary’ and the ‘magicians.’ an ordinary genius is a 
fellow whom you and I would be just as good as, if we were only many times better. There is 
no mystery as to how his mind works. Once we understand what they’ve done, we feel certain 
that we, too, could have done it. It is different with the magicians... Feynman is a magician
of the highest caliber.
```

Steven Weinberg's *Dreams of a Final Theory*:

```markdown
Theoretical physicists in their most successful work tend to play one of two roles: they are 
either sages or magicians... It is possible to teach general relativity today by following 
pretty much the same line of reasoning that Einstein used when he finally wrote up his work in 1915. 

Then there are magician-physicists, who do not seem to be reasoning at all but who jump over 
all intermediate steps to a new insight about nature. The authors of physics textbook are usually
compelled to redo the work of the magicians so they seem like sages; otherwise no reader would 
understand the physics.
```

Before we move on: why dichotomy? Why not trichotomy, or "quadrochotomy" [like Barry Mazur's tribes](#what-every-mathematician-should-know)? Commenter alkjash on drossbucket's post [Two types of mathematician](https://www.lesswrong.com/posts/5QnvHZpy4pGgCo3Pp/two-types-of-mathematician) says it's because a dichotomy corresponds to doing PCA:

```markdown
All over the place, we speak in terms of dichotomies and not trichotomies or more. The reason
is basically that each dichotomy corresponds to doing PCA and projecting space onto a single 
axis, and a one-dimensional line has two directions. This suggests that much of the interesting
conversation about any given topic (i.e. axis) can be picked up by having exactly two people 
talk about it. Two people will always differ slightly on the axis. Adding any additional people
to a conversation has rapidly diminishing returns: you may have more total disagreement, but 
rarely more total *dimensionality* in the disagreement.

Applying the Solitaire Principle, for all the same reasons it's useful to have conversations
between two people, it's most useful to draw dichotomies between two pieces of the mind instead
of more. This is why we have Internal Double Crux instead of Triple or more. A conversation/internal
conflict is always about something and should have a purpose, and that purpose projects the entire
conversation onto the one relevant dimension, so it's really only necessary to divide into two sides
along this axis. Thus we get S1/S2, Elephant/Rider, Episodic/Diachronic, etc.
```

Why project onto a single axis in the first place? Qiaochu:

```markdown
There are many reasons it's so tempting to project onto a single axis but maybe the foundational
reason is the dichotomy between approaching and avoiding, or if you prefer, between positive and 
negative reward in reinforcement learning terms. This blows up into good vs. evil, friend vs. enemy,
and so forth.
```

So what's the asymmetry?

```markdown
Subjects that appeal to theory-builders are, at the moment,
much more fashionable than the ones that appeal to problem-solvers.
Moreover, mathematicians in the theory-building areas often regard what they are doing 
as the central core (Atiyah uses this exact phrase) of mathematics, with subjects such 
as combinatorics thought of as peripheral and not particularly relevant to the main aims 
of mathematics. 

One can almost imagine a gathering of highly educated mathematicians 
expressing their incredulity at the ignorance of combinatorialists, most of whom could 
say nothing intelligent about quantum groups, mirror symmetry, Calabi-Yau manifolds, the 
Yang-Mills equation, solitons or even cohomology. If a combinatorialist were to interrupt 
such a gathering and ask roughly how many subsets of {1, 2, . . . , n} can be found such that
the symmetric difference of any two of them has size at least n/3, the response might very 
well be a little frosty. (This problem is very easy if and only if one knows the appropriate
technique, which is to choose sets randomly and show that the chances of any given pair of them
having a symmetric difference of size less than n/3 are exponentially small. So the answer
is e^cn for some constant c > 0.) ...

My main purpose here is to defend some of the less fashionable subjects against
criticisms commonly made of them. I shall devote most of my attention to combinatorics,
since this is the area I know best.
```

A litmus test to see which camp you belong to:

```markdown
(i) The point of solving problems is to understand mathematics better.
(ii) The point of understanding mathematics is to become better able to solve problems.

Most mathematicians would say that there is truth in both (i) and (ii). Not all problems
are equally interesting, and one way of distinguishing the more interesting ones is to
demonstrate that they improve our understanding of mathematics as a whole. Equally,
if somebody spends many years struggling to understand a difficult area of mathematics,
but does not actually do anything with this understanding, then why should anybody else
care? 

However, many, and perhaps most, mathematicians will not agree equally strongly
with the two statements.
```

A prototypical theory-builder would be Michael Atiyah (RIP). From a 1984 interview in the Mathematical Intelligencer:

```markdown
MINIO: How do you select a problem to study?

ATIYAH: I think that presupposes an answer. I don’t think that’s the way I work
at all. Some people may sit back and say, “I want to solve this problem” and they
sit down and say, “How do I solve this problem?” I don’t. I just move around in
the mathematical waters, thinking about things, being curious, interested, talking to
people, stirring up ideas; things emerge and I follow them up. Or I see something
which connects up with something else I know about, and I try to put them together
and things develop. I have practically never started off with any idea of what I’m
going to be doing or where it’s going to go. I’m interested in mathematics; I talk, I
learn, I discuss and then interesting questions simply emerge. I have never started off
with a particular goal, except the goal of understanding mathematics.
```

(Tangentially, this sounds like what John Baez does, as someone who's followed him for years.)

A prototypical problem-solver would be Erdos. See also [Golovanov on Grigori Perelman](#grigori-perelman).

Different branches of math, Gowers claims, "obviously" need different aptitudes (*orientations* is the more correct word here):

```markdown
In some, such as algebraic number theory, or the cluster of subjects
now known simply as Geometry, it seems (to an outsider at least - I have no authority for
what I am saying) to be important for many reasons to build up a considerable expertise
and knowledge of the work of other mathematicians are doing, as progress is often the
result of clever combinations of a wide range of existing results. Moreover, if one selects
a problem, works on it in isolation for a few years and finally solves it, there is a danger,
unless the problem is very famous, that it will no longer be regarded as all that significant.

At the other end of the spectrum is, for example, graph theory, where the basic object,
a graph, can be immediately comprehended. One will not get anywhere in graph theory
by sitting in an armchair and trying to *understand graphs* better. Neither is it particularly
necessary to read much of the literature before tackling a problem: it is of course helpful
to be aware of some of the most important techniques, but the interesting problems tend
to be open precisely because the established techniques cannot easily be applied.
```

Gowers continues with his defense of the problem-solving orientation/subculture:

```markdown
Why should problem-solving subjects be less highly regarded than theoretical ones?
To answer this question we must consider a more fundamental one: what makes one piece
of mathematics more interesting than another? 

Atiyah makes the point (see for example [A2]) that so much
mathematics is produced that it is not possible for all of it to be remembered. The processes
of abstraction and generalization are therefore very important as a means of making sense
of the huge mass of raw data (that is, proofs of individual theorems) and enabling at least
some of it to be passed on. The results that will last are the ones that can be organized
coherently and explained economically to future generations of mathematicians. Of course,
some results will be remembered because they solve very famous problems, but even these,
if they do not fit into an organizing framework, are unlikely to be studied in detail by more
than a handful of mathematicians.

Thus, it is useful to think not so much about the intrinsic interest of a mathematical
result as about how effectively that result can be communicated to other mathematicians,
both present and future. Combinatorics appears to many to consist of a large number
of isolated problems and results, and therefore to be at a disadvantage in this respect.
Each result individually may well require enormous ingenuity, but ingenious people exist,
especially in Hungary, and future generations of combinatorialists will not have the time
or inclination to read and admire more than a tiny fraction of their output.

It is certainly rare in combinatorics for
somebody to find a very general statement which suddenly places a large number of existing 
results in their proper context. It is also true that many of the results proved by
combinatorialists are somewhat isolated and will be completely forgotten (but this does
not distinguish combinatorics from any other branch of mathematics). However, it is not
true that there is no structure at all to the subject. The reason it appears to many mathe-
maticians as though combinatorics is just a miscellaneous collection of individual problems
and results is that the organizing principles are less explicit.

If the processes of abstraction and generalization, which are so important in mathematics,
are of only limited use in combinatorics, then how can the subject be transmitted
to future generations? One way of thinking about this question is to ask what the 
requirements of tomorrow’s combinatorialists are likely to be. As I have said already, their
priority is likely to be solving problems, so their interest in one of today’s results will
be closely related to whether, by understanding it, they will improve their own problem-
solving ability. And this brings us straight to the heart of the matter. The important ideas
of combinatorics do not usually appear in the form of precisely stated theorems, but more
often as *general principles of wide applicability*.
```

Gowers points out that these principles are so powerful that problems can "suddenly switch from being impossible to being almost trivia". 

An example of such a general principle comes from Erdos, which "opened the floodgates to probabilistic arguments in combinatoric":

```markdown

if one is trying to maximize the size of some structure under certain constraints, and
if the constraints seem to force the extremal examples to be spread about in a uniform
sort of way, then choosing an example randomly is likely to give a good answer.
```

This "general principles" phenomenon happens in in nonlinear PDEs too. Terry Tao says in his answer to the MO question [Why can’t there be a general theory of nonlinear PDE?](http://mathoverflow.net/questions/15292/why-cant-there-be-a-general-theory-of-nonlinear-pde):

```markdown
PDE does not have a general theory, but it does have a general set of principles and methods
(e.g. continuity arguments, energy arguments, variational principles, etc.).

Sergiu Klainerman's "PDE as a unified subject" discusses this topic fairly exhaustively.

Any given system of PDE tends to have a combination of ingredients interacting with each
other, such as dispersion, dissipation, ellipticity, nonlinearity, transport, surface tension,
incompressibility, etc. Each one of these phenomena has a very different character. Often the
main goal in analysing such a PDE is to see which of the phenomena "dominates", as this tends
to determine the qualitative behaviour (e.g. blowup versus regularity, stability versus 
instability, integrability versus chaos, etc.) But the sheer number of ways one could combine
all these different phenomena together seems to preclude any simple theory to describe it all.
This is in contrast with the more rigid structures one sees in the more algebraic sides of 
mathematics, where there is so much symmetry in place that the range of possible behaviour is
much more limited. (The theory of completely integrable systems is perhaps the one place where
something analogous occurs in PDE, but the completely integrable systems are a very, very small 
subset of the set of all possible PDE.)
```

Sergiu Klainerman's [PDE AS A UNIFIED SUBJECT](https://web.math.princeton.edu/~seri/homepage/papers/telaviv.pdf) has some great quotes itself expanding on what Terry said above, but Markdown screws with the quotes, so I'll just leave the link there.

Related to the "general principles" phenomenon is the *"become the grand meta-theorem"* comment on drossbucket's LW post [Two types of mathematician](https://www.lesswrong.com/posts/5QnvHZpy4pGgCo3Pp/two-types-of-mathematician) by alkjash that I keep (1) misattributing to Qiaochu (2) losing, irritatingly, so I'm pinning it down here:

```markdown
My take on the "Two Cultures" model of problem-solvers and theory-builders: theory-building
fields of mathematics like algebraic topology (say) are those where the goal is to articulate 
grand meta-theorems that are bigger than any particular application. This was the work of a
Grothendieck.

Meanwhile, concrete problem-solving fields of mathematics like combinatorics are those where
the goal is to become the grand meta-theorem that contains more understanding than any 
particular theorem you can prove. This was the style of an Erdos. The inarticulate grand meta-
theorems lived in his cognitive strategies so that the theorems he actually proved are 
individually only faint impressions thereof. (I think I heard the "become grand meta-theorem" 
phrasing originally from Alon & Spencer.)

Of course reality is self-similar, so it's not surprising that there's currently a big divide
in combinatorics between what I would call the "algebraic/enumerative" style of Richard Stanley
containing the Flajolet and Sedgewick stuff, characterized by fancy algebra/explicit formulae/
crystalline structures and the "analytic/extremal" style of Erdos, characterized by asymptotic
formulae and less legibility. It's surprisingly rare to see a combinatorialist bridge this gap.
```

Qiaochu responds by casting the difference in terms of legibility:

```markdown
Yeah, there's something less legible about combinatorics compared to most other fields of 
mathematics. People like Erdos know lots of important principles and meta-principles for 
solving combinatorial problems but it's a tremendous chore to state those principles explicitly
in terms of theorems and nobody really does it (the closest thing I've seen is Flajolet and 
Sedgewick - by the way, amazing book, highly recommended). A concrete example here is the 
exponential formula, which is orders of magnitude more complicated to state precisely than
it is to understand and use.
```

Qiaochu, re: hammers and nails dichotomy:

```markdown
Theory-building hammers are legible: they're big theorems, or maybe big messes of definitions 
and then theorems (the term of art for this is "machinery"). 

Problem-solving hammers are illegible: they're a bunch of tacit knowledge sitting inside 
some mathematician's head.
```

Sarah Constantin with a 2x2:

```markdown
Ok, here’s a 2x2 that captures a lot of the variation in OP:

abstract/concrete x intuitive/methodical.

Intuitive vs. Methodical is what Atiyah, Klein, and Poincare are talking about. 
Abstract vs Concrete is what Gowers, Rota, and Dyson are talking about.

Abstract and intuitive is like Grothendieck.

Concrete and intuitive is like geometry or combinatorics.

Concrete and methodical is like analysis.

Abstract and methodical — I don’t know what goes in this space.
```

More examples by Terry Tao:

```markdown
There is a famous distinction in prime number theory between the number theorists who 
like to multiply primes, and the number theorists who like to add primes. As the primes 
are very heavily multiplicatively structured, the mathematics of multiplying primes is 
very algebraic in nature, in particular involving field extensions, Galois representations,
etc. But the primes are very additively unstructured, and so for adding primes we see the
tools of analysis used instead (circle method, sieve theory, etc.).

“Counting primes in arithmetic progressions” can be easily converted (via the multiplicative 
Fourier transform) to “counting primes twisted by characters” - an eminently multiplicative
question, and one which is handled by primarily algebraic means. “Counting arithmetic
progressions in primes” however seems to be a stubbornly additive question and thus not 
really amenable to algebraic attacks. (On the other hand, “counting geometric progressions 
in primes” is very easy. :-) ).
```

Terry's comment on "structure" as part of structure/pseudorandom dichotomy and "structure" as seen by theory-builders, where he introduces the notion of "noisy" additive cohomologies and group theories:

```markdown
It does seem that categorification and similar theoretical frameworks are currently better 
for manipulating the type of exact mathematical properties (identities, exact symmetries,
etc.) that show up in structured objects than the fuzzier type of properties (correlation, 
approximation, independence, etc.) that show up in pseudorandom objects, but this may well 
be just a reflection of the state of the art than of some fundamental restriction. 

For instance, in my work on the Gowers uniformity norms, there are hints of some sort of
“noisy additive cohomology” beginning to emerge – for instance, one may have some sort of 
function which is “approximately linear” in the sense that its second “derivative” is “mostly
negligible”, and one wants to show that it in fact differs from a genuinely linear function
by some “small” error; this strongly feels like a cohomological question, but we do not yet
have the abstract theoretical machinery to place it in the classical cohomology framework
(except perhaps in the ergodic theory limit of these problems, where there does seem to be
a reasonable interpretation of these informal concepts). 

Similarly, when considering inverse theorems in additive combinatorics, a lot of what we do 
has the feel of “noisy group theory”, and we can already develop noisy analogues of some 
primitive group theory concepts (e.g. quotient groups, group extensions, the homomorphism 
theorems, etc.), but we are nowhere near the level of sophistication (and categorification,
etc.) with noisy algebra that exact algebra enjoys right now. But perhaps that will change in
the future.
```

Interesting remark by Dave Tweed on applied vs pure math as popular uprising vs army tank division:

```markdown
Disclaimer: I’m claiming “pure” mathematics is any activity where one has decreed that the entities
in the problem “work this way” and then proceeds, even if the problem is pursued partly for some other
reason. To me, “applied” really means one is constantly rejecting/modifying parts of the mathematics
“on physical grounds”.

Part of the justification for theory building is that it’s the equivalent of building an army tank
division rather than using a popular uprising: by optimally structuring things you can accomplish
exactly the same things but much, much easier. A good example of this is the theory of generating
functions and precise asymptotic estimation of coefficients. People like Philippe Flajolet are 
doing incredibly intricate and – to my mind – deep work putting together theories that can 
pulverise some of the combinatorial problems that occur in algorithm analysis. This is theory to
solve problems, rather than give pedantically correct names to everything. ...

In contrast, one area I’d like to work in seems to scream out for an organising theory, namely 
the mathematics/algorithmics of scene reconstruction given some subset of camera parameters and
scene parameters/structures. Part of the reason it’s an area “I’d like to work in” rather than 
“an area I do work in” is that there seems to be little structuring theory with sudden appearance 
of different matrix decompositions and different classifications of the degenerate conditions,
etc, at seemingly completely unrelated ways in the different algorithms, so it seems like 
currently to get to the cutting (maybe bleeding :-) ) edge you’ve got to study each algorithm 
from scratch. I’ve seen some work that claims to provide a theory for such things, but they all 
look like “getting the names right” theories rather than “army tank division theories”. 

...

What I was trying to get at by hyperbole in the original post was that you can have theories 
that “explain” things and “get the names right” and they’re good things to have developed. There
seemed to me a sort-of subtext in your post that most theories were of this sort (which is
probably a mis-reading based partly on the “aesthetic” point), so I was pointing out that there 
are other theories which are more about systematizing powerful tools. (Indeed, it’s really a
spectrum rather than a binary choice.) I’m not putting down explanatory theories but rather
pointing out there are also some really rather splendid “tank division” theories around. (Indeed,
arguably differential/integral calculus and linear algebra are more commonly used to “get 
answers” rather than “explain”.)

When I talk about “getting the names right” theories I just mean the cases where pains are taken
in definitions yet it’s not clear that this buys you anything more than precise definitions. This
is in contrast to, say, the more rigorous development of calculus in the nineteenth century which
actually clarifies the errors in some “paradoxes/contradictions” that were “constructible” before.
```

Another difference between the cultures is given in [this comment by John Baez](https://golem.ph.utexas.edu/category/2007/05/the_two_cultures_of_mathematic_1.html#c009757) responding to Terry Tao's claim that

```markdown
Secondly, one thing about the “problem solving” culture as opposed to the “theory building” is
that we tend to make progress by working upward from special cases, rather than downward from more
general formulations.
```

with this:

```markdown
It’s all very complicated.

Theory-builders may *act* as if general theories come full-blown into their heads, just waiting
to be applied to special cases. But often the most exciting part is finding those general theories 
in the first place. For this, one has to dream up patterns that would make sense of obscure clues.
This often progresses from special to general.

I think of my style as ‘finding paths of least resistance’, or ‘following the tao of mathematics’.
I’m more of a hiker than a rock-climber. I prefer to know lots of fun trails, and occasionally bump
into a new one while I’m strolling about, than spend my day trying to climb up a sheer cliff. 
Instead of trying to do anything hard, I prefer to keep lots of facts, patterns and questions in
mind, and make obvious guesses and deductions when I notice patterns turning up.

Given this rather lazy approach to mathematics, the only way to discover anything new is by knowing
a little about lots of things, and knowing some good patterns that haven’t been fully exploited. 
‘Categorification’ is my favorite pattern, because it’s extremely broad, and nowhere near being 
tapped out. But, it’s just one of many.

We can imagine two extremes. At one extreme we have someone who tries very hard to open a specific
door, perhaps melting the lock with an acetylene torch if necessary, or even blowing the door open 
with dynamite. At the other extreme, we have someone who carries a huge ring of keys and tries them 
all on any door they happen to walk by.
```

This reminds me of Julie Moronuki aka Monoid Mary aka Argumatronic's great essay [The Unreasonable Effectiveness of Metaphor](https://argumatronic.com/posts/2018-09-02-effective-metaphor.html), which I keep returning to but don't know where to categorize here.

<a name="#How-mathematical-structures-are-defined"></a>
### How mathematical structures are defined
([overview](#overview))

From Terry Tao's [post on Buzz](http://www.google.com/buzz/114134834346472219368/Mu6ZqEcaZkR/When-defining-the-concept-of-a-mathematical-space) via David Corfield's [notebook entry](https://ncatlab.org/davidcorfield/show/Two+Cultures) (the original link has succumbed to linkrot):

```markdown
When defining the concept of a mathematical space or structure (e.g. a group,
a vector space, a Hilbert space, etc.), one needs to list a certain number of 
axioms or conditions that one wants the space to satisfy. Broadly speaking, 
one can divide these conditions into three classes:

1. **closed conditions**. These are conditions that generally involve an = or 
a ≥ sign or the universal quantifier, and thus codify such things as algebraic
structure, non-negativity, non-strict monotonicity, semi-definiteness, etc. As
the name suggests, such conditions tend to be closed with respect to limits and
morphisms.

2. **open conditions**. These are conditions that generally involve a ≠ or a > 
sign or the existential quantifier, and thus codify such things as non-degeneracy,
finiteness, injectivity, surjectivity, invertibility, positivity, strict 
monotonicity, definiteness, genericity, etc. These conditions tend to be stable
with respect to perturbations.

3. **hybrid conditions**. These are conditions that involve too many quantifiers
and relations of both types to be either open or closed. Conditions that codify
topological, smooth, or metric structure (e.g. continuity, compactness,
completeness, connectedness, regularity) tend to be of this type (this is the 
notorious “epsilon-delta” business), as are conditions that involve subobjects
(e.g. the property of a group being simple, or a representation being irreducible).
These conditions tend to have fewer closure and stability properties than the
first two (e.g. they may only be closed or stable in sufficiently strong 
topologies). (But there are sometimes some deep and powerful rigidity theorems 
that give more closure and stability here than one might naively expect.)

Ideally, one wants to have one’s concept of a mathematical structure be both
closed under limits, and also stable with respect to perturbations, but it is 
rare that one can do both at once. Instead, one often has to have two classes 
for a single concept: a larger class of “weak” spaces that only have the closed
conditions (and so are closed under limits) but could possibly be degenerate or
singular in a number of ways, and a smaller class of “strong” spaces inside that
have the open and hybrid conditions also. A typical example: the class of Hilbert
spaces is contained inside the larger class of pre-Hilbert spaces. Another 
example: the class of smooth functions is contained inside the larger class of
distributions.

As a general rule, algebra tends to favour closed and hybrid conditions, whereas
analysis tends to favour open and hybrid conditions. Thus, in the more algebraic
part of mathematics, one usually includes degenerate elements in a class (e.g. 
the empty set is a set; a line is a curve; a square or line segment is a rectangle;
the zero morphism is a morphism; etc.), while in the more analytic parts of 
mathematics, one often excludes them (Hilbert spaces are strictly positive-definite;
topologies are usually Hausdorff (or at least T_0); traces are usually faithful; etc.)
```

<a name="#why-tricki-failed"></a>
### Why Tricki failed
([overview](#overview)

A couple quotes from Tim Gowers’ post [Is the Tricki dead?](https://gowers.wordpress.com/2010/09/24/is-the-tricki-dead/) saved for future personal reference, answering some questions I’ve had in mind for awhile (and many I hadn’t).

What was the Tricki for?

```markdown
The hope was that after the site had reached some level of completeness, it would be possible to
take a mathematics research problem (or subproblem) and search efficiently for known techniques 
that were likely to be relevant.

It would be doing something a little different from Wikipedia mathematics articles, which concentrate
more on what I like to think of as “things with names”. For instance, if you suspect that discrete 
Fourier analysis is likely to be a useful tool for your problem, then you can type “discrete Fourier 
analysis” into Google and find many links, including to a Wikipedia article that contains many of the
basic facts.

But what if it doesn’t occur to you that discrete Fourier analysis is what you need (even though it in
fact is)? The idea was that, using easily identifiable features of your problem, you would be able to
follow links to ever more specific Tricki pages until you would reach a page that explained *when* 
discrete Fourier analysis was useful and *how* it was used. In general, the whole site would be about how
to do mathematics rather than about lists of facts.
```

One of Gowers’ strongest motivations:

```markdown
the thought that one day the [automated theorem proving] programmers would be able to do all the low-level 
stuff and the Tricki would be able to tell them how to do the higher-level stuff.
```

He notes that the ‘activation energy’ required to write a Tricki article is prohibitively high:

```markdown
I still believe in this general concept, but for a wiki-type site to be successful it must reach the stage
where people think it is worth contributing. Since writing a good Tricki article takes a bit of work, the 
motivation to do it has to be particularly high. And it seems that it is not high enough for the site to 
have taken off.
```

One-time contributor Emmanuel Kowalski agrees:

```markdown
I still like the idea of the Tricki a lot. For me, the difficulty in writing more articles is that 
I feel that a Tricki article should be well-written, in a way which is different from either a blog
post, or a MathOverflow question or answer. And this means it involves more time — I typically write
blog posts in one sitting, and would dash off an answer to a MO question as I would a comment to a 
blog post, but when I wrote the only Tricki article I have done, it was more like writing a short 
survey paper. Unfortunately, time is difficult to find for such contributions, at least for me…
```

This is related to the following comment by Joseph Malkevitch:

```markdown
Unfortunately, for those contributors to Tricki who are academic mathematicians (employees of mathematics
departments) there is little career incentive to writing or developing materials of this kind.

Perhaps there might be a group of people who would volunteer to be “editors” for certain pieces of Tricki 
and when these individuals saw a post to MO, journal article, or web article, with content related to the
area they “supervise,” they could contact the author of that item to modify if for posting on Tricki. The
fact that there is less work in adapting something nice that has been done already compared with creating
something new from scratch may encourage more contributions.
```

The part about lack of career incentive reminds me of Chris Olah’s [Research Debt](https://distill.pub/2017/research-debt/) essay, under ‘Where are the Distillers?’:

```markdown
Like the theoretician, the experimentalist or the research engineer, the research distiller is an integral 
role for a healthy research community. Right now, almost no one is filling it.

Why do researchers not work on distillation? One possibility is perverse incentives, like wanting your 
work to look difficult. Those certainly exist, but we don’t think they’re the main factor.

Another possibility is that they don’t enjoy research distillation. Again, we don’t think that’s what’s
going on.

Lots of people want to work on research distillation. Unfortunately, it’s very difficult to do so, 
because we don’t support them.

An aspiring research distiller lacks many things that are easy to take for granted: a career path, places
to learn, examples and role models. Underlying this is a deeper issue: their work isn’t seen as a real 
research contribution. We need to fix this.
```

And then MO came along:

```markdown
During that time, a new factor has come into play: Mathoverflow. For the Tricki to be successful, it 
had to do something that Wikipedia doesn’t do. And now, to be successful, it would also have to do 
something that Mathoverflow doesn’t do. This is a serious point: I used to think that one of the main
functions of the Tricki would be to make it much easier for people to find out what was known about 
a problem, but Mathoverflow seems to me to be a better way of doing that. …

Is there, at least in principle, still a niche for the Tricki, or is it squeezed out by Wikipedia on 
the static side and Mathoverflow on the dynamic side?
```

What niche might Tricki still occupy that hasn’t been taken by MO?

```markdown
I’m thinking of questions along the lines of “This problem that has just emerged is of a kind I haven’t
seen before but it feels as though people ought to have thought about similar things; what should I do
now?” Obviously Mathoverflow would be useful for some such problems, but sometimes they are a bit too 
vague, sometimes one might have a subproblem that one does not wish to make public, and sometimes they 
may be sufficiently easy that one would prefer just to look up the answer rather than bother other 
people with the question.

[Also] if the Tricki became more complete, then one could browse it more systematically than either 
Wikipedia or Mathoverflow. One could for example decide to read up on all the standard techniques in
some subarea.
```

Some comments by Greg Graviton:

```markdown
First of all, I think the quality of the articles on the Tricki is excellent and well worth preserving
in form or another, for instance the discussion of homology as “linear combinations of level lines
(lines/surfaces where a function is constant)”. Most importantly, you can’t find this stuff elsewhere
except in informal discussions with other mathematicians. There ought to be a place to make that public.

Concerning the format, I think the current technology of the Tricki fails to deliver your original 
“promise” of a powerful search function, that somehow helps you from nothing to a trick that applies.
This is a hard problem, it’s not sure whether it can be solved with computers, and bolting the Tricki 
on top of a Drupal installation apparently does not really solve anything. (On the technology note, note
that MathOverflow was programmed from scratch as well, so a fresh start is quite unavoidable, not to 
mention that even small issues in usability (e.g. sluggish to load) matter a lot.)
```

I think the Tricki failed for the same reason Arbital failed: [Arbital postmortem](https://www.lesswrong.com/posts/kAgJJa3HLSZxsuSrf/arbital-postmortem). Arbital was much more ambitious in both goal and execution attempt, as you can see from reading the linked postmortem.

Continuing with Greg:

```markdown
Then, there is the “bandwidth” problem of human communication. The fastest way to convey a
mathematical concept or trick is to present it to your colleague on the blackboard. It takes 
very little effort on your part because a lot of information per time is being exchanged: mistakes,
mnemonics, steps are weighted by difficulty and importance, questions can be asked, etc. etc. 
In contrast, the amount of information that a written article can transfer is very small and it 
takes a lot of effort and skill to maximize its utility.
```

Anytime mathematical communication is brought up I’m always reminded of Bill Thurston’s essay [On proof and progress in mathematics](https://arxiv.org/abs/math/9404236), in particular this quote:

```markdown
Much of the difficulty has to do with the language and culture of mathematics, which is divided 
into subfields. Basic concepts used every day within one subfield are often foreign to another 
subfield. Mathematicians give up on trying to understand the basic concepts even from neighboring 
subfields, unless they were clued in as graduate students.

In contrast, communication works very well within the subfields of mathematics. Within a subfield,
people develop a body of common knowledge and known techniques. By informal contact, people learn 
to understand and copy each other’s ways of thinking, so that ideas can be explained clearly and easily.

Mathematical knowledge can be transmitted amazingly fast within a subfield. When a significant theorem
is proved, it often (but not always) happens that the solution can be communicated in a matter of 
minutes from one person to another within the subfield. The same proof would be communicated and
generally understood in an hour talk to members of the subfield. It would be the subject of a 15- or
20-page paper, which could be read and understood in a few hours or perhaps days by members of the 
subfield.

Why is there such a big expansion from the informal discussion to the talk to the paper? One-on-one,
people use wide channels of communication that go far beyond formal mathematical language. They use 
gestures, they draw pictures and diagrams, they make sound effects and use body language. Communication
is more likely to be two-way, so that people can concentrate on what needs the most attention. With 
these channels of communication, they are in a much better position to convey what’s going on, not
just in their logical and linguistic facilities, but in their other mental facilities as well.

In talks, people are more inhibited and more formal. Mathematical audiences are often not very good at
asking the questions that are on most people’s minds, and speakers often have an unrealistic preset 
outline that inhibits them from addressing questions even when they are asked. In papers, people are
still more formal. Writers translate their ideas into symbols and logic, and readers try to translate 
back.

People familiar with ways of doing things in a subfield recognize various patterns of statements or 
formulas as idioms or circumlocution for certain concepts or mental images. But to people not already 
familiar with what’s going on the same patterns are not very illuminating; they are often even 
misleading. The language is not alive except to those who use it.
```

Back to Greg:

```markdown
Related is the question of rewards. It’s rewarding to publish a paper (career) or book (fame), and 
it’s rewarding to talk to other people (see MathOverflow). There is no reward associated with a tricki
article, also because the appreciation by a reader happens at a different time than when the article 
is written.

However, I think there is room for the Tricki as a “MathOverflow for intuition questions”. The idea is
that a Tricki article could be initiated as a discussion between people and then transformed into a
proper article by volunteers. By the way, this is how the community wiki feature of StackOverflow/
MathOverflow was originally supposed to work. I think it’s still possible to do that, albeit with a 
software that encourages the corresponding behavior better than MathOverlfow currently does.

Again, note that building such software and community is a very hardproblem! A simple wiki software
probably won’t cut it, simply because it doesn’t encourage the right behavior. To get an impression of
its hardness, remember that Wikipedia’s success could not have been planned, it was just the fittest to
survive, and that MathOverflow didn’t get the community wiki thing right either. This is not intended to
discourage, I’d just like to point out that a successful Tricki probably needs more cleverness than is 
apparent at first.
```

Xamuel notes that “you almost have to already know what trick you need before you can search for it”:

```markdown
Take for example the problem “Prove every vector space has a basis”. If you don’t already know how
to do it, you aren’t likely to know to search for keywords like “make something maximal”, “extend
something one thing at a time”, much less “Zorn’s Lemma”.

If I were designing the Tricki, I would set it up like this. There would be articles for individual
problems, and articles about techniques. The former would link to the latter. I would then fill it up
with as many “stock” problems (mostly from undergrad math) as I could. Essentially it would be like 
[Example Problems](http://exampleproblems.com/), except, instead of just giving the solutions, it would link to the pages for the 
techniques used in the solution. As the number of problems grew, this would be much more efficient
than ultimately writing the same techniques over and over and over (which is what you’d do if you took
an Example Problems site to its logical conclusion).

So for example it would have a page “Prove every vector space has a basis” which would in turn link to
“How to use Zorn’s Lemma” as well as maybe “Partially ordering sets by inclusion”, and any other 
technique pages that might be relevant.
```

Terry Tao notes that MO takes advantage of [Metcalfe’s law](http://en.wikipedia.org/wiki/Metcalfe's_law), whereas the Tricki doesn’t:

```markdown
If N people ask questions and N people read [MO] to answer questions, there are O(N^2) opportunities 
for a question to be answered.

In contrast, to write a Tricki article, one of N people must come up with the idea and then write at 
least a stub article, and so there are only about O(N) opportunities for such an article to be created.
```

Gowers notes that MO can help Tricki:

```markdown
One of the difficulties in writing a Tricki article is that it can be hard to think of examples. 
For example (!) I know that the trick of making something easier by generalizing it is frequently
useful. But if I try to think of a good example my mind goes a bit blank, which is part of the reason
I have not written such an article.

However, the job has just got easier: if I post a big-list question on MO asking for good examples of
this technique, I can be pretty sure of getting some excellent ones. Then I can base an article on
people’s answers and include a link to the MO discussion (partly to credit people with their help, and
partly because the discussion will be different and will therefore offer more than the Tricki article
on its own).
```

Vipul Naik contends that what the Tricki needed was at least a handful of super-passionate contributors, probably in the vein of [r/slatestarcodex - Most of What You Read on the Internet is Written by Insane People](https://www.reddit.com/r/slatestarcodex/comments/9rvroo/most_of_what_you_read_on_the_internet_is_written/):

```markdown
I think there’s a general perception here that what needs to be done is get a large number of 
contributors. But I think that at this stage, if the Tricki needs to grow, it needs just 2-5 very 
passionate contributors, who agitate day and night about continually improving the organisation, 
adding new articles, etc. Large numbers of diffused contributions could take over at a later stage,
but they won’t do the trick at this stage.

For instance, the psychology wiki here: http://psychology.wikia.com/wiki... was written almost 
completely by one person at least for the first few years — now there are contributions from large
numbers of people.

The story is a little different with something like Math Overflow, because it is not primarily an 
information corpus as a place to ask and answer questions. But even there, it is the dedicated few 
who monitor the site who made sure that it took off. The need for that “dedicated few” in the case 
of the Tricki would be substantially more.
```

Commenter probable trickipedian mentions non-academic mathematicians as potential contributors, due to their specialized domain knowledge:

```markdown
One likely source of Tricki contributors – not for deep mathematics, but useful applied math “tricks”
– would be people who use mathematics for our research, but are not necessarily academic mathematicians.
For instance, I have (over the years) built a collection of definite integrals not found in standard 
“tables of integrals”; because they occur in (my) somewhat obscure research area, they are generally 
unknown outside it.

I (obviously) cannot publish such work in the journals of my discipline, and the techniques are too 
classical and elementary to constitute modern mathematics research, but it would be nice if I could 
post them on a well-trafficked public venue and someone else found it useful. I could supply (weak) 
proofs or justifications for them and have verified them to the best of my abilities, though the proofs
would certainly not meet the standards of rigor required by pure mathematicians. If a mathematician
could ‘vet’ them, I would be pleased to get a login and contribute.
```

Phi. Isett argues that the Tricki could be enhanced by integrating it with online, publicly-written math books:

```markdown
For example, usually a textbook will use a well-known and common trick at some stage in a proof, but 
will rarely have the opportunity to give much insight into the trick itself, its origins, its limits,
alternative methods, etc. All too often, the first time you see a trick, it is also much more complicated
than the most basic example of its use, which makes it harder to digest. Imagine you learned the Fourier
transform before you ever diagonalized a matrix… You might not know why it has certain magical properties
when it comes to translations and differentiation — in any event, it’s useful to understand that 
diagonalizing commuting operators is a truly general trick.

Often the trick appears as an ingenious technical detail in a proof. For example: the proof of Sard’s 
theorem uses this trick you might call “decomposing the total change into small changes”. ...You may 
recognize this trick from a proof of the Fundamental Theorem of Calculus, but maybe you didn’t see it
coming. Or you might find it enlightening to see the same trick in other contexts and in a much more 
general light. If you can link to the Tricki, then the individual techniques can be explored separately
and generally without disturbing the flow of the exposition.
```

<a name="#solving-famous-open-problems"></a>
### Solving famous open problems
([overview](#overview))

(See also Scott Aaronson on [making progress on big problems](#general-philosophy) in philosophy.)

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

Michael Nielsen has [a great essay](http://cognitivemedium.com/srs-mathematics) talking about how he used spaced repetition via Anki flashcards to iteratively deepen his understanding of ("see through") a math concept. See also [Nielsen on augmenting long-term memory](#augmenting-long-term-memory). 

First -- on understanding in math being not black and white but layered / spectrum:

```markdown
What does it mean to understand a piece of mathematics? Naively, we perhaps think of this 
in relatively black and white terms: initially you don’t understand a piece of mathematics,
then you go through a brief grey period where you’re learning it, and with some luck and 
hard work you emerge out the other side “understanding” the mathematics.

In reality, mathematical understanding is much more nuanced. My experience is that it’s
nearly always possible to deepen one’s understanding of any piece of mathematics. This is 
even true – perhaps especially true – of what appear to be very simple mathematical ideas.

I first really appreciated this after reading an essay by the mathematician Andrey Kolmogorov.
You might suppose a great mathematician such as Kolmogorov would be writing about some very 
complicated piece of mathematics, but his subject was the humble equals sign: what made it a
good piece of notation, and what its deficiencies were. Kolmogorov discussed this in loving 
detail, and made many beautiful points along the way, e.g., that the invention of the equals
sign helped make possible notions such as equations (and algebraic manipulations of equations).

Prior to reading the essay I thought I understood the equals sign. Indeed, I would have been
offended by the suggestion that I did not. But the essay showed convincingly that I could 
understand the equals sign much more deeply.

This experience suggested three broader points. First, it’s possible to understand other 
pieces of mathematics far more deeply than I assumed. Second, mathematical understanding 
is an open-ended process; it’s nearly always possible to go deeper. Third, even great
mathematicians – perhaps, especially, great mathematicians – thought it worth their time
to engage in such deepening.
```

Nielsen being Nielsen, he gets excited about how to make iterative deepening of mathematical understanding actionable via heuristics. He's collected "many such heuristics over the years"; his essay talks about Anki. 

Does this really depend on Anki though? Not really:

```markdown
There’s very little in the above process that explicitly depended on me using Anki’s spaced-
repetition flashcards. Rather, what I’ve described is a general process for pulling apart 
the proof of a theorem and making much more sense of it, essentially by atomizing the 
elements. There’s no direct connection to Anki at all – you could carry out the process 
using paper and pencil.
```

Here's the "Ankification" of the proof of the following theorem: "a complex normal matrix is always diagonalizable by a unitary matrix".

```markdown
*Phase I: understanding the proof*: This involves multiple passes over the proof. Initially,
it starts out with what I think of as grazing, picking out single elements of the proof and 
converting to Anki cards. ... 

I work hard to restate ideas in multiple ways. Indeed, I worked hard to simplify both questions
and answers – the just given question-and-answer pair started out somewhat more complicated.
Part of this was some minor complexity in the question, which I gradually trimmed down. The 
answer I’ve stated above, though, is much better than in earlier versions. Earlier versions
mentioned M explicitly (unnecessary), had more blocks in the matrices, used ⋯⋯ rather than 
⋅⋅, and so on. You want to aim for the minimal answer, displaying the core idea as sharply as 
possible. 

I can’t emphasize enough the value of finding multiple different ways of thinking about the
“same” mathematical ideas. Here’s a couple more related restatements:

*Q: What’s a geometric interpretation of the diagonal entries in the matrix MM†?

A: The lengths squared of the respective rows.

Q: What’s a geometric interpretation of the diagonal entries in the matrix M†M?

A: The lengths squared of the respective columns.

Q: What do the diagonal elements of the normalcy condition MM†=M†M mean geometrically?

A: The corresponding row and column lengths are the same.*

What you’re trying to do at this stage is learn your way around the proof. Every piece
should become a comfortable part of your mental furniture, ideally something you start to
really feel. That means understanding every idea in multiple ways, and finding as many 
connections between different ideas as possible.

People inexperienced at mathematics sometimes memorize proofs as linear lists of statements.
A more useful way is to think of proofs is as interconnected networks of simple observations.
Things are rarely true for just one reason; finding multiple explanations for things gives 
you an improved understanding. This is in some sense “inefficient”, but it’s also a way of
deepening understanding and improving intuition. You’re building out the network of the proof,
making more connections between nodes.

One way of doing this is to explore minor variations. ...

(By the way, it’s questions like these that make me think it helps to be fairly 
mathematically experienced in carrying this Ankification process out. For someone who has
done a lot of linear algebra these are very natural observations to make, and questions to
ask. But I’m not sure they would be so natural for everyone. The ability to ask the “right”
questions – insight-generating questions – is a limiting part of this whole process, and
requires some experience.)

I’ve been describing the grazing process, aiming to thoroughly familiarize yourself with
every element of the proof. This is useful, but is also a rather undirected process, with 
no clear end point, and not necessarily helping you understand the broader to structure of
the proof. I also impose on myself a set of aspirational goals, all variations on the idea 
of distilling the entire proof to one question and (simple) answer. The aim is to fill in 
the answers to questions having forms like:

*Q: In one sentence, what is the core reason a (complex) normal matrix is diagonalizable?

And:

Q: What is a simple visual representation of the proof that (complex) normal matrices are
diagonalizable?*

I think of these question templates as boundary conditions or forcing functions. They’re 
things to aim for, and I try to write questions that will help me move toward answers. That 
starts with grazing, but over time moves to more structural questions about the proof, and
about how elements fit together.

In general, it’s helpful to make both questions and answers as atomic as possible; it seems
to help build clarity. That atomicity doesn’t mean the questions and answers can’t involve 
quite sophisticated concepts, but they ideally express a single idea.

In practice, as I understand the proof better and better the aspirational goal cards change
their nature somewhat.

What you really want is to feel every element (and the connections between them) in your 
bones. Some substantial part of that feeling comes by actually constructing the cards. That’s
a feeling you can’t get merely by reading an essay, it can only be experienced by going
through the deep Ankification process yourself. Nonetheless, I find that process, as described
up to now, is also not quite enough. You can improve upon it by asking further questions
elaborating on different parts of the answer, with the intent of helping you understand the
answer better.

Another helpful trick is to have multiple ways of writing these top-level questions. Much of 
my thinking is non-verbal (especially in subjects I’m knowledgeable about), but I still find
it useful to force a verbal question-and-answer...

*Phase II: variations, pushing the boundaries*: Let’s get back to details of how the
Ankification process works. One way of deepening your understanding further is to find ways
of pushing the boundaries of the proof and of the theorem. I find it helpful to consider many
different ways of changing the assumptions of the theorem, and to ask how it breaks down (or
generalizes). Another good strategy is to ask if the conditions can be weakened. ...

This second phase really is open-ended: we can keep putting in variations essentially ad 
infinitum. The questions are no longer directly about the proof, but rather are about poking
it in various ways, and seeing what happens. The further I go, and the more I connect to other
results, the better.
```

"Exhaust" cards:

```markdown
As described, this deep Ankification process can feel rather wasteful. Inevitably, over 
time my understanding of the proof changes. When that happens it’s often useful to rewrite
(and sometimes discard or replace) cards to reflect my improved understanding. And some of
the cards written along the way have the flavor of exhaust, bad cards that seem to be
necessary to get to good cards. I wish I had a good way of characterizing these, but I 
haven’t gone through this often enough to have more than fuzzy ideas about it.
```

How it feels like to "be inside a piece of mathematics":

```markdown
Typically, my mathematical work begins with paper-and-pen and messing about, often in
a rather ad hoc way. But over time if I really get into something my thinking starts to
change. I gradually internalize the mathematical objects I’m dealing with. It becomes 
easier and easier to conduct (most of) my work in my head. I will go on long walks, and
simply think intensively about the objects of concern. Those are no longer symbolic or 
verbal or visual in the conventional way, though they have some secondary aspects of 
this nature. Rather, the sense is somehow of working directly with the objects of 
concern, without any direct symbolic or verbal or visual referents. Furthermore, as my 
understanding of the objects change – as I learn more about their nature, and correct my
own misconceptions – my sense of what I can do with the objects changes as well. It’s as
though they sprout new affordances, in the language of user interface design, and I get 
much practice in learning to fluidly apply those affordances in multiple ways.

This is a very difficult experience to describe in a way that I’m confident others will
understand, but it really is central to my experience of mathematics – at least, of 
mathematics that I understand well. I must admit I’ve shared it with some trepidation; 
it seems to be rather unusual for someone to describe their inner mathematical experiences
in these terms (or, more broadly, in the terms used in this essay).
```

Related is Einstein's musings in his letter to Hadamard describing his thought processes:

```markdown
The words or the language, as they are written or spoken, do not seem to play any role 
in my mechanism of thought. The psychical entities which seem to serve as elements in 
thought are certain signs and more or less clear images which can be “voluntarily” 
reproduced and combined… The above-mentioned elements are, in my case, of visual and some
of muscular type. Conventional words or other signs have to be sought for laboriously 
only in a secondary stage, when the mentioned associative play is sufficiently established
and can be reproduced at will.
```

Nielsen thinks this is all chunking:

```markdown
People who intensively study a subject gradually start to build mental libraries of “chunks” 
– large-scale patterns that they recognize and use to reason. This is why some grandmaster 
chess players can remember thousands of games move for move. They’re not remembering the 
individual moves – they’re remembering the ideas those games express, in terms of larger 
patterns. And they’ve studied chess so much that those ideas and patterns are deeply
meaningful, much as the phrases in a lover’s letter may be meaningful. It’s why top 
basketball players have extraordinary recall of games. Experts begin to think, perhaps only
semi-consciously, using such chunks. The conventional representations – words or symbols in
mathematics, or moves on a chessboard – are still there, but they are somehow secondary.
```

This segues into Terry Tao's [three stages of mathematical education](https://terrytao.wordpress.com/career-advice/theres-more-to-mathematics-than-rigour-and-proofs/) article:

```markdown
One can roughly divide mathematical education into three stages:

1. The “pre-rigorous” stage, in which mathematics is taught in an informal, intuitive 
manner, based on examples, fuzzy notions, and hand-waving. (For instance, calculus is 
usually first introduced in terms of slopes, areas, rates of change, and so forth.) 
The emphasis is more on computation than on theory. This stage generally lasts until 
the early undergraduate years.

2. The “rigorous” stage, in which one is now taught that in order to do maths “properly”,
one needs to work and think in a much more precise and formal manner (e.g. re-doing calculus
by using epsilons and deltas all over the place). The emphasis is now primarily on theory;
and one is expected to be able to comfortably manipulate abstract mathematical objects
without focusing too much on what such objects actually “mean”. This stage usually occupies 
the later undergraduate and early graduate years.

3. The “post-rigorous” stage, in which one has grown comfortable with all the rigorous 
foundations of one’s chosen field, and is now ready to revisit and refine one’s pre-
rigorous intuition on the subject, but this time with the intuition solidly buttressed by 
rigorous theory. (For instance, in this stage one would be able to quickly and accurately 
perform computations in vector calculus by using analogies with scalar calculus, or informal
and semi-rigorous use of infinitesimals, big-O notation, and so forth, and be able to 
convert all such calculations into a rigorous argument whenever required.) The emphasis is 
now on applications, intuition, and the “big picture”. This stage usually occupies the late
graduate years and beyond.

The transition from the first stage to the second is well known to be rather traumatic, with
the dreaded “proof-type questions” being the bane of many a maths undergraduate. But the
transition from the second to the third is equally important, and should not be forgotten.

It is of course vitally important that you know how to think rigorously, as this gives you
the discipline to avoid many common errors and purge many misconceptions. Unfortunately, this
has the unintended consequence that “fuzzier” or “intuitive” thinking (such as heuristic
reasoning, judicious extrapolation from examples, or analogies with other contexts such as 
physics) gets deprecated as “non-rigorous”. All too often, one ends up discarding one’s
initial intuition and is only able to process mathematics at a formal level, thus getting 
stalled at the second stage of one’s mathematical education.  (Among other things, this can
impact one’s ability to read mathematical papers; an overly literal mindset can lead to 
“compilation errors” when one encounters even a single typo or ambiguity in such a paper.)

The point of rigour is not to destroy all intuition; instead, it should be used to destroy 
bad intuition while clarifying and elevating good intuition. It is only with a combination
of both rigorous formalism and good intuition that one can tackle complex mathematical
problems; one needs the former to correctly deal with the fine details, and the latter to 
correctly deal with the big picture. Without one or the other, you will spend a lot of time
blundering around in the dark (which can be instructive, but is highly inefficient). So once
you are fully comfortable with rigorous mathematical thinking, you should revisit your
intuitions on the subject and use your new thinking skills to test and refine these intuitions
rather than discard them. One way to do this is to ask yourself dumb questions; another is 
to relearn your field.

The ideal state to reach is when every heuristic argument naturally suggests its rigorous 
counterpart, and vice versa. Then you will be able to tackle maths problems by using both 
halves of your brain at once – i.e., the same way you already tackle problems in “real life”.
```

See [this article](https://terrytao.wordpress.com/advice-on-writing-papers/on-compilation-errors-in-mathematical-reading-and-how-to-resolve-them/) by Terry for more on compilation errors.

The kind of mistakes made by mathematicians of each stage:

```markdown
It is perhaps worth noting that mathematicians at all three of the above stages of 
mathematical development can still make formal mistakes in their mathematical writing.
However, the nature of these mistakes tends to be rather different, depending on what 
stage one is at:

1. Mathematicians at the pre-rigorous stage of development often make formal errors 
because they are unable to understand how the rigorous mathematical formalism actually 
works, and are instead applying formal rules or heuristics blindly.  It can often be 
quite difficult for such mathematicians to appreciate and correct these errors even 
when those errors are explicitly pointed out to them.

2. Mathematicians at the rigorous stage of development can still make formal errors
because they have not yet perfected their formal understanding, or are unable to perform
enough “sanity checks” against intuition or other rules of thumb to catch, say, a sign
error, or a failure to correctly verify a crucial hypothesis in a tool.  However, such 
errors can usually be detected (and often repaired) once they are pointed out to them.

3. Mathematicians at the post-rigorous stage of development are not infallible, and are
still capable of making formal errors in their writing.  But this is often because they
no longer need the formalism in order to perform high-level mathematical reasoning, and 
are actually proceeding largely through intuition, which is then translated (possibly 
incorrectly) into formal mathematical language.

The distinction between the three types of errors can lead to the phenomenon (which can
often be quite puzzling to readers at earlier stages of mathematical development) of a 
mathematical argument by a post-rigorous mathematician which locally contains a number
of typos and other formal errors, but is globally quite sound, with the local errors 
propagating for a while before being cancelled out by other local errors.  (In contrast,
when unchecked by a solid intuition, once an error is introduced in an argument by a pre-
rigorous or rigorous mathematician, it is possible for the error to propagate out of 
control until one is left with complete nonsense at the end of the argument.)
```

Commenter Chris makes the following claim:

```markdown
I’d call pre-rigorous the “cargo cult” stage. You’re not doing mathematics, you’re merely
performing a very close approximation to it using rote learned rules. It was this sort of
mathematics taught in the first year of the undergraduate curriculum at my university which 
caused me to take physics as my major.

Physicists and engineers call the third type of mathematics you propose a “back of the
envelope” calculation. I suspect the less pretentious mathematicians do also. It is the
step you use to flesh out a hypothesis before you apply rigour.
```

I only recorded it as context for Terry's response:

```markdown
Hmm. I think perhaps I would classify the “back of the envelope” calculations as a 
fourth stage, let’s call it the “heuristic” stage, in the following, almost commuting square:

pre-rigorous —> rigorous
| ……………………….|
v ……………………….v
heuristic —> post-rigorous

As I discussed in the post, mathematicians tend to proceed through the upper route, but I
do see the point that physicists and engineers tend to proceed through the lower route. 
Though, as I said, the diagram doesn’t quite commute; there are some significant cultural
differences in doing mathematics that depend on which route one took to achieve the post-
rigorous stage.

The distinction between heuristic and post-rigorous is that in the latter, one uses
intuition and rigour in an integrated fashion; one knows how to justify one’s intuition
and convert it to rigorous arguments, and conversely one knows how to take rigorous 
arguments and extract an intuitive explanation. For instance, one could convert arguments
involving infinitesimals into rigorous epsilon-delta arguments whenever required, and vice
versa. At the heuristic level, one could argue accurately with infinitesimals, but might 
not be able to convert them into a rigorous argument.

Just as mathematicians sometimes get stuck at the rigorous stage, unable to fully develop
their intuition, I would imagine that the converse problem can happen to people educated 
using the physicist/engineer approach, who then miss out on the stereoscopic view that one
gets from using both rigour and intuition simultaneously.
```

Going back to Nielsen's chunking above, there's also Bill Thurston's legendary MO question [Thinking and explaining](https://mathoverflow.net/questions/38639/thinking-and-explaining), whose favorite answers I'm quoting wholesale below.

Here's the [legendary answer by Anonymous Quoran](https://www.quora.com/What-is-it-like-to-understand-advanced-mathematics-Does-it-feel-analogous-to-having-mastery-of-another-language-like-in-programming-or-linguistics/answers/873950?amp&share=1&srid=p6KQ) I always have to much around in the Google search results to get at for some reason:

```markdown
**You can answer many seemingly difficult questions quickly**. But you are not very impressed
by what can look like magic, because you know the trick. The trick is that your brain can
quickly decide if a question is answerable by one of a few powerful general purpose "machines"
(e.g., continuity arguments, the correspondences between geometric and algebraic objects,
linear algebra, ways to reduce the infinite to the finite through various forms of
compactness) combined with specific facts you have learned about your area. The number of
fundamental ideas and techniques that people use to solve problems is, perhaps surprisingly,
pretty small -- see http://www.tricki.org/tricki/map for a partial list, maintained by Timothy
Gowers.

**You are often confident that something is true long before you have an airtight proof for it
(this happens especially often in geometry)**. The main reason is that you have a large 
catalogue of connections between concepts, and you can quickly intuit that if X were to be 
false, that would create tensions with other things you know to be true, so you are inclined 
to believe X is probably true to maintain the harmony of the conceptual space. It's not so much 
that you can imagine the situation perfectly, but you can quickly imagine many other things that
are logically connected to it.

**You are comfortable with feeling like you have no deep understanding of the problem you are 
studying**. Indeed, when you do have a deep understanding, you have solved the problem and it 
is time to do something else. This makes the total time you spend in life reveling in your mastery
of something quite brief. One of the main skills of research scientists of any type is knowing how
to work comfortably and productively in a state of confusion. More on this in the next few bullets.

**Your intuitive thinking about a problem is productive and usefully structured, wasting little 
time on being aimlessly puzzled**. For example, when answering a question about a high-dimensional
space (e.g., whether a certain kind of rotation of a five-dimensional object has a "fixed point"
which does not move during the rotation), you do not spend much time straining to visualize those 
things that do not have obvious analogues in two and three dimensions. (Violating this principle
is a huge source of frustration for beginning maths students who don't know that they shouldn't be
straining to visualize things for which they don't seem to have the visualizing machinery.) Instead...

**When trying to understand a new thing, you automatically focus on very simple examples that 
are easy to think about, and then you leverage intuition about the examples into more impressive
insights**. For example, you might imagine two- and three-dimensional rotations that are analogous
to the one you really care about, and think about whether they clearly do or don't have the 
desired property. Then you think about what was important to the examples and try to distill those
ideas into symbols. Often, you see that the key idea in the symbolic manipulations doesn't depend
on anything about two or three dimensions, and you know how to answer your hard question. 

**As you get more mathematically advanced, the examples you consider easy are actually complex 
insights built up from many easier examples; the "simple case" you think about now took you two
years to become comfortable with**. But at any given stage, you do not strain to obtain a magical
illumination about something intractable; you work to reduce it to the things that feel friendly.

To me, **the biggest misconception that non-mathematicians have about how mathematicians work is that 
there is some mysterious mental faculty that is used to crack a research problem all at once**. It's 
true that sometimes you can solve a problem by pattern-matching, where you see the standard tool 
that will work; the first bullet above is about that phenomenon. This is nice, but not fundamentally
more impressive than other confluences of memory and intuition that occur in normal life, as when
you remember a trick to use for hanging a picture frame or notice that you once saw a painting of 
the street you're now looking at.

In any case, by the time a problem gets to be a research problem, it's almost guaranteed that
simple pattern matching won't finish it. So in one's professional work, the process is piecemeal:
you think a few moves ahead, trying out possible attacks from your arsenal on simple examples 
relating to the problem, trying to establish partial results, or looking to make analogies with 
other ideas you understand. This is the same way that you solve difficult problems in your first
real maths courses in university and in competitions. What happens as you get more advanced is 
simply that the arsenal grows larger, the thinking gets somewhat faster due to practice, and you
have more examples to try. Sometimes, during this process, a sudden insight comes, but it would 
not be possible without the painstaking groundwork [ http://terrytao.wordpress.com/ca... ].

Indeed, most of the bullet points here summarize feelings familiar to many serious students of 
mathematics who are in the middle of their undergraduate careers; as you learn more mathematics,
these experiences apply to "bigger" things but have the same fundamental flavor.

**You go up in abstraction, "higher and higher"**. The main object of study yesterday becomes 
just an example or a tiny part of what you are considering today. For example, in calculus
classes you think about functions or curves. In functional analysis or algebraic geometry, you
think of spaces whose points are functions or curves -- that is, you "zoom out" so that every
function is just a point in a space, surrounded by many other "nearby" functions. Using this 
kind of zooming out technique, you can say very complex things in short sentences -- things 
that, if unpacked and said at the zoomed-in level, would take up pages. Abstracting and 
compressing in this way makes it possible to consider extremely complicated issues with one's 
limited memory and processing power.

**The particularly "abstract" or "technical" parts of many other subjects seem quite accessible
because they boil down to maths you already know. You generally feel confident about your ability
to learn most quantitative ideas and techniques**. A theoretical physicist friend likes to say, 
only partly in jest, that there should be books titled "______ for Mathematicians", where _____ 
is something generally believed to be difficult (quantum chemistry, general relativity, securities
pricing, formal epistemology). Those books would be short and pithy, because many key concepts in 
those subjects are ones that mathematicians are well equipped to understand. Often, those parts 
can be explained more briefly and elegantly than they usually are if the explanation can assume a
knowledge of maths and a facility with abstraction. 

Learning the domain-specific elements of a different field can still be hard -- for instance,
physical intuition and economic intuition seem to rely on tricks of the brain that are not 
learned through mathematical training alone. But the quantitative and logical techniques you 
sharpen as a mathematician allow you to take many shortcuts that make learning other fields
easier, as long as you are willing to be humble and modify those mathematical habits that are 
not useful in the new field.

**You move easily among multiple seemingly very different ways of representing a problem**. For
example, most problems and concepts have more algebraic representations (closer in spirit to an 
algorithm) and more geometric ones (closer in spirit to a picture). You go back and forth between
them naturally, using whichever one is more helpful at the moment. 

Indeed, some of the most powerful ideas in mathematics (e.g., duality, Galois theory, algebraic
geometry) provide "dictionaries" for moving between "worlds" in ways that, ex ante, are very 
surprising. For example, Galois theory allows us to use our understanding of symmetries of shapes
(e.g., rigid motions of an octagon) to understand why you can solve any fourth-degree polynomial
equation in closed form, but not any fifth-degree polynomial equation. Once you know these threads
between different parts of the universe, you can use them like wormholes to extricate yourself 
from a place where you would otherwise be stuck. The next two bullets expand on this.

**Spoiled by the power of your best tools, you tend to shy away from messy calculations or long,
case-by-case arguments unless they are absolutely unavoidable**. Mathematicians develop a powerful
attachment to elegance and depth, which are in tension with, if not directly opposed to, mechanical
calculation. Mathematicians will often spend days figuring out why a result follows easily from some 
very deep and general pattern that is already well-understood, rather than from a string of 
calculations. Indeed, you tend to choose problems motivated by how likely it is that there will be 
some "clean" insight in them, as opposed to a detailed but ultimately unenlightening proof by
exhaustively enumerating a bunch of possibilities. (Nevertheless, detailed calculation of an example 
is often a crucial part of beginning to see what is really going on in a problem; and, depending on
the field, some calculation often plays an essential role even in the best proof of a result.)

In A Mathematician's Apology [http://www.math.ualberta.ca/~mss..., the most poetic book I know on what it is "like" to be a mathematician], G.H. Hardy wrote:

"In both [these example] theorems (and in the theorems, of course, I include the proofs) there is a
very high degree of unexpectedness, combined with inevitability and  economy. The arguments take so
odd and surprising a form; the weapons used seem so childishly simple when compared with  the far-
reaching results; but there is no escape from the conclusions. There are no complications of detail—
one line of attack is enough in each case; and this is true too of the proofs of many much more 
difficult theorems, the full appreciation of which demands quite a high degree of technical
proficiency. We do not want many ‘variations’ in the proof of a mathematical theorem: ‘enumeration 
of cases’, indeed, is one of the duller forms of mathematical argument. A mathematical proof should
resemble a simple and clear-cut constellation, not a scattered cluster in the Milky Way."

[...]

"[A solution to a difficult chess problem] is quite genuine mathematics, and has its merits; but it
is just that ‘proof by enumeration of cases’ (and of cases which do not, at bottom, differ at all
profoundly) which a real mathematician tends to despise."

**You develop a strong aesthetic preference for powerful and general ideas that connect hundreds of
difficult questions, as opposed to resolutions of particular puzzles**. Mathematicians don't really
care about "the answer" to any particular question; even the most sought-after theorems, like
Fermat's Last Theorem, are only tantalizing because their difficulty tells us that we have to 
develop very good tools and understand very new things to have a shot at proving them. It is
what we get in the process, and not the answer per se, that is the valuable thing. The 
accomplishment a mathematician seeks is finding a new dictionary or wormhole between different 
parts of the conceptual universe. As a result, many mathematicians do not focus on deriving the 
practical or computational implications of their studies (which can be a drawback of the hyper-
abstract approach!); instead, they simply want to find the most powerful and general connections.
Timothy Gowers has some interesting comments on this issue, and disagreements within the 
mathematical community about it [ http://www.dpmms.cam.ac.uk/~wtg1... ].

**Understanding something abstract or proving that something is true becomes a task a lot like
building something**. You think: "First I will lay this foundation, then I will build this framework
using these familiar pieces, but leave the walls to fill in later, then I will test the beams..." 
All these steps have mathematical analogues, and structuring things in a modular way allows you to 
spend several days thinking about something you do not understand without feeling lost or frustrated.
(I should say, "without feeling unbearably lost and frustrated"; some amount of these feelings is 
inevitable, but the key is to reduce them to a tolearable degree.)

Andrew Wiles, who proved Fermat's Last Theorem, used an "exploring" metaphor:

"Perhaps I can best describe my experience of doing mathematics in terms of a journey through a
dark unexplored mansion. You enter the first room of the mansion and it's completely dark. You 
stumble around bumping into the furniture, but gradually you learn where each piece of furniture
is. Finally, after six months or so, you find the light switch, you turn it on, and suddenly it's
all illuminated. You can see exactly where you were. Then you move into the next room and spend 
another six months in the dark. So each of these breakthroughs, while sometimes they're momentary,
sometimes over a period of a day or two, they are the culmination of—and couldn't exist without—
the many months of stumbling around in the dark that proceed them." [ http://www.pbs.org/wgbh/nova/phy... ]

**In listening to a seminar or while reading a paper, you don't get stuck as much as you used to**
in youth because you are good at modularizing a conceptual space, taking certain calculations or
arguments you don't understand as "black boxes", and considering their implications anyway. You
can sometimes make statements you know are true and have good intuition for, without understanding
all the details. You can often detect where the delicate or interesting part of something is based
on only a very high-level explanation. (I first saw these phenomena highlighted by Ravi Vakil, who
offers insightful advice on being a mathematics student: http://math.stanford.edu/~vakil/... .)

**You are good at generating your own definitions and your own questions in thinking about some new
kind of abstraction**. One of the things one learns fairly late in a typical mathematical education 
(often only at the stage of starting to do research) is how to make good, useful definitions.
Something I've reliably heard from people who know parts of mathematics well but never went on to be
professional mathematicians (i.e., write articles about new mathematics for a living) is that they
were good at proving difficult propositions that were stated in a textbook exercise, but would be
lost if presented with a mathematical structure and asked to find and prove some interesting facts 
about it. Concretely, the ability to do this amounts to being good at making definitions and, using
the newly defined concepts, formulating precise results that other mathematicians find intriguing or
enlightening. 

This kind of challenge is like being given a world and asked to find events in it that come together 
to form a good detective story. You have to figure out who the characters should be (the concepts 
and objects you define) and what the interesting mystery might be. To do these things, you use 
analogies with other detective stories (mathematical theories) that you know and a taste for what
is surprising or deep. How this process works is perhaps the most difficult aspect of mathematical
work to describe precisely but also the thing that I would guess is the strongest thing that 
mathematicians have in common.

**You are easily annoyed by imprecision in talking about the quantitative or logical**. This is
mostly because you are trained to quickly think about counterexamples that make an imprecise claim
seem obviously false.

**On the other hand, you are very comfortable with intentional imprecision or "hand-waving" in areas
you know, because you know how to fill in the details**. Terence Tao is very eloquent about this here 
[ http://terrytao.wordpress.com/ca... ]: 

"[After learning to think rigorously, comes the] 'post-rigorous' stage, in which one has grown 
comfortable with all the rigorous foundations of one’s chosen field, and is now ready to revisit
and refine one’s pre-rigorous intuition on the subject, but this time with the intuition solidly
buttressed by rigorous theory. (For instance, in this stage one would be able to quickly and 
accurately perform computations in vector calculus by using analogies with scalar calculus, or
informal and semi-rigorous use of infinitesimals, big-O notation, and so forth, and be able to
convert all such calculations into a rigorous argument whenever required.) The emphasis is now 
on applications, intuition, and the 'big picture'. This stage usually occupies the late graduate
years and beyond."

In particular, an idea that took hours to understand correctly the first time ("for any arbitrarily
small epsilon I can find a small delta so that this statement is true") becomes such a basic element
of your later thinking that you don't give it conscious thought.

Before wrapping up, it is worth mentioning that mathematicians are not immune to the limitations 
faced by most others. They are not typically intellectual superheroes. For instance, they often 
become resistant to new ideas and uncomfortable with ways of thinking (even about mathematics) 
that are not their own. They can be defensive about intellectual turf, dismissive of others, or
petty in their disputes. Above, I have tried to summarize how the mathematical way of thinking 
feels and works at its best, without focusing on personality flaws of mathematicians or on the 
politics of various mathematical fields. These issues are worthy of their own long answers!

**You are humble about your knowledge because you are aware of how weak maths is, and you are comfortable
with the fact that you can say nothing intelligent about most problems**. There are only very few
mathematical questions to which we have reasonably insightful answers. There are even fewer questions,
obviously, to which any given mathematician can give a good answer. After two or three years of a 
standard university curriculum, a good maths undergraduate can effortlessly write down hundreds of
mathematical questions to which the very best mathematicians could not venture even a tentative answer.
(The theoretical computer scientist Richard Lipton lists some examples of potentially "deep" ignorance 
here: http://rjlipton.wordpress.com/20...) This makes it more comfortable to be stumped by most problems;
a sense that you know roughly what questions are tractable and which are currently far beyond our abilities
is humbling, but also frees you from being very intimidated, because you do know you are familiar with the
most powerful apparatus we have for dealing with these kinds of problems.
```

Ravi Vakil's [advice page](http://math.stanford.edu/~vakil/potentialstudents.html) for potential PhD students has some great quotes. The most memorable is this one:

```markdown
Here's a phenomenon I was surprised to find: you'll go to talks, and hear various words, whose 
definitions you're not so sure about. At some point you'll be able to make a sentence using those
words; you won't know what the words mean, but you'll know the sentence is correct. You'll also 
be able to ask a question using those words. You still won't know what the words mean, but you'll
know the question is interesting, and you'll want to know the answer. Then later on, you'll learn 
what the words mean more precisely, and your sense of how they fit together will make that learning
much easier. 

The reason for this phenomenon is that mathematics is so rich and infinite that it is impossible to 
learn it systematically, and if you wait to master one topic before moving on to the next, you'll 
never get anywhere. Instead, you'll have tendrils of knowledge extending far from your comfort zone. 
Then you can later backfill from these tendrils, and extend your comfort zone; this is much easier 
to do than learning "forwards". 

(Caution: this backfilling is necessary. There can be a temptation to learn lots of fancy words and
to use them in fancy sentences without being able to say precisely what you mean. You should feel 
free to do that, but you should always feel a pang of guilt when you do.)
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

<a name="#Solving-math-problems-terribly"></a>
### Solving math problems terribly
([overview](#overview))

From Alon Amit's wonderful essay [Solving math problems terribly](https://qr.ae/TUnpLe):

```markdown
When you solve a math problem, especially a hard one, there’s a profound sense of
accomplishment accompanied by a need to share your masterpiece with the world. In doing 
so, most people’s instinct is to present the solution in its most pristine, elegant,
nicely worked-out form. This works well to impress, but not so well to teach.

After all, your path to discovery almost certainly didn’t land on that clean, elegant 
solution right away. You stumbled, fumbled and groped in the dark for a while, you tried
various things that failed, you hit on the right path only thanks to some instinct or 
intuition or methodology that makes sense to you but is hard to describe, and so on. All
of that stuff is, lamentably, missing from the vast majority of research papers, “solutions
to exercises” appendices, and even most worked-out solutions on places like AoPS, where 
ostensibly the goal is to help people become better problem solvers.

On several occasions on Quora, I resisted the urge to present a short, glamorous solution
to a problem, and instead revealed in painful detail the false turns, stupid blunders and 
failed attempts I went through as I was solving it...

I like that. I think it’s helpful, I think it’s not done often enough, and I think
presenting the most elegant solution can be downright harmful. It makes readers feel it’s
magic, and they would have had no chance of discovering it themselves. It can be 
intimidating and makes math look like voodoo. It’s not. Many things that look like strokes 
of genius are actually the result of very methodical and organized efforts.

So, in the future, I intend to keep doing that as much as I can. And when I do, I don’t 
want to spend the first few paragraphs of every such answer explaining my rationale. ...

Please keep in mind:

1. This approach will make many of my answers *long*. Don’t be intimidated by that. I could
have made them 90% shorter and 100% more mysterious. If you’re genuinely interested in 
learning how to solve math problems, I hope that my revealing the meandering path is more
helpful even if it makes for longer answers.

2. My experience and my failures are still my own, and yours may differ. I hope you learn 
something from my experience, but I can’t guarantee that it works in all cases.

3. It’s impossible to reduce a problem solving journey to absolute first principles. Every 
problem we successfully solve relies on some amount of prior knowledge, experience and 
preparation. I’ll try to highlight those explicitly whenever I can, but please be aware that
you do need to be prepared. If I solve a problem using complex analysis and you happen to 
not know anything about complex analysis, it’s unlikely that you’ll learn a whole lot from 
reading my answer.
```

<a name="#product-management-of-math"></a>
### Product management of math
([overview](#overview))

I've never seen this perspective articulated before or since, which makes it all the more valuable. This is from Alon Amit's [The Product Management of Mathematics](https://affinemess.quora.com/The-Product-Management-of-Mathematics). 

Exposition:

```markdown
Ask someone “what is a real number?”, and you will likely get something involving Cauchy
sequences, or Dedekind cuts, or decimal expansions.

Ask them “what is a complex number?”, and you may be informed about pairs of real numbers
with an i thrown in.

Ask them “what’s the difference between Riemann and Lebesgue integration?”, and in all 
likelihood you’ll get a dollop of Riemann sums, vertical vs horizontal partitioning, and
some measure theory.

All of these answers are correct. All of them, and many like them, are wrong. Not *wrong* as
in *incorrect*, but wrong as in this is *not the right answer*. It’s likely unhelpful, or at 
least not the most helpful it could be.

Why?

Ask someone “what is the difference between Facebook and Twitter?” Imagine they start telling
you about Scala, PHP, Thrift, Hadoop, Memcached and the like. If they know what they’re
talking about, they may provide you with a very accurate picture of the differences between
the tech stacks and software architectures of the two services. Their answer may be fully 
correct.

But this isn’t what you wanted to know, is it? The answer is correct, but useless.

What you want to know is what is the difference between the *products*. What people who *use* 
them experience differently. You want to know about friending vs following, sharing vs
broadcasting, personal social circles vs celebrity fan bases, and so on. You don’t care about
specific features, and you certainly don’t care about the underlying technology. You care 
about the experience, what it feels like, what you can do and how you are likely to use them.

You see, the math examples I gave are like answering the FB/Twitter question with the tech 
stack. It’s telling you about the inner workings, the construction, the engineering of those 
mathematical concepts instead of telling you what they *do*, which is what a Math Product Manager
would tell you.

A Math Product Manager would explain the difference between Riemann and Lebesgue integration
without ever mentioning Riemann sums and partitioning the range instead of partitioning the 
domain. Those things belong to the Math Engineers. The Riemann Integral and Lebesgue Integral 
are *products*. They have some commonalities (like Facebook and Twitter) and certain profound, 
crucial differences, and it is those differences you should care about, and those are 
differences in what they *do*, not how they are *built*.

Both integrals are machines, black boxes, devices that crunch functions and produce numbers. 
They are both linear, monotonic and have other nice features. The Lebesgue integral, however,
can handle many functions which make the Riemann integral crash. The Lebesgue integral, in fact,
has a much better-written spec: it’s possible, with reasonable effort, to describe just what it
can and cannot do. The Riemann integral is a classical “engineering-driven” product: it was 
built, rather than defined. It works great when it works, but describing exactly what it’s *good*
for is next to impossible.

This is the difference between engineering-oriented and product-oriented *exposition* of mathematical
ideas. It’s a difference in how we choose to teach, to explain, to clarify. 
```

Research:

```markdown
But the difference between Math PMs and Math Engineers goes well beyond math education. It exists 
right at the very endeavor of doing mathematics.

Product Managers *define* products. Engineers *build* them. Math research can sometimes be seen in 
an analogous way.

When faced with a challenge, many mathematicians start building scaffolding and structures with 
ingredients they have, piecing them together and hoping to achieve what they set to achieve. But
other times, they try to step back and define what it is they hope to build.

This can take the form of a *program*: a plan for a mathematical reality we don’t yet understand. We
don’t even know if it’s possible, but the far-sighted among us can envision. Robert Langlands,
famously, created such a program.

Other times, this literally takes the form of a “product spec”. Following the success of proving 
the Weil Conjectures for curves over finite fields, André Weil created an ambitious program for
expanding them into a profound, far-reaching edifice, but he also suggested how this could be done:
by creating a cohomology theory for contexts where there was no apparent way to have one. Weil 
wrote a spec for this cohomology theory, but he didn’t know how to build it. It took decades to 
build, but this is just how étale cohomology came to be: it was an engineering response to a 
product spec. Grothendieck, Deligne and others knew what requirements they needed to satisfy. They
set out to satisfy them. Grothendieck himself created far, far-reaching definitions for mathematical
universes we are still trying to put together.

At a much smaller scale, math research and even math problem solving are sometimes like that. A 
mathematician may say to themselves, if only I had a non-abelian analogue of this… this is a rough
spec. A problem solver may think, wow, if only I could have an energy function with *these* 
properties… hmmm… It’s a top-down instead of a bottom-up approach: instead of using the given data,
you are portraying what you need, the end result, and then you try to build it, sometimes literally
working backwards from the specification.

To be clear, this isn’t a competition or a war between camps. Product Managers and Engineers work 
together, not against each other. Successful companies and products emerge when they work together
well. There are usually more engineers than PMs, and it’s the same in math. In software development,
it is more common to have the discipline to define what you’re after before you start building it. 
Many mathematicians work without a product spec, and that’s fine and reasonable because often they 
don’t know what they will find. It’s research, not product development.

But there are at least two contexts in which the PM perspective is important: when mathematical 
leaders like Langlands, Grothendieck and Weil define a vision for what’s needed; and when we *teach*. 
Because when we teach it’s crucial to explain not just *how* something is built but also *why*. Why 
did we introduce quaternions? Why did we introduce cohomology theory? Why did we introduce measures,
matroids or matrices? What can you *do* with those things? How do you *use* them?

That’s true even if, historically, some of those things were stumbled upon rather than designed, 
constructed haphazardly rather than under the watchful eye of a product designer. The number e was
originally defined as the limit of certain compound interest calculations; this is almost irrelevant
nowadays. That’s not why it’s so important. When we teach it today, we can clarify its utility and
importance as a *product*.

I’ve often quoted Tim Gowers’ tenet that mathematical objects *are* what they *do*. I think this is 
a facet of the same idea: thinking in product terms, rather than engineering terms, can often be 
helpful in understanding math, in teaching math, and in guiding mathematical research. You don’t 
have to be math PM, but it’s good to know that they exist. And I take comfort in knowing that 
sometimes I play a PM role when I teach math, in rough analogy to my own day job.

It’s a good feeling.
```

<a name="#Thinking-and-explaining"></a>
### Thinking and explaining
([overview](#overview))

I always return to the late Bill Thurston's great MO question [Thinking and explaining](https://mathoverflow.net/questions/38639/thinking-and-explaining) every few months or years for the wealth of insightful quotes within. Here I place them within the wider context of my walled garden of ideas/document.

Bill's question:

```markdown
How big a gap is there between how you think about mathematics and what you say to others?
Do you say what you're thinking? Please give either personal examples of how your thoughts
and words differ, or describe how they are connected for you.


I've been fascinated by the phenomenon the question addresses for a long time. We have 
complex minds evolved over many millions of years, with many modules always at work. A 
lot we don't habitually verbalize, and some of it is very challenging to verbalize or to
communicate in any medium. Whether for this or other reasons, I'm under the impression 
that mathematicians often have unspoken thought processes guiding their work which may 
be difficult to explain, or they feel too inhibited to try. One prototypical situation 
is this: there's a mathematical object that's obviously (to you) invariant under a 
certain transformation. For instant, a linear map might conserve volume for an 'obvious'
reason. But you don't have good language to explain your reason---so instead of 
explaining, or perhaps after trying to explain and failing, you fall back on computation. 
You turn the crank and without undue effort, demonstrate that the object is indeed
invariant.

Here's a specific example. Once I mentioned this phenomenon to Andy Gleason; he immediately
responded that when he taught algebra courses, if he was discussing cyclic subgroups of a
group, he had a mental image of group elements breaking into a formation organized into 
circular groups. He said that 'we' never would say anything like that to the students. His
words made a vivid picture in my head, because it fit with how I thought about groups. I 
was reminded of my long struggle as a student, trying to attach meaning to 'group', rather
than just a collection of symbols, words, definitions, theorems and proofs that I read in 
a textbook.
```

The following are MO's responses I liked. 

Here's one by Bill that comes to mind every once in a while:

```markdown
When listening to a lecture, I can't possibly attend to every word: so many words blank 
out my thoughts. My attention repeatedly dives inward to my own thoughts and my own mental
models, asking 'what are they really saying?' or 'where is this going?'. I try to shortcut
through my own understanding, then emerge to see if I'm still with the lecture.
```

And here's another, also by Bill:

```markdown
I've learned that when I go back to look at something, my thinking has usually rounded off
too many corners, so my understanding is much fuzzier. I sometimes find things I have 
written to be very obtuse. I was too wrapped up in my then state of mind to express ideas 
clearly even to myself, reading it much later.

What's important is not the process by which you arrived at an idea, but a story that gives
the idea context and meaning. It's a story you make: a setting of meaning and reason for the 
idea, rather than the history of how you stumbled on the idea.
```

Terry Tao is -- well, he's as close as you'll get to a universal problem-solver this generation:

```markdown
I find there is a world of difference between explaining things to a colleague, and explaining
things to a close collaborator. With the latter, one really can communicate at the intuitive
level, because one already has a reasonable idea of what the other person's mental model of the
problem is. In some ways, I find that throwing out things to a collaborator is closer to the 
mathematical thought process than just thinking about maths on one's own, if that makes any 
sense.

One specific mental image that I can communicate easily with collaborators, but not always to 
more general audiences, is to think of quantifiers in game theoretic terms. Do we need to show
that for every epsilon there exists a delta? Then imagine that you have a bag of deltas in your
hand, but you can wait until your opponent (or some malicious force of nature) produces an 
epsilon to bother you, at which point you can reach into your bag and find the right delta to 
deal with the problem. Somehow, anthropomorphising the "enemy" (as well as one's "allies") can 
focus one's thoughts quite well. This intuition also combines well with probabilistic methods, 
in which case in addition to you and the adversary, there is also a Random player who spits out
mathematical quantities in a way that is neither maximally helpful nor maximally adverse to your 
cause, but just some randomly chosen quantity in between. The trick is then to harness this
randomness to let you evade and confuse your adversary.

Is there a quantity in one's PDE or dynamical system that one can bound, but not otherwise 
estimate very well? Then imagine that it is controlled by an adversary or by Murphy's law, and 
will always push things in the most unfavorable direction for whatever you are trying to
accomplish. Sometimes this will make that term "win" the game, in which case one either gives up
(or starts hunting for negative results), or looks for additional ways to "tame" or "constrain" 
that troublesome term, for instance by exploiting some conservation law structure of the PDE.

For evolutionary PDEs in particular, I find there is a rich zoo of colourful physical analogies
that one can use to get a grip on a problem. I've used the metaphor of an egg yolk frying in a
pool of oil, or a jetski riding ocean waves, to understand the behaviour of a fine-scaled or 
high-frequency component of a wave when under the influence of a lower frequency field, and how
it exchanges mass, energy, or momentum with its environment. In one extreme case, I ended up 
rolling around on the floor with my eyes closed in order to understand the effect of a gauge 
transformation that was based on this type of interaction between different frequencies. 
(Incidentally, that particular gauge transformation won me a Bocher prize, once I understood how 
it worked.) I guess this last example is one that I would have difficulty communicating to even 
my closest collaborators. Needless to say, none of these analogies show up in my published papers,
although I did try to convey some of them in my PDE book eventually.

ADDED LATER: I think one reason why one cannot communicate most of one's internal mathematical
thoughts is that one's internal mathematical model is very much a function of one's mathematical
upbringing. For instance, my background is in harmonic analysis, and so I try to visualise as
much as possible in terms of things like interactions between frequencies, or contests between 
different quantitative bounds. This is probably quite a different perspective from someone 
brought up from, say, an algebraic, geometric, or logical background. I can appreciate these other
perspectives, but still tend to revert to the ones I am most personally comfortable with when I am
thinking about these things on my own.

ADDED (MUCH) LATER: Another mode of thought that I and many others use routinely, but which I 
realised only recently was not as ubiquitious as I believed, is to use an "economic" mindset to 
prove inequalities such as X≤Y or X≤CY for various positive quantities X,Y, interpreting them in the
form "If I can afford Y, can I therefore afford X?" or "If I can afford lots of Y, can I therefore
afford X?" respectively. This frame of reference starts one thinking about what types of quantities
are "cheap" and what are "expensive", and whether the use of various standard inequalities 
constitutes a "good deal" or not. It also helps one understand the role of weights, which make things
more expensive when the weight is large, and cheaper when the weight is small.

ADDED (MUCH, MUCH) LATER: One visualisation technique that I have found very helpful is to
incorporate the ambient symmetries of the problem (a la Klein) as little "wobbles" to the objects 
being visualised. This is most familiarly done in topology ("rubber sheet mathematics"), where every
object considered is a bit "rubbery" and thus deforming all the time by infinitesimal homeomorphisms.
But geometric objects in a scale-invariant problem could be thought of as being viewed through a 
camera with a slightly wobbly zoom lens, so that one's mental image of these objects is always 
varying a little in size. Similarly, if one is in a translation-invariant setting, one's mental
camera should be sliding back and forth just a little to remind you of this, if one is working in a 
Euclidean space then the camera might be jiggling through all the rigid motions, and so forth. A more
advanced example: if the problem is invariant under tensor products, as per the tensor product trick,
then one's low dimensional objects should have a tiny bit of shadowing (or perhaps look like one of 
these 3D images when one doesn't have the polarised glasses, with the slightly separated red and blue
components) that suggest that they are projections of a higher dimensional Cartesian product.

One reason why one wants to do this is that it helps suggest useful normalisations. If one is
viewing a situation with a wobbly zoom lens and there is some length that appears all over one's
analysis, one is reminded that one can spend the scale invariance of the problem to zoom up or 
down as appropriate to normalise this scale to equal 1. Similarly for other ambient symmetries.

This sort of wobbling of symmetries is also available in less geometric settings. When viewing,
say, a graph on n vertices, perhaps the labels 1,…,n on the vertices have a tendency to swap with 
each other every so often, to emphasise the symmetry of relabeling in graph theory. Similarly, 
when dealing with a set {a,b,c,d,…}, perhaps the positions of the elements a,b,c,d in one's
enumeration of the set are volatile and swap places every so often. In analysis, one often only 
cares about the order of magnitude of some very large or very small quantity X, rather than its 
exact value; so one should view this quantity as being a bit squishy in size, growing or shrinking
by a factor of two or so every time one looks at the problem. If there is some probability theory
in one's problem, and some of your objects are random variables rather than deterministic 
variables, then you can imagine that every so often the "game resets", with the random variables
jumping around to different values in their range (and any quantities depending on these variables 
changing accordingly), whereas the deterministic variables stay fixed. Similarly if one has generic
points in a variety, or nonstandard objects in a space (with the point being that if something bad
happens if, say, your generic point is trapped in a subvariety, you can "reset the game" in which 
the generic point is now outside the subvariety; similarly one can "reset" an unbounded nonstandard 
number to be larger than any given standard number, etc.).
```

Tim Gowers notes that this also happens "at the very bottom" in simple arithmetic:

```markdown
This phenomenon occurs not just in advanced mathematics but also right at the very bottom in 
simple mental arithmetic. If I have to do a moderately complicated calculation such as adding 
two three-digit numbers, there's often a part of my brain that jumps ahead to the answer before
another more cautious part has got there with carefully checked calculations. The first part 
just sort of feels the answer and then says "I told you so" to the second part, except 
occasionally when the first part gets it wrong and the second part says "Now you know why I
bother to be careful" to the first part.

And there are also aspects of how I carry out integer addition and subtraction that I would 
normally be a bit embarrassed to verbalize, such as that if I subtract 48 from 135 then there's 
a preliminary answer, 97, that I know from experience is wrong and has to be corrected by
subtracting 10. (The justification for the preliminary answer is that 13-4=9 and that the answer
must end in a 7.) It's not quite what's going on in my head, but it's almost as though I say, 
"OK I'll subtract 58 instead so as to get the right answer." But if I were teaching this to a 
child then I'd tell a slightly different story, such as borrowing 1, or first subtracting 50 and 
then adding 2.
```

Bill agrees:

```markdown
I agree, beginning math is a very rich and intriguing area. I've discussed arithmetic questions
with many young children, and they are often very creative in strategies to think their way to
an answer. It really requires being on your toes to discern their thought processes, because the
words do not match adult expectations; they often take phrases with logical meanings that I've
suppressed because of convention. To teach math to kids, I think it's paramount to encourage 
them to think, rather than teach conventional "borrowing 1" type stories. Early math teaching 
usually *suppresses* thinking.
```

I also like Deane Yang's response to Gowers above:

```markdown
Actually, I like explaining ways of solving problems that involve making mistakes, intentional 
or not, and then figuring out how to correct them. I like this better than trying to teach
error-free algorithms, because it incorporates the error-checking as a natural part of the process.
I believe we should be teaching more systematic methods for finding and correcting errors. 
Students should learn when guessing, checking, and correcting is faster and easier than a more 
direct algorithm. Integrals that require more than one integration by parts is an obvious example
of this.
```

Alon Amit takes what Deane says above and makes it the guiding ethos of his expository math writing on Quora (see [Solving math problems terribly](#Solving-math-problems-terribly)).

And then there's Vivek Shende's "subconscious mastication", which is analogous to Ramanujan, just slower:

```markdown
I have a worse problem than having unspoken thought processes: some of my best thought processes
are simply beneath the level of consciousness and I don't notice them at all until they're finished.
Even then, I often get only an answer and not an explanation out of them. Surely this happens to 
everyone: the problem solved during sleep, the idea on a walk in the woods, the conviction that a 
conjecture is true on utterly minimal evidence, the argument that pops up full formed in the middle
of a conversation.

My mathematical process is roughly this: consciously, I try a lot of stupid things which essentially
have no chance of working but do have the benefit of exposing me to lots of examples; these examples
pile up and are subconsciously masticated for days, weeks, months -- I'm not old enough 
mathematically to put "years" here yet -- and eventually by some inner and unobservable process I 
just have a feeling about what to do.

Perhaps that's an exaggeration. But I certainly do feel that way sometimes, and to the extent that 
it's true, it means that the whole project of trying to communicate how I thought of something is 
just telling stories, at least if I say anything other than "well, I just knew one day."
```

Cam MacLeman:

```markdown
One of my favorites from undergrad was describing a linear transformation as a commander-
in-chief, who told the generals (a basis) where to go, who in turn tells all the soldiers
(the rest of the vectors) where to go. The chain of command in action in a linear algebra
class.
```

<a name="#math-advice"></a>
## Math advice
([overview](#overview))

<a name="#reading-the-masters-in-math"></a>
### Reading the masters in math
([overview](#overview))

(See also [Reading the masters in philosophy](#reading-the-masters-in-philosophy), or my old post [If Aristotle were a pro skater: or, reading the masters in math and philosophy*](https://mosstuff.quora.com/If-Aristotle-were-a-pro-skater-or-reading-the-masters-in-math-and-philosophy) to see both math and philo in one place.) 

Should you read the masters? In other words, should you prefer primary sources to summaries and commentaries?

On the one hand, the masters are the masters, so surely there’s something to reading them. On the other hand, I’m the kind of person who easily gets lost in walls of text, so when it comes to writing on difficult / ‘slippery’ topics I prefer polished, non-digressive reads. And primary texts, so they seem, are nothing but digressive.

(I suppose it depends why you’re reading. If it’s for enjoyment then secondhand sources certainly won’t cut it. I’m usually looking for insight; enjoyment I relegate to fiction, or exceptionally-written exposition, or something.)

It doesn’t help that Andrew L’s comment in [this MO thread](https://mathoverflow.net/questions/28268/do-you-read-the-masters) is essentially what I think of the masters (to wit, that they’re notoriously hard to read):

```markdown
There's a myth surrounding Abel's dictum that stems from the unreadability of the masters
like Gauss as a measure of their nearly inhuman brilliance. This is a fallacy.

The reason the masters are so difficult to read is because we are catching them with their
pants down in the act of creation: they are groping towards the right notation and
terminology, but aren't quite there yet.

For example, it's pretty clear Riemann in his doctoral lecture was trying to explain the 
need for higher dimensional spaces that went beyond familiar three dimensional space 
("multiply extended quantities") which preserved all the familiar properties of the usual
Euclidean spaces, i.e. Kleinian transformations and calculus in local neighborhoods. The
problem was without either linear algebra or the fundamentals of topology, it was next to 
impossible to express this idea clearly and precisely. He just ends up babbling on about
what's needed. But all the same, Riemann recognized what was needed, even if how to
express it correctly was beyond his ability.
```

There must be *something* to reading the masters, or at least primary sources. What could it be?

Often you can judge how ‘mature’ a field is by seeing how much shorter proofs of old results become when appropriate machinery gets developed and subsumes them as special cases within the larger theoretical framework. (Think Grothendieck, but less extreme.) This is usually good. But then there are cases to the contrary, like Fedja’s experience, recounted in the MO thread [Papers better than books?](https://mathoverflow.net/questions/140954/papers-better-than-books?lq=1&noredirect=1):

```markdown
Very recently I and Misha Sodin had a strong incentive to learn the Ito-Nisio lemma… The 
textbooks we could find fell into 2 categories: those that didn't present the proof at 
all and those presenting it on page 2xx as a combination of theorems 3.x.x, 4.x.x, 5.x.x,
etc.

The original paper is less than 10 pages long, essentially self-contained, and very easy
to read and understand.

The moral is the same as Boris put forth: the books are there to optimize the time you 
need to spend to learn the whole theory. However, for every particular implication A->B 
the approach they usually take is something like E->F->G, G->F, (F and Q)->B; since A->E,
then A->G; once we know G, we have F, so it suffices to prove that A->Q to show that A->B;
we show that Q,R,S,T,U are equivalent, with the trivial implication S->Q left to the 
reader as an exercise; finally, we prove that A->S.

So if all you need is A->B, you may be much better off reading the paper whose only purpose
is to prove exactly that.
```

Andrew L again, same thread as the first:

```markdown
One of my favorite books is Hassler Whitney's Geometric Integration Theory. I have friends 
in differential geometry who tell me it's a dinosaur, that his proof of the de Rham theorem 
is incredibly coarse and tedious. Yes, it is — but it has the advantage of being a DIRECT
proof from the construction of simplexes on the boundary of an embedded manifold. I love the
book because although Whitney's ideas were old fashioned, they were incredibly powerful IDEAS
that allow us to tackle the subject concretely and with an amazing amount of insight. THAT'S
what we get from reading the masters — their insight and depth of understanding that allows 
us to see beyond the machinery into why things are defined as they are.
```

Igor Pak makes a cameo:

```markdown
There is more than one reason to read "masters". One such reason is field-specific and can be 
phrased as "read the latest work right before a scientific revolution" (standard example is 
the large body of work by Cayley, Sylvester, Gordan, etc., in the pre-Hilbert classical 
invariant theory). Often such results are more powerful in very specific cases of interest.

Another practical reason to read "masters" is to avoid embarrassment. Lots of (mostly minor) 
results are not mentioned in later treatises, so a number of people rediscover these results 
because they are either too lazy to read, or simply assume that "masters" couldn't have possibly
be so smart to figure out these results back then... When going through the references in
writing this survey, I read all 80 pages of J.J. Sylvester, A constructive theory of partitions,
arranged in three acts, an interact and an exodion, Amer. J. Math. 5 (1882), 251–330. As a 
result, I discovered that a number of recent results were already proved there, sometimes by 
leaders in the field (let me not name them here - see the survey).
```

And then there is Roy Smith’s rich, long answer from the same thread; I’ll only quote a few scattered paragraphs:

```markdown
These are elementary examples hence from a fairly naive and uneducated person, myself, who 
has not at all plumbed the depth of many original papers. But these few forays have definitely 
convinced me there is a benefit that cannot be gained elsewhere, as these exposures can
transform the understanding of ordinary mortals closer to that of more knowledgeable persons, 
at least in a narrow vein. So while it might be thought that only the strongest mathematicians
can attempt these papers, my advice would be that reading such masters may be even more helpful
to us average students.

Once as grad student in Auslander's algebraic geometry class, I vowed to try out Abel's advice
and read the master Zariski's paper on the concept of a simple point. I was very discouraged 
when several hours passed and I had managed only a few pages. Upon returning to class, Auslander
began to pepper us with questions about regular local rings. I found out how much I had learned
when I answered them all easily until he literally told me to be quiet, since I obviously knew 
the subject cold. (To be honest, I did not know the very next question he posed, but I was off 
the hook.) …

The sense of wonder and awe one gets upon reading people like Riemann or Euler, is also quite
wonderful. Any student who has struggled to compute the sum of the even powers of the reciprocals
of natural numbers 1/n^2k, will be amazed at Euler's facile accomplishment of this for many
values of k. Calculus students estimating π by the usual series to 3 or 4 places will also be 
impressed at his scores of correct digits. …

A remark on the definition of master, versus creator. There are cases where a later master 
reexamines an earlier work and adds to it, and in these cases it seems valuable to read both 
versions. In addition to examples given above of Newton generalizing Euclid and Mumford using
Hilbert, perhaps Mumford's demonstration of the power of Grothendieck's Riemann Roch theorem in 
calculating inavriants of moduli space of curves is relevant.
```

I’ve been conflating ‘masters’ and ‘primary sources’. Usually they’re the same, because the really enduring texts are written by the masters, but sometimes the masters write expository texts too, and it’s still marginally beneficial to read them, per Ilya Grigoriev’s comment in the MO thread [Why do so many textbooks have so much technical detail and so little enlightenment?](https://mathoverflow.net/questions/13089/why-do-so-many-textbooks-have-so-much-technical-detail-and-so-little-enlightenme?rq=1):

```markdown
Providing real enlightenment well is very, very hard, and requires a very intimate relationship with a subject.

Even for well-established subjects, like undergraduate mathematics, where there are a million
mathematicians who know the subject very well, I find that all the really good books are written
by the true titans of the field -- like Milnor, Serre, Kolmogorov, etc. They understand the 
underlying structure and logical order of the subject so well that it can be presented in a way
that it basically motivates itself -- basically, they can explain math the way they discovered 
it, and it's beautiful. Every next theorem you read is obviously important, and if it isn't then
the proof motivates it. …It's interesting how all the best books I know don't have explicit 
paragraphs providing the motivation - they don't need them.
```

<a name="#go-to-seminars"></a>
### Go to seminars
([overview](#overview))

Ravi Vakil's [advice page](http://math.stanford.edu/~vakil/potentialstudents.html) for potential PhD students has loads of advice related to going to seminars:

```markdown
Older graduate students will verify that there is a high correlation between those students who 
are doing the broadest and deepest work and those who are regularly attending seminars. Many
people erroneously conclude that those who are the strongest students therefore go to seminars, 
while in fact the causation goes very much in the opposite direction.

Go to research seminars earlier than you think you should. Do not just go to seminars that you 
think are directly related to what you do (or more precisely, what you currently think you 
currently do). You should certainly go to every single seminar related to algebraic geometry that
you can, and likely drop by other seminars occasionally too. Learning to get information out of
research seminars is an acquired skill, usually acquired much later than the skill of reading 
mathematics. You may think it isn't helpful to go to a seminar where you understand just 5% of
what the speaker says, and may want to wait until you are closer to 100%; but no one is anywhere
near 100% (even the speaker!), so you should go anyway.

Try to follow the thread of the talk, and when you get thrown, try to get back on again. (This
isn't always possible, and admittedly often the fault lies with the speaker.)

At the end of the talk, you should try to answer the questions: What question(s) is the speaker
trying to answer? Why should we care about them? What flavor of results has the speaker proved?
Do I have a small example of the phenonenon under discussion? You can even scribble down these 
questions at the start of the talk, and jot down answers to them during the talk.

Try to extract three words from the talk (no matter how tangentially related to the subject at 
hand) that you want to know the definition of. Then after the talk, ask me what they mean. (In 
general, feel free to touch base with me after every seminar. I might tell you something 
interesting related to the talk.)

See if you can get one lesson from the talk (broadly interpreted). If you manage to get one lesson
from each talk you go to, you'll learn a huge amount over time, although you'll only realize this 
after quite a while. (If you are unable to learn even one thing about mathematics from a talk,
think about what the speaker could have done differently so that you could have learned something.
You can learn a lot about giving good talks by thinking about what makes bad talks bad.)

Try to ask one question at as many seminars as possible, either during the talk, or privately
afterwards. The act of trying to formulating an interesting question (for you, not the speaker!)
is a worthwhile exercise, and can focus the mind.

Your thesis problem may well come out of an idea you have while sitting in a seminar.

Go to seminar dinners when at all possible, even though it is scary, and no one else is going.

Go to colloquia fairly often, so you have a reasonable idea of what is happening in other parts 
of mathematics. It is amazing what can become relevant to your research. You won't believe it 
until it happens to you. And it won't happen to you unless you go to colloquia. Ditto for seminars
in other fields.
```

Vakil expands upon one of the points above in this page: [The "Three Things" Exercise for getting things out of talks](http://math.stanford.edu/~vakil/threethings.html):

```markdown
*The challenge of talks*. It is tricky to get things out of talks, even after a lot of practice. 
It is very easy to go to a talk, and at some point have your eyes glaze over. Talks are like horses:
once you are thrown off, it is hard to get back on. Especially if the horse is stomping on your face.
(That's why it is very bad to come into a talk a few minutes late --- even if it is sometimes
necessary.)

"Three Things" is an exercise to learn how to get things out of talks. It can be useful if you are in
the first few years of going to seminars --- I've intended it as practice for graduate students --- 
but I've also found that I got much more out of talks (especially those out of my comfort zone) when
using it. It is admittedly a little contrived, and when a bunch of us first experimented with it 
(perhaps around 2007?), we stopped doing it after a while because we got tired of it.

*The theory is as follows*. If you can get even three small things out of a talk, it is a successful
talk. And if you can't get even three small things out of a talk, it was not a successful experience.
Note that the things you get out of a talk needn't be the things that your neighbor got out of a talk,
or the things the speaker expected you to get out of the talk.

*Here is how it works*. Take a clean sheet of paper, or an index card. Your goal is to have three things,
and only three things, on this sheet at the end of the talk. The "things" can be of many forms:

- a definition you want to remember (e.g. "a K3 surface is...")
- a theorem you want to remember ("the moduli space of polarized K3 surfaces is smooth")
- a motivating or key example ("a quartic is an example of a K3 surface")
- a motivating problem ("why are all moduli spaces of polarized K3 surfaces the same dimension?")
- a question you want to ask the speaker ("why is that hypothesis in your theorem?")
- a question you want to ask someone else (a definition, motivation, a question about a connection etc.)
- anything else of a similar flavor: something specific that made you think. Something vague ("I liked 
the part where she talked about groups") does not count as a "thing".

*As you watch the talk*, look out for "things" you like. When one comes your way, write it down. Then
later write down a second. Then write down a third. Hopefully a fourth will come your way --- and
then you must look over the previous three, and decide which one must be cut. A dirty secret is that
you may not be able to prevent yourself from remembering the one you cut --- and the ones you kept
and reviewed will be more fixed in your mind.

(If you take notes in a more traditional sense, you can still play the game, by putting a star beside
each "thing". This works a little less well; you will be less focused on looking for "things".)

*After the talk*: if other people are playing, send each other your things by email (or discuss them
in person). It is surprisingly enlightening. And there will likely be some follow-up discussion. It
doesn't take much time (to type or to send one sentence responses to others' things if the spirit 
moves you). If you have questions, then ask them to someone (perhaps the speaker over the semianr
dinner; or perhaps your advisor or your students or your colleagues). Don't let them drop.
```

See also his celebrated [backfilling tendrils of knowledge](#mathematical-maturity) quote.

<a name="#asking-the-right-question"></a>
### Asking the right question
([overview](#overview))

[Jay Daigle](https://jaydaigle.net/) is an assistant professor of math at Occidental College who received his PhD in number theory at Caltech under Matthias Flach. He’s also jadagul of [Maybe-Mathematical Musings](http://jadagul.tumblr.com/), one of the two really consistently high-quality math-content-producers/commentators I’ve had the pleasure of stumbling across on math Tumblr (the other being Rob Nostalgebraist, who also writes [genuinely great fiction](https://archiveofourown.org/users/nostalgebraist/pseuds/nostalgebraist) and is a [brilliant book reviewer](https://www.goodreads.com/author/show/13933106.nostalgebraist)). He’s sufficiently [differently free from me](https://www.ribbonfarm.com/2014/11/05/dont-surround-yourself-with-smarter-people/) in Venkat Rao’s sense, plus just flat-out smarter, that I always get a lot out of his writings in Alan Kay’s “point of view is worth 80 IQ points” sense, so I always enjoy reading his math #effortposts.

Recently I discovered that he’s collected these effortposts into a standalone blog, [Jay's Blog](https://jaydaigle.net/blog/paradigms-and-priors/), so I’ve had a lot of fun going over his essays. Here are some quotes from one of those essays, [Asking the Right Question](https://jaydaigle.net/blog/asking-the-right-question/), which I’m saving here for quick future reference. (You should Jay’s original essay instead of defaulting to my quotes below! He’s a really enjoyable read, I promise.)

First off: why is asking good questions so important? About four reasons, the last one being the main thrust of this section:

```markdown
First and most obviously, it’s easier to get help with things and learn things if you can ask better
questions. 

Second, and maybe more importantly, framing questions well is a lot of what makes you a good 
mathematician.

The most boring way to ask a bad question is just to not include enough information. Sometimes this
is just laziness (“I don’t understand how to do this problem, please help”). And I’ve definitely seen 
questions asked that are thin disguises over “I don’t want to do my homework; can someone do it for me?”

But more often, badly-phrased questions result from deep confusion on the part of the asker. If they 
understood the material well enough to ask their question clearly and correctly, they wouldn’t need to
ask it in the first place.
```

It's important to be able to figure out what question to ask in the first place:

```markdown
A lot of math is less about answering questions than about figuring out exactly what question you should
be asking, and how to make it precise. We tend to sweep this under the rug a bit when teaching, in a way 
that I suspect probably leads to a certain amount of confusion.

When we teach, we often ask a question, and then demonstrate a tool to answer it, without necessarily 
stopping to explain why that question is a good one, or how people settled on asking exactly that question.
And this often leaves our students with the sense that what they’re doing doesn’t really mean anything.

This is a major reason students fall back on figuring out what “type of problem” they’re working on, and
then following “the steps” to get the answer. They see math as a sort of opaque box, and a question asks
them to perform the correct magical ritual to get the answer. Because if the words you’re using—and your
questions—don’t have a meaning, that’s all you can really do.

And that’s how you get questions like “how do I find solutions to f(x) = sin(x)+1/2.” I can tell what the
original question probably was. But because the student doesn’t really understand what a “function” is, 
they ask a question that is, read literally, completely nonsensical.
```

An example of a badly-written but actually great question:

```markdown
Sometimes, you see a question that’s basically “this one thing feels kind of like this other thing, but 
I can’t tell you how. Can you tell me?”

These people are doing good math. They’re noticing a pattern, and trying to put it into words. They’re 
maybe not quite there, and sometimes it’s hard to answer the question clearly. But it shows great
instincts.

And this is how math tends to actually get done! When we teach, we tend to define terms, then state 
theorems about them, and then prove the theorems. But this is exactly backwards from how math is often
actually done. First we understand what’s going on; then we figure out what the rule is and write it 
down; and finally understand what conditions are important and give those conditions names. That is, 
we formulate a proof, then state the theorem, and then define the terms.

These questions are working on step 1. I want to encourage them.
```

<a name="#why-math-is-boring"></a>
### Why math is boring
([overview](#overview))

From John Baez's "very rough draft" [Why Mathematics is Boring](http://math.ucr.edu/home/baez/boring.pdf), where he argues in the abstract that the boring style of math publications is a serious matter to contend with:

```markdown
Storytellers have many strategies for luring in their audience and keeping them interested.
These include standardized narrative structures, vivid characters, breaking down long stories
into episodes, and subtle methods of reminding the readers of facts they may have forgotten. The
typical style of writing mathematics systematically avoids these strategies, since the explicit goal
is “proving a fact” rather than “telling a story”. Readers are left to provide their own narrative
framework, which they do privately, in conversations, or in colloquium talks. As a result, even
expert mathematicians find papers — especially those outside their own field — boring and
difficult to understand. This impedes the development of mathematics.
```

Introduction:

```markdown
In their research papers, mathematicians usually eschew narrative techniques designed to keep readers
interested, since their main goal is not to “entertain” or even explain, but present logical arguments
as efficiently as possible. While this makes a certain sense, it neglects the human dimension
of mathematics. It neglects the fact that a piece of mathematics is almost useless if almost nobody
understands it. But, before anyone can understand a piece of mathematics, they must first become
interested in it. So, for a mathematician who wants to fully develop a piece of mathematics, discovery
and proof are only the first steps on a longer road. The next step is getting people interested.

Unfortunately, mathematicians are not trained in this art. Indeed, their writing is famous for
being “dry”. There are exceptions, and these exceptions are worth studying. But it also makes sense
to look to people whose whole business is getting people interested: story-tellers.
Everyone enjoys a good story. We have been telling and listening to stories for untold millennia.
Stories are one of our basic ways of understanding the world. I believe that when we read a piece of
mathematics, part of us is reading it as a highly refined and sublimated sort of story, with characters
and a plot, conflict and resolution.

If this is true, maybe we should consider some tips for short story writers, and see how they can
be applied — in transmuted form — to the writing of mathematics. These tips may sound a bit
crass to mathematicians, or even readers of “serious” fiction. But they go straight to the heart of
what gets people interested, and what keeps them interested, in a piece of writing.
```

Under "write a catchy first paragraph":

```markdown
We are constantly encountering texts; we don’t bother reading all the way through most of them.
Once texts were rare and precious. Now, in the era of the world-wide web, there is always too much
to read. We must efficiently cull out most of the material vying for our attention. Often we base
our decision on the first sentence or two.

Since most writers of short stories succeed largely on their sheer number of readers, and few
people read stories because they need to, writers of short stories learn the importance of quickly
grabbing the reader’s attention. In a catchy story, each sentence makes the reader want to read the
next. The first few sentences bear the brunt of this responsibility.

Mathematicians operate in a more forgiving environment, with guaranteed permanent employment for many. 
They can succeed with only few people reading their work. Consider two of the 
most famous mathematicians of recent years: Andrew Wiles and Grigori Perelman. How many of us
   have really read Wiles’ proof of Fermat’s last theorem, or Perelman’s sketched proof of the Poincar´e
conjecture? Even among professional mathematicians, most are satisfied to know that a few experts
vouch for these proofs’ validity. So, instead of broadening their readership, mathematicians are
mostly concerned with impressing other experts in their field.
```

See also [why academic writing sucks](#why-academic-writing-sucks). 

So how might we do better? 

From Terry Tao's [Write in your own voice](https://terrytao.wordpress.com/advice-on-writing-papers/write-in-your-own-voice/):

```markdown
When one is not simply quoting the prior text for historical or archival purposes, it is best to 
paraphrase and interpret the previous text rather than to copy that text verbatim.  This is for a 
number of reasons:

- One wants to avoid conveying any impression to readers, referees, or editors of plagiarism, padding,
or intellectual laziness in one’s papers.  (Note that the latter is a danger even if one is copying 
from one’s own work, rather than that of others.)

- The prior work may be dated in view of more recent developments and insights, as mentioned above.

- If you are copying or adapted a piece of text from another author that you do not fully understand
yourself, then it may end up being inappropriate or incongruous for your intended purpose, and may 
convey the impression of superficiality or being ill-informed.  If the text becomes inaccurate due 
to this adaptation, then this can also cause some embarrassment and annoyance for the original author
of that text.

- Excessive use of quotation from famous mathematicians to make one’s own work look more impressive is
the mathematical equivalent of name-dropping, and should be avoided.  Appeal to authority should not be
the primary basis for motivating a paper; a handful of citations to demonstrate the depth of interest 
in the problem being studied is usually sufficient.

- But most importantly of all, for one’s further mathematical development and career, one needs to
develop one’s own consistent mathematical “voice” and style, and to avoid the impression of simply 
imitating the voices of other authors.  There is no need in this subject for the mathematical equivalent
of a parrot, and a text which is a mix of the author’s voice and the voice of others can read very 
strangely.
```

Terry advises strongly *against* imitating an author's style:

```markdown
In some cases, the imitation of a previous author’s style and text is intended as a sign of respect or 
flattery for that author.  This is misguided; an author will in fact often find such mimicry to actually 
be somewhat offensive.  If one wants to truly respect a mathematician, then understand that
mathematician’s methods, results, and exposition, and improve, update, adapt, and advance all three.  
Even the greatest mathematician’s contributions should advance with the field, rather than being 
worshipped and preserved in some supposed state of perfection; the latter is mostly suitable only for 
historical purposes.
```

Contrast [Scott Alexander's comment on Luke's *Rhetoric* post](#nonfiction) (it's a long section, so I'll quote only the relevant bit):

```markdown
Your role models here should be those vampires who hunt down the talented, suck out their souls, and absorb
their powers. Which writers' souls you feast upon depends on your own natural style and your goals. I've
gained most from reading Eliezer, Mencius Moldbug, Aleister Crowley, and G.K. Chesterton; I'm currently making
my way through Chesterton's collected works pretty much with the sole aim of imprinting his writing style into 
my brain.

Stepping from the sublime to the ridiculous, I took a lot from reading Dave Barry when I was a child. He 
has a very observational sense of humor, the sort where instead of going out looking for jokes, he just
writes about a topic and it ends up funny. It's not hard to copy if you're familiar enough with it. And
if you can be funny, people will read you whether you have any other redeeming qualities or not.

Getting imprinted with good writers like this will serve you for your entire life. It will serve you 
whether you're on your fiftieth draft of a thesis paper, or you're rushing a Less Wrong comment in
the three minutes before you have to go to work. It will even serve you in regular old non-written
conversation, because wit and clarity are independent of medium.
```

More general advice by Terry on writing papers (all go to links for further reading):

```markdown
- Use the introduction to “sell” the key points of your paper; the results should be described accurately.
One should also invest some effort in both organising and motivating the paper, and in particular in 
selecting good notation and giving appropriate amounts of detail. But one should not over-optimise the paper.
It also assists readability if you factor the paper into smaller pieces, for instance by making plenty 
of lemmas.

- To reduce the time needed to write and organise a paper, I recommend writing a rapid prototype first.

- For first time authors especially, it is important to try to write professionally, and in one’s own voice.
One should take advantage of the English language, and not just rely purely on mathematical symbols.

- The ratio between results and effort in one’s paper should be at a local maximum.
```

More on [creating lemmas](https://terrytao.wordpress.com/advice-on-writing-papers/create-lemmas/) to factor the paper into smaller pieces to aid readability -- this is similar to [information hiding](http://en.wikipedia.org/wiki/Information_hiding) in software engineering, or [structured programming](http://en.wikipedia.org/wiki/Structured_programming) and [modularity](http://en.wikipedia.org/wiki/Modularity_%28programming%29):

```markdown
A typical argument in modern mathematics is often quite intricate, requiring many different steps, 
ingredients, and notation. The authors of the argument, having been intimately involved in all aspects 
of its construction, often do not realise just how complicated such an argument appears to a reader who 
is encountering it for the first time (I myself have been guilty of this oversight).

Part of the reason for this is that there is plenty of implicit structure in a paper which is crucial 
to understanding it properly, and which is known to the authors, but is not readily apparent to the
readers. Suppose for instance that part of a paper goes like this:

…
In Section 2, facts A, B, and C are derived, and then used to deduce D.
In Section 3, D is used to derive E.
In Section 4, D, and another fact F, are used to derive G.
In Section 5, E, G, and another fact H, are used to derive I.
…

A reader who is going through this paper one section at a time will try to keep A, B, C, and D all in
mind after finishing Section 2, and moving on to later sections.  However, facts A, B, and C are never
used again; they were instrumental to the argument because they allowed one to establish D, but once D 
is established, A, B, and C can be safely forgotten. Note, though that the reader does not know this. 
As a consequence, while reading Sections 3, 4, and 5, the reader has to set aside some of his or her 
mental resources to retain some facts which are of no further use, thus obscuring the structure of the
argument and making it more difficult to follow.

Now one could address this by placing some remarks at the end of Section 2 along the lines of “Facts A,
B, and C will not be used again in the rest of the paper”, or by devoting more thought to organising 
and motivating the paper. These are all worthwhile things to do, but a much more elegant solution is
simply to encapsulate D as a lemma, and to place A, B, C inside the proof of that lemma. 

This conveys several useful structural cues to the reader: firstly, that D is likely to be an important 
fact to use in later parts of the argument, and secondly, that A, B, and C are not needed elsewhere in 
the paper and can be safely forgotten. This additional structure will be useful to all readers, but will
be especially appreciated by those readers who are already expert in how to prove facts such as D, since
they can then glance at the statement of the lemma, readily convince themselves that the lemma is plausible
(possibly by using other tools than A, B, and C), and then quickly move on to the next part of the argument.
One can also add some remarks “for the experts” after the proof of a lemma, discussing possible alternate
proofs, refinements, special cases, connections to other lemmas in the literature, etc.

We have seen how “folding” the argument into lemmas can reduce the complexity of that argument by
“localising” certain facts in the argument. The same method can also be used to localise notation, e.g. some
special-purpose notation used to prove D but is not used elsewhere in the paper. The design philosophy here 
is similar to that of information hiding in software engineering. (Other relevant software engineering 
philosophies for mathematical writing include structured programming and modularity.)

Lemmas also provide a good opportunity to explicitly “recap” all the running hypotheses, assumptions, and
notational conventions that have already been introduced in the argument, which can be invaluable to a
reader who has misunderstood or forgotten about part of this implied context. (Sometimes, such a recap would
be tediously long, in which case a sentence such as “Let the notation and assumptions be as above” may 
suffice. When these situations occur, one might wish to formalise all the running assumptions by judiciously
introducing some good notation.)

In some cases, the conclusion of the lemma may only need a portion of these hypotheses; this might be worth 
stating explicitly within the statement of the lemma, as it can clarify the nature of that lemma, and may 
also make it more useful for future applications.

One should write the statement of a lemma in a way that makes it easy to use, rather than easy to prove. 
Thus, one should try to make the hypotheses of the lemma natural and easy to verify, and the conclusions
of the lemma manifestly useful. Basically, the idea is to push as much of the details of the argument 
into the lemma as one can, to make the rest of the argument as simple as possible. Also, it may end up 
that you (or someone else) will eventually find a simpler proof of that lemma, thus reducing the net
complexity of the paper markedly (cf. the object-oriented approach to software engineering).

Folding the argument into lemmas also makes it easier to write a rapid prototype, as once one finalises 
the statement of the lemma, one can defer the proof of the lemma until later.

In summary, it’s almost always a good idea to have plenty of lemmas (and propositions and corollaries too,
of course) in an argument; it makes the overall structure of the argument more apparent, it makes the 
argument easier to follow, and can also provide some useful tools for future work in the area.
```

More on [avoiding premature optimization](https://terrytao.wordpress.com/advice-on-writing-papers/dont-overoptimise/) -- see also [the same in computer science](#premature-optimization) and [readability in writing](#readability):

```markdown
here is a danger in being too perfectionist, and in trying to make every part of a paper as “optimal” 
as possible. After all the “easy” improvements have been made to a paper, one encounters a law of 
diminishing returns, in which any further improvements either require large amounts of time and effort,
or else require some tradeoffs in other qualities of the paper.

For instance, suppose one has a serviceable lemma that suffices for the task of proving the main
theorems of the paper at hand. One can then try to “optimise” this lemma by making the hypotheses weaker
and the conclusion stronger, but this can come at the cost of lengthening the proof of the lemma, and 
obscuring exactly how the lemma fits in with the rest of the paper. In the reverse direction, one could
also “optimise” the same lemma by replacing it with a weaker (but easier to prove) statement which still
barely suffices to prove the main theorem, but is now unsuitable for use in any later application. Thus
one encounters a tradeoff when one tries to improve the lemma in one direction or another. (In this case,
one resolution to this tradeoff is to have one formulation of the lemma stated and proved, and then add 
a remark about the other formulation, i.e. state the strong version and remark that we only use a special
case, or state the weak version and remark that stronger versions are possible.)

Carefully optimising results and notations in the hope that this will help future researchers in the 
field is a little risky; later authors may introduce new insights or new tools which render these 
painstakingly optimised results obsolete. The only time when this is really profitable is when you already 
know of a subsequent paper (perhaps a sequel to the one you are already writing) which will indeed rely
heavily on these results and notations, or when the current paper is clearly going to be the definitive 
paper in the subject for a long while.

If you haven’t already written a rapid prototype for your paper, then optimising a lemma may in fact be a 
complete waste of time, because you may find later on in the writing process that the lemma will need to
be modified anyway to deal with an unforeseen glitch in the original argument, or to improve the overall 
organisation of the paper.

I have sometimes seen authors try to optimise the length of the paper at the expense of all other
attributes, in the mistaken belief that brevity is equivalent to simplicity. While it can be that shorter
papers are simpler than longer ones, this is generally only true if the shortness of the paper was
achieved naturally rather than artificially. If brevity was attained by removing all examples, remarks,
whitespace, motivation, and discussion, or by striking out “redundant” English phrases and relying purely
on mathematical abbreviations (e.g. \forall instead of “For all”, etc.) and various ungrammatical
contractions, then this is generally a poor tradeoff; somewhat ironically, a paper which has been 
overcompressed may be viewed by readers as being more difficult to read than a longer, gentler, and more 
leisurely treatment of the same material. (See also “Give appropriate amounts of detail.”)

On the other hand, optimising the readability of the paper is always a good thing (except when it is at
the expense of rigour or accuracy), and the effort put into doing so is appreciated by readers.
```

More on [Maximising the results-to-effort ratio](https://terrytao.wordpress.com/advice-on-writing-papers/maximising-the-results-to-effort-ratio/):

```markdown
As a professional courtesy, research papers in mathematics should be at a “local maximum” with respect
to the results-to-effort ratio: any “cheap” consequences, generalisations, variants, illustrative
counterexamples, etc. of one’s main results should be put into the paper if this can be done with only
moderate effort on the author’s part.  If one is too lazy to do this, these consequences might not 
appear in the literature for some time (as they are too close to your own paper to be separately
publishable in their own right), and each reader may have to rederive them by himself or herself, which
is a much less efficient process in the long run.

Conversely, if a huge fraction of the paper is devoted to only a minor extension of the main results,
one may consider removing that section, or replacing it by a sketch or even just a remark; it may be 
that a subsequent paper is able to achieve that result with much less effort anyway.
```

<a name="#Common-misconceptions"></a>
## Common misconceptions
([overview](#overview))  

<a name="#Misconceptions-about-relativity"></a>
### Misconceptions about relativity
([overview](#overview))  

From [Philip Freeman's answer](https://qr.ae/TW1mSb) to the Quora question "If spacetime can bend, stretch, and ripple, could there be a possible “tear” in spacetime?", which Viktor approves of:

```markdown
OK, everybody repeat after me:

Spacetime is NOT a fabric. 
Spacetime is NOT a rubber sheet. 
Spacetime does not bend, stretch, ripple or tie-dye.

Analogy is awesome. It is how our brains work. But analogies are also dangerous because
they are inherently *wrong*. 

Spacetime is (probably) not a THING. Spacetime is the set of connections between things/
events. Image all the things that are happening, everywhere, everywhen. They are all 
connected by real and potential cause and effect, they all have real and potential 
measured separations. These are the “things” that spacetime really is. We can imagine 
them as a weave linking all these events and things, but that’s a picture not the reality.
The reality is just the connections between things and the pattern of that. That pattern
does have a reality… it can be usefully thought of as a field and it can contain energy 
and momentum, so it isn’t really all that wrong to call it a thing. But it has no physical
interconnection, no elasticity or resilience. It doesn’t ‘push on things’ (at least not 
the way we think of things doing that) and it doesn’t really behave like a rubber sheet 
at all.

When we say that spacetime is distorted we mean that the pattern of connections is
different than we’d normally expect (called “flat spacetime”, yes, we’re victims of
analogy too, though the physicists using that term do know what it means mathematically, 
and it isn’t because it is flat). The distortions are distortions in the metric, the 
pattern of interconnections. Such distortions can cause, for example, a region of space to 
have a larger volume than you’d expect from its surface area. That’s mathematically 
described using a term called “curvature”. Sometimes those distortions cause a region to
have an energy density… we call that “pressure” (because the units of pressure are 
joules/metre^3). And so on.

Those patterns can, under certain circumstances, produce real or apparent ‘discontinuities’,
most of which (like an event horizon) are byproducts of making our observations of
interconnections from a certain point of view, so a different point of view can smooth them
out. A few (like the singularity described at the centre of a black hole) can’t be erased 
this way — which pretty much everyone thinks means that our theory has a hole, not spacetime!

So… spacetime isn’t really the sort of thing that can rip. It isn’t really a sort of thing 
at all, except for having the admittedly thing-ish ability to hold momentum-energy. And
ultimately to follow your (admirable) desire to understand this more you’ll have to learn 
more about the real thing, not the fake version that you’ve been peddled.
```

See also [Teaching Physics](https://xkcd.com/895/) by Randall Munroe of xkcd.

