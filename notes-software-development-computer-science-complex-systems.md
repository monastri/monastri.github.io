*[Word count](https://wordcounter.net/): 41,400*

## What is this?

This is the "software development, computer science and complex systems" section of [this notebook](https://github.com/monastri/monastri.github.io/blob/master/quotes.md), last updated Apr 6, 2019, which got so big (1.2 million char) that GitHub refused to render the whole page anymore, ruining my original dream of having my entire notebook in one long page for two purposes: (1) zero-latency clickthrough to make up for my working memory's sand-thru-sieve transience; (2) lower activation energy for continuous document-wide refactoring, to aid recall and cross-domain interlinking.

That said, this is a "living document", a "perpetual draft" in [the style of Gwern](https://www.gwern.net/About#long-content). I'm particulary taken by the following quote: 

```markdown
I have read blogs for many years and most blog posts are the triumph of the hare over the tortoise.
They are meant to be read by a few people on a weekday in 2004 and never again, and are quickly
abandoned—and perhaps as Assange says, not a moment too soon. (But isn’t that sad? Isn’t it a 
terrible ROI for one’s time?) On the other hand, the best blogs always seem to be building something:
they are rough drafts—works in progress. (EY's early contributions to LW is an example; Robin 
Hanson's OB blog is the *anti*-example.) 

I did not wish to write a blog. Then what? More than just “evergreen content”, what would constitute 
Long Content as opposed to the existing culture of Short Content? How does one live in a Long Now 
sort of way?

My answer is that one uses such a framework to work on projects that are too big to work on normally
or too tedious. ...Knowing your site will survive for decades to come gives you the mental wherewithal
to tackle long-term tasks like gathering information for years, and such persistence can be useful --
if one holds onto every glimmer of genius for years, then even the dullest person may look a bit like
a genius himself. Half the challenge of fighting procrastination is the pain of starting—I find when 
I actually get into the swing of working on even dull tasks, it’s not so bad. 

So this suggests a solution: never start. Merely have perpetual drafts, which one tweaks from time to
time. And the rest takes care of itself.
```

(There's also the parallel to [perpetual beta](https://breakingsmart.com/en/season-1/running-code-and-perpetual-beta/) for web-based software: scaffolding for extensive ongoing experimentation within the already-deployed app. Never start, as Gwern says.)

There's also this quote from Paul Graham's essay [You weren't meant to have a boss](http://www.paulgraham.com/boss.html), [paraphrased](https://meltingasphalt.com/about/) by Kevin Simler:

```markdown
An obstacle downstream propagates upstream. If you're not allowed to implement new ideas, 
you stop having them. And vice versa: when you can do whatever you want, you have more 
ideas about what to do. So [keeping a blog] makes your brain more powerful in the same way
a low-restriction exhaust system makes an engine more powerful.
```

This is my first experiment in Gwern's vein. The quotes here have been collected over more than half a decade, albeit in different pages. I intend for them to shape my worldview; doing so like this allows, or so I hope, the shaping to be more fine-grained and guided than the recency-weighted randomness of normal worldview-shaping. (Or at least that was the original intent before I had to break up the notebook. Now I'm not so sure I can do this.)

I also really, *really* hate experiences of the [Jeremy Bentham type](https://github.com/monastri/monastri.github.io/blob/master/notes-amazing-people.md#Jeremy-bentham). This document is intended to prevent them from happening again.

Besides Gwern Branwen, [Cosma Shalizi's notebooks](http://bactra.org/notebooks/) (indeed his [entire oeuvre](http://bactra.org/)) are another major inspiration behind this document. 

<a name="#overview"></a>

## Overview

I've sorted the quotes below into the following categories. This is a provisional taxonomy, subject to perpetual refactoring. The reason it has a [Borgesian flavor](https://github.com/monastri/monastri.github.io/blob/master/poetry.md#the-celestial-emporium-of-benevolent-knowledge) is that it's meant to aid recall and idea-building. The categories are ordered alphabetically; the actual quotes (the top-level categories that is) are chronologically added.

1. [Amazon vs Google comparison (2011)](#Amazon-vs-Google-2011)
2. [CS is beyond the glass ceiling of popular science](#CS-is-beyond-the-glass-ceiling-of-pop-science)
2. [Curse of the gifted programmer](#Curse-of-the-gifted-programmer)
2. [Debugging](#Debugging)
	1. [Systematic debugging is a fundamental skill](#Systematic-debugging-is-a-fundamental-skill)
2. [Esolangs](#Esolangs)
	1. [What esolangs are, and why](#What-are-esolangs)
	1. [Daniel Temkin on code art](#Temkin-on-code-art)
	2. [Intentionally unusable, uncomputable, or conceptual languages](#Language-without-code)
	3. [INTERCAL](#intercal)
2. [Hacking](#Hacking)
2. [Perpetual beta](#Perpetual-beta)
2. [Practical magic](#practical-magic)
2. [Non-pathological programming languages](#Programming-languages)
	1. [Smalltalk](#smalltalk), ft. misconception corrections by Alan Kay
2. [Operating systems](#Operating-systems)
	1. [Why OSes?](#Why-operating-systems)
	2. [OSes as stack of metaphors](#Operating-systems-as-stack-of-metaphors)
	3. [Selling OSes was a radical idea](#Selling-operating-systems-was-a-radical-idea)
2. [Optimization](#Optimization)
	1. [Performance optimization done properly](#Performance-optimization), pretty much all Carlos Bueno 
	2. [The unreasonable effectiveness of a thousand small optimizations](#The-unreasonable-effectiveness-of-a-thousand-small-optimizations)
2. [Software complexity](#Software-complexity)
	1. [The many faces of software complexity](#The-many-faces-of-software-complexity)
	2. [Codebase as organism](#codebase-as-organism)
	2. [Second-system effect, or well-intended redesign bloat](#Second-system-effect)
	3. [Single-handedly designing large codebases](#Single-handedly-designing-large-codebases), Wolfram's 10,000 hours of design reviews
	4. [No, you can't write a better Google in a weekend](#You-cannot-write-a-better-Google-in-a-weekend)
2. [Systems galore: complex systems, complexity science, systems theory](#Complex-systems-and-systems-theory)		
	1. [How complex systems fail](#How-complex-systems-fail)
3. [The conservative-liberal axis in software development](#yegges-conservative-liberal-axis)   
5. [Theoretical CS contributions, or, CS as quantitative epistemology](#Theoretical-CS-contributions)  
2. [Why platforms matter](#platforms)

---------------------------------------


<a name="#Curse-of-the-gifted-programmer"></a>
## Curse of the gifted programmer
([overview](#overview))

The go-to is Eric Raymond's email to Linus Torvalds, [Move of input drivers, some word needed from you](http://lwn.net/2000/0824/a/esr-sharing.php3). Always interesting to see two giants go at it; didn't know ESR and Linus are from two different generations.

Key phrase -- "the scale of the problem always increases to the point where native talent alone doesn't cut it anymore":

```markdown
I'm not arguing that splitting a driver is always wrong -- I can
easily imagine making that call myself in your shoes, and for the
exact reasons you give.  I'm arguing that the perspective from which
you approach this issue causes you to underweight the benefits of
sharing code, and to not look for ways to do it as carefully and
systematically as you ought.

When you were in college, did you ever meet bright kids who graduated
top of their class in high-school and then floundered freshman year 
in college because they had never learned how to study?  It's a common
trap.  A friend of mine calls it "the curse of the gifted" -- a tendency
to lean on your native ability too much, because you've always been
rewarded for doing that and self-discipline would take actual work.

You are a brilliant implementor, more able than me and possibly (I say
this after consideration, and in all seriousness) the best one in the
Unix tradition since Ken Thompson himself.  As a consequence, you
suffer the curse of the gifted programmer -- you lean on your ability
so much that you've never learned to value certain kinds of coding
self-discipline and design craftsmanship that lesser mortals *must*
develop in order to handle the kind of problem complexity you eat for
breakfast.

Your tendency to undervalue modularization and code-sharing is one
symptom.  Another is your refusal to use systematic version-control or
release-engineering practices.  To you, these things seem mostly like
overhead and a way of needlessly complicating your life.  And so far,
your strategy has worked; your natural if relatively undisciplined
ability has proved more than equal to the problems you have set it.
That success predisposes you to relatively sloppy tactics like
splitting drivers before you ought to and using your inbox as a patch
queue.

But you make some of your more senior colleagues nervous.  See, we've
seen the curse of the gifted before.  Some of us were those kids in
college.  We learned the hard way that the bill always comes due --
the scale of the problems always increases to a point where your
native talent alone doesn't cut it any more.  The smarter you are, the
longer it takes to hit that crunch point -- and the harder the
adjustment when you finally do.  And we can see that *you*, poor damn
genius that you are, are cruising for a serious bruising.

As Linux grows, there will come a time when your raw talent is not
enough.  What happens then will depend on how much discipline about
coding and release practices and fastidiousness about clean design you
developed *before* you needed it, back when your talent was sufficient
to let you get away without.  The code-sharing issue -- more
specifically, your tendency to abandon modularization and re-use
before you probably ought to -- is part of this.  Andy Tanenbaum's
charge against you was not entirely without justice.

The larger problem is a chronic topic of face-to-face conversation
whenever two or more senior lkml people get together and you aren't
around.  You're our chosen benevolent dictator and maybe the second
coming of Ken, and we respect you and like you, but that doesn't mean
we're willing to close our eyes.  And when you react to cogent and
well-founded arguments like Rogier Wolff's as you have -- well, it
makes us more nervous.

I used to worry about what would happen if Linus got hit by a truck.
With all respect, I still worry about what will happen if the
complexity of the kernel exceeds the scope of your astonishing native
talent before you grow up.
```

On a smaller scale is a phenomenon you see in college often. Dan Luu recounts one such personal anecdote in [Teach debugging](https://danluu.com/teach-debugging/#fn:2):

```markdown
In the fall of 2000, I took my first engineering class: ECE 352, an entry-level
digital design class for first-year computer engineers. It was standing room 
only, filled with waitlisted students who would find seats later in the 
semester as people dropped out. We had been warned in orientation that half of
us wouldn't survive the year. In class, We were warned again that half of us 
were doomed to fail, and that ECE 352 was the weed-out class that would be
responsible for much of the damage.

The class moved briskly. The first lecture wasted little time on matters of the
syllabus, quickly diving into the real course material. Subsequent lectures 
built on previous lectures; anyone who couldn't grasp one had no chance at the 
next. Projects began after two weeks, and also built upon their predecessors; 
anyone who didn't finish one had no hope of doing the next.

A friend of mine and I couldn't understand why some people were having so much
trouble; the material seemed like common sense. The Feynman Method was the only
tool we needed.

Write down the problem
Think real hard
Write down the solution
The Feynman Method failed us on the last project: the design of a divider, a
real-world-scale project an order of magnitude more complex than anything we'd 
been asked to tackle before. On the day he assigned the project, the professor
exhorted us to begin early. Over the next few weeks, we heard rumors that some
of our classmates worked day and night without making progress.

But until 6pm the night before the project was due, my friend and I ignored all
this evidence. It didn't surprise us that people were struggling because half 
the class had trouble with all of the assignments. We were in the half that 
breezed through everything. We thought we'd start the evening before the
deadline and finish up in time for dinner.

We were wrong.

An hour after we thought we'd be done, we'd barely started; neither of us had a 
working design. Our failures were different enough that we couldn't productively
compare notes. The lab, packed with people who had been laboring for weeks 
alongside those of us who waited until the last minute, was full of bad news:
a handful of people had managed to produce a working division unit on the first
try, but no one had figured how to convert an incorrect design into something
that could do third-grade arithmetic.

I proceeded to apply the only tool I had: thinking really hard. That method, 
previously infallible, now yielded nothing but confusion because the project was
too complex to visualize in its entirety. I tried thinking about the parts of 
the design separately, but that only revealed that the problem was in some
interaction between the parts; I could see nothing wrong with each individual 
component. Thinking about the relationship between pieces was an exercise in
frustration, a continual feeling that the solution was just out of reach, as 
concentrating on one part would push some other critical piece of knowledge out 
of my head. The following semester I would acquire enough experience in managing
complexity and thinking about collections of components as black-box abstractions
that I could reason about a design another order of magnitude more complicated 
without problems -- but that was three long winter months of practice away, and 
this night I was at a loss for how to proceed.

By 10pm, I was starving and out of ideas. I rounded up people for dinner, hoping
to get a break from thinking about the project, but all we could talk about was 
how hopeless it was. How were we supposed to finish when the only approach was to
flawlessly assemble thousands of parts without a single misstep? It was a tedious
version of a deranged Atari game with no lives and no continues. Any mistake was 
fatal.

A number of people resolved to restart from scratch; they decided to work in pairs
to check each other's work. I was too stubborn to start over and too inexperienced
to know what else to try. After getting back to the lab, now half empty because so
many people had given up, I resumed staring at my design, as if thinking about it 
for a third hour would reveal some additional insight.

It didn't. Nor did the fourth hour.

And then, just after midnight, a number of our newfound buddies from dinner 
reported successes. Half of those who started from scratch had working designs. 
Others were despondent, because their design was still broken in some subtle, non-
obvious way. As I talked with one of those students, I began poring over his design.
And after a few minutes, I realized that the Feynman method wasn't the only way 
forward: it should be possible to systematically apply a mechanical technique 
repeatedly to find the source of our problems. Beneath all the abstractions, our 
projects consisted purely of NAND gates (woe to those who dug around our toolbox
enough to uncover dynamic logic), which outputs a 0 only when both inputs are 1. If
the correct output is 0, both inputs should be 1. The input that isn't is in error,
an error that is, itself, the output of a NAND gate where at least one input is 0 
when it should be 1. We applied this method recursively, finding the source of all
the problems in both our designs in under half an hour.

We excitedly explained our newly discovered technique to those around us, walking
them through a couple steps. No one had trouble; not even people who'd struggled with
every previous assignment. Within an hour, the group of folks within earshot of us 
had finished, and we went home.

I understand now why half the class struggled with the earlier assignments. Without 
an explanation of how to systematically approach problems, anyone who didn't 
intuitively grasp the correct solution was in for a semester of frustration. People 
who were, like me, above average but not great, skated through most of the class and
either got lucky or wasted a huge chunk of time on the final project. I've even seen 
people talented enough to breeze through the entire degree without ever running into
a problem too big to intuitively understand; those people have a very bad time when
they run into a 10 million line codebase in the real world. The more talented the 
engineer, the more likely they are to hit a debugging wall outside of school.
```

<a name="#Debugging"></a>
## Debugging
([overview](#overview))

<a name="#Systematic-debugging-is-a-fundamental-skill"></a>
### Systematic debugging is a fundamental skill
([overview](#overview))

From Dan Luu's blog post [Teach debugging](https://danluu.com/teach-debugging/), recounting his experience taking a "weeder class" back in the day. Memorable for the last line -- "for all the high-level talk about how we need to plug the leaks in our STEM education pipeline, not only are we not plugging the holes, we're proud of how fast the pipeline is leaking":

```markdown
What I don't understand is why schools don't teach systematic debugging. It's one
of the most fundamental skills in engineering: start at the symptom of a problem 
and trace backwards to find the source. It takes, at most, half an hour to teach
the absolute basics – and even that little bit would be enough to save a
significant fraction of those who wash out and switch to non-STEM majors. Using 
the standard engineering class sequence of progressively more complex problems, a
focus on debugging could expand to fill up to a semester, which would be enough 
to cover an obnoxious real-world bug: perhaps there's a system that crashes once
a day when a Blu-ray DVD is repeatedly played using hardware acceleration with a
specific video card while two webcams and record something with significant 
motion, as long as an obscure benchmark from 1994 is running. 

	This is an actual CPU bug I saw that took about a month to track down. And this
	is the easy form of the bug, with a set of ingredients that causes the fail to
	be reproduced about once a day -- the original form of the bug only failed once
	every few days. I'm not picking this example because it's particularly hard, 
	either: I can think of plenty of bugs that took longer to track down and had 
	stranger symptoms, including a disastrous bug that took six months for our best
	debugger to understand.
	
	For ASIC post-silicon debug folks out there, this chip didn't have anything 
	close to full scan, and our only method of dumping state out of the chip
	perturbed the state of the chip enough to make some bugs disappear. Good times.
	On the bright side, after dealing with non-deterministic hardware bugs with 
	poor state visibility, software bugs seem easy. At worst, they're boring and
	tedious because debugging them is a matter of tracing things backwards to the 
	source of the issue.
	
This dynamic isn't unique to ECE 352, or even Wisconsin – I saw the same thing when
TA'ed EE 202, a second year class on signals and systems at Purdue. The problems 
were FFTs and Laplace transforms instead of dividers and Boolean2, but the avoidance
of teaching fundamental skills was the same. It was clear, from the questions 
students asked me in office hours, that those who were underperforming weren't 
struggling with the fundamental concepts in the class, but with algebra: the 
problems were caused by not having an intuitive understanding of, for example, the
difference between f(x+a) and f(x)+a.

When I suggested to the professor that he spend half an hour reviewing algebra for 
those students who never had the material covered cogently in high school, I was told
in no uncertain terms that it would be a waste of time because some people just can't
hack it in engineering. I was told that I wouldn't be so naive once the semester was 
done, because some people just can't hack it in engineering. I was told that helping
students with remedial material was doing them no favors; they wouldn't be able to 
handle advanced courses anyway because some students just can't hack it in engineering.
I was told that Purdue has a loose admissions policy and that I should expect a high 
failure rate, because some students just can't hack it in engineering.

I agreed that a few students might take an inordinately large amount of help, but it 
would be strange if people who were capable of the staggering amount of memorization
required to pass first year engineering classes plus calculus without deeply
understanding algebra couldn't then learn to understand the algebra they had memorized. 
I'm no great teacher, but I was able to get all but one of the office hour regulars up
to speed over the course of the semester. An experienced teacher, even one who doesn't
care much for teaching, could have easily taught the material to everyone.

Why do we leave material out of classes and then fail students who can't figure out 
that material for themselves? Why do we make the first couple years of an engineering 
major some kind of hazing ritual, instead of simply teaching people what they need to
know to be good engineers? For all the high-level talk about how we need to plug the 
leaks in our STEM education pipeline, not only are we not plugging the holes, we're 
proud of how fast the pipeline is leaking.	
```


<a name="#Perpetual-beta"></a>
## Perpetual beta
([overview](#overview)) 

From Venkat Rao's [Breaking Smart newsletter](https://breakingsmart.com/en/season-1/running-code-and-perpetual-beta/) on the topic. 

```markdown
All modern web-based software includes scaffolding for extensive ongoing 
experimentation within the deployed production site or smartphone app 
backend (and beyond, through developer APIs). Some of it is even visible 
to users. In addition to experimental features that allow users to stay 
ahead of the curve, many services also offer “classic” settings that allow
them to stay behind the curve — for a while. The best products use 
perpetual beta as a way to lead their users towards richer, more empowered
behaviors, instead of following them through customer-driven processes. 
Backward compatibility is limited to situations of pragmatic need, rather
than being treated as a religious imperative.

How does anything ambitious get finished by groups of stubborn individuals
heading in the foggiest possible direction of “maximal interestingness” with
neither purist visions nor “customer needs” guiding them?

The answer is that it *doesn’t* get finished. But unlike in waterfall models,
this does not necessarily mean the *product* is incomplete. It means the *vision*
is perpetually incomplete and growing in unbounded ways, due to ongoing 
evolutionary experiments. When this process works well, what engineers call 
technical debt can get transformed into what we might call technical surplus.
The parts of the product that lack satisfying design justifications represent
the areas of rapid innovation. The gaps in the vision are sources of 
serendipitous good luck. (If you are a Gmail user, browsing the “Labs” section
might lead you to some serendipitous discoveries: features you did not know
you wanted might already exist unofficially).

The deeper significance of perpetual beta culture in technology often goes
unnoticed: in the industrial age, engineering labs were impressive, enduring
buildings inside which experimental products were created. In the digital 
age, engineering labs are experimental sections inside impressive, enduring
products. Those who bemoan the gradual decline of famous engineering labs 
like AT&T Bell Labs and Xerox PARC often miss the rise of even more impressive 
labs inside major modern products and their developer ecosystems.
```

Corollary to perpetual beta:

```markdown
Just as rough consensus drives ideation towards “maximal interestingness”,
agile processes drive evolution towards the regimes of greatest operational
uncertainty, where failures are most likely to occur. In well-run modern 
software processes, not only is the resulting chaos tolerated, it is 
actively invited. Changes are often deliberately made at seemingly the worst
possible times. 

Intuit, a maker of tax software, has a history of making large numbers of 
changes and updates at the height of tax season.

Conditions that cause failure, instead of being cordoned off for avoidance
in the future, are deliberately and systematically recreated and explored 
further. There are even automated systems designed to deliberately cause 
failures in production systems, such as ChaosMonkey, a system developed by
Netflix to randomly take production servers offline, forcing the system to
heal itself or die trying.

This is neither perverse, nor masochistic: it is necessary to uncover hidden
risks in experimental ideas early, and to quickly resolve gridlocks with data.

The origins of this curious philosophy lie in what is known as the release 
early, release often (RERO) principle, usually attributed to Linus Torvalds,
the primary architect of the Linux operating system. The idea is exactly what
it sounds like: releasing code as early as possible, and as frequently as 
possible while it is actively evolving.

What makes this possible in software is that most software failures do not
have life-threatening consequences. As a result, it is usually faster and 
cheaper to learn from failure than to attempt to anticipate and accommodate
it via detailed planning (which is why the RERO principle is often restated 
in terms of failure as fail fast).

	This is not true of all software of course: there is a different 
	development regime for code with life-threatening consequences. 
	Code developed in such regimes tends to evolve far more slowly 
	and is often between 10-30 years behind the curve. This is one
	reason for the perception that trivial applications dominate the 
	industry: it takes longer for mission-critical code in life-
	threatening applications to be updated.

So crucial is the RERO mindset today that many companies, such as Facebook
and Etsy, insist on new hires contributing and deploying a minor change to 
mission-critical systems on their very first day. Companies that rely on 
waterfall processes by contrast, often put new engineers through years of 
rotating assignments before trusting them with significant autonomy.

To appreciate just how counterintuitive the RERO principle is, and why it 
makes traditional engineers nervous, imagine a car manufacturer rushing to 
put every prototype into “experimental” mass production, with the intention
of discovering issues through live car crashes. Or supervisors in a 
manufacturing plant randomly unplugging or even breaking machinery during peak
demand periods. Even lean management models in manufacturing do not go this 
far. Due to their roots in scarcity, lean models at best mitigate the problems
caused by waterfall thinking. Truly agile models on the other hand, do more: 
they catalyze abundance.

Perhaps the most counter-intuitive consequence of the RERO principle is this: 
where engineers in other disciplines attempt to minimize the number of releases,
software engineers today strive to maximize the frequency of releases. The 
industrial-age analogy here is the stuff of comedy science fiction: an intern 
launching a space mission just to ferry a single paper-clip to the crew of a 
space station.

This tendency makes no sense within waterfall models, but is a necessary feature 
of agile models. The only way for execution to track the changing direction of 
the rough consensus as it pivots is to increase the frequency of releases. Failed
experiments can be abandoned earlier, with lower sunk costs. Successful ones can
migrate into the product as fast as hidden risks can be squeezed out. As a result,
a lightweight sense of direction — rough consensus — is enough. There is no need
to navigate by an increasingly unattainable utopian vision.
```

Not convinced/impressed, but perhaps that's my backwards mindset talking; in any case it's a nice example of perception refactoring. Another issue is causality tracing: *why* did the system fuck up, *which* release caused it? That segues into complex systems stuff. 

<a name="#Esolangs"></a>
## Esolangs
([overview](#overview)) 

Ben Olmstead (creator of Malbolge) describes esolangs as “pushing the boundaries of programming, but not in useful directions.”

<a name="#What-are-esolangs"></a>
### What are esolangs
([overview](#overview)) 

Daniel Temkin on programming languages in general:

```markdown
We might think of languages as being software-like themselves, but this is 
not quite right; they’re more immaterial than software. Languages are lists 
of rules about how to interpret combinations of symbols, that sometimes are
used to write programs. They are more like a(n Oulipean) field of potential
software; tools that can be used in infinite different ways but have their
own logic of getting to that goal.
```

or: 

```markdown
Languages are already almost nothing: sets of rules, with no particular implementation. 
```

More discussion in [Language without code](http://artes.ucp.pt/citarj/article/view/432/212):

```markdown
Surprisingly, this
concept is hard to pin down. It is usually defined
through utility: a programming language is used to
express commands to a computer. The Merriam
Webster definition, Wikipedia's definitions (both the
longest-posted one and the one currently posted at
the time of writing) are all variations of these,
sometimes with "formal language" mentioned, which
at least points to a substantial difference from natural
language.

Wikipedia helpfully notes that the first programming
languages were used for automation before
existence of the digital computer, which points to
perhaps the biggest issue with the term: what is a
computer and do we need it to execute code? Before
the first modern digital computer, we had the Turing
Machine, a purely theoretical automaton used for
mathematical proofs about computation. Are we
defining programming languages in terms of
computers as they are today? As we imagine them
tomorrow? Or always in terms of the theoretical
machine, as the first languages were designed?
Microsoft, IBM, and others have designed quantum
computing languages for computers that don't yet
physically exist and perhaps won’t, at least as they
are currently conceived (Simonite, 2017). While we
have a system of computational complexity that
shows the algorithmic potential of a language, as we
will see through example, there is no established
lower boundary of what we expect programming
languages to be capable of in order to consider them
languages. As the (possibly apocryphal but wholly
-incharacter) quote from Edsger Dijkstra goes,
"Computer science is no more about computers than
astronomy is about telescopes". 

Programming languages as logical systems lacking in
ambiguity, along with their relentlessly imperative
tone (even for the non-imperative languages, which
are different in form but not in mood)—are perhaps
what most clearly differentiate programming
languages from natural language. 
```

Chris Pressey is a central figure of esolangs; he ran the mailing list where the first community of esolangs came together. In [*The Aesthetics of Esolangs*](http://catseye.tc/node/The_Aesthetics_of_Esolangs), he argues that esolangs can be understood as art, but not as a form of digital art: 

```markdown
...they’re made up of concepts, and these concepts would exist even if our
computing equipment wasn’t electronic, or wasn’t digital, or if we didn’t
have computing equipment at all. It’s just that having computing equipment 
makes it a lot easier to design and experience these programming languages.

The rules are the work, and the fact that these rules produce runnable code 
is secondary.
```

As to why esolangs -- there's a lot of nostalgia:

```markdown
Where code golf and obfuscated code willingly embrace esoteric methods of
programming, we can also see in these alternate methods a breaking away from 
the safety of high-level languages, a call back to what programming was like 
in the days of machine code – particularly in esolangs themselves. 

Wendy Hui Kyong Chun has written about how giving up the direct interface with
the machine was hard for early programmers. Chun quotes John Backus, developer
of FORTRAN about the “black art” of early coding, saying they had a

	chauvinistic pride in their frontiersmanship and a corresponding
	conservatism, so many programmers of the 1950s began to regard themselves 
	as members of a priesthood guarding skills and mysteries far too complex 
	for ordinary mortals. Languages like FORTRAN opened up this world to
	people who were not trained in this black art.

In a sense, alternative coding practices recreate this sense of code as an
esoteric knowledge. Here not in a chauvansitic way, but with a sense of 
excitement in breaking new ground within deliberately obscure rules offered by
an esolang or a set of code golf constraints. Each esolang creating a unique 
means of communicating with the computer that make sense only to esoprogrammers
willing to bypass the niceties of mainstream computing. Esolangs may convolute
code but do it in a way that gives esolangers access to low-level activity 
masked in the name of safety and ease provided by these high level languages. 
As crazy as brainfuck looks, it forces one to deal with memory cells directly;
much of the delight of the language is in this engagement with the machine
which is obscured by the safety of high level code and the “humble” approach 
of reducing complexity. The most extreme of which is probably Checkout, a 
language proposal that tries to give direct chip access to the programmer.
```

Scott Feeney, founder of esolangs.org:

```markdown
I think what’s most interesting about
esolangs is the conversation between
languages, which ask questions, and
programs written in those languages, which
answer the questions. When you build a new
esoteric language with a weird set of
constraints, you get people thinking: I wonder
if I can do X in this language? I wonder if
there’s a way to do Y? And figuring that out,
by writing programs that do X and Y, can be
a fun challenge.
```

Why do esolangs strive for Turing completeness? Because it's aesthetic to show that a strange idea is also very expressive/powerful:

```markdown
For example, the highly influential
esolang brainfuck (typically spelled lower-case)
expresses all code in eight commands, each
represented by a punctuation mark. What makes
brainfuck interesting is how such a minimal language
with such odd logic is provably as powerful a
language as Python or C, despite having no built-in
representation of the number 2 or of the action of
multiplication. 
```

<a name="#Temkin-on-code-art"></a>
## Temkin on code art
([overview](#overview)) 

From the wild frontier of Temkin's page [Sentences on Code Art](https://esoteric.codes/blog/sentences-on-code-art) -- there are lots of hyperlinks to example esolangs illustrating the claimed properties in the original page, so do check it out:

```markdown
0. Computers are logical systems that arise as often by accident as by design.

1. Their core materiality is logic, not pixels or circuits or bits or other 
features of their physical implementation. Other implementations are possible.

2. Our engagement with logic is irrational because we are irrational beings.
We are incapable of fully asserting our agency through a system that forces us
to translate our intentions into logical steps.

3. This central drama of human / computer interaction is experienced most 
directly at the code level.

4. Bugs are the primary progeny of programmers. We write broken software.

5. Although the machine presents a world of our own making, it rebukes us by not
doing what we want, leading to a compulsive cycle of “fixing” and augmenting code
(as says Joseph Weizenbaum). We are all “computer bums”.

6. For any definition of the term “programming language,” there is a language 
that sits on its border.

7. Programmability is not a requirement for programming languages. Theoretical 
programming languages existed before practical ones. We can create valid languages
whose programs are physically unconstructable or whose executors are logically
impossible.

8. The ambiguity of human language is present in code, which never fully escapes 
its status as human writing, even when machine-generated. We bring to code our 
excesses of language, and an ambiguity of semantics, as discerned by the human 
reader.

9. We don’t need an irrational idea to follow logically; our irrationality will
pollute any attempt at rigor.

A. Banal ideas can be rescued by carrying them out with precision, or even through
increased repetition, as it is hard for us to understand even relatively immediate
repercussions of our actions in the logical space, bringing us again and again to 
unexpected places.
```

<a name="#Language-without-code"></a>
### Language without code
([overview](#overview)) 

Some of the most mind-bending stuff in Daniel Temkin's [eponymous paper](http://artes.ucp.pt/citarj/article/view/432/212). 

The abstract promises/claims a whole lot:

```markdown
Most esolangs are experiential works; we understand the
languages by writing code in them. Through this
action, the logic of the language becomes clear.

However, a smaller subset of esolangs make their
point not through actively writing code, but instead by
simply contemplating their rules. We can think of
these esolangs as conceptual rather than
experiential. Some are designed in such a way that
they don’t allow any code to be written for them at all.

By stepping away from usability, the conceptual
esolangs offer the most direct challenge to the
definition of programming language, a commonly
used term which is surprisingly unspecific, and
usually understood through utility, despite the fact
that programming languages predate digital
computers. 
```

PLs that don't allow code to be written for them at *all?* What does that even *mean?*

Take Three Star Programmer, created in 2015 by ais523:

```markdown
This language asks programmers to write code with
three levels of indirection: pointers to pointers to
pointers to memory cells. A program in Three Star
Programmer is in the form of a string of numbers;
each can be thought of as both raw data and as a
pointer to another location in memory, where that
memory is also the code itself. The numbers are
consecutively read, each dereferenced three times
(meaning the interpreter jumps to the location
corresponding to the number in that cell), until we get
to a final number which is then incremented.
However, that final location is also a pointer (to a
pointer to a pointer), meaning where it points has just
changed. 

On the esolangs wiki, ais523 (the creator of
the language) says "it's very hard to actually write
anything in the language, because of the fundamental
nature of the language, in which everything affects
everything else and no change is really reversible."
Despite this, at the time of writing, it was not yet
known how powerful it was, in terms of the language’s
potential to represent algorithms. 

Between the time of writing and final publication of
this paper, ais523 has reported that the language has 
indeed been proven Turing Complete.
```

Another example is uncomputable code. Take Lenguage:

```markdown
Lenguage embraces the minimalism of brainfuck, and
uses the same command set, with a different
encoding of signifiers. Lenguage’s name is a play on
words; LEN() is the command in many languages that
reports the length of a string. In Lenguage, the length
of the program in characters is the only thing that
matters. A C program could be a Lenguage program
as well, if its length were correct to correspond to a
series of commands (“Lenguage - Esolang,” 2014).

Lenguage asks the question: do we need both 0 and
1? If we're going for pure minimalism, why not just
one symbol? With a vocabulary of undifferentiated
symbols (such as 1s), we could represent code with
anything: the length of a line, or enumerating each in
a pile of rocks.

In Lenguage, this is performed by translating each of
brainfuck's commands into a binary sequence: 000
for + (increment), 001 for - (decrement) etc., and set
in order, to produce a single number. A program with
the length of that number will be read by the
Lenguage interpreter by translating that number into
binary and reading the sequence, giving us the
program.

The Hello World program for Lenguage is any file with
17,498,005,810,995,570,277,424,757,300,680,353,
162,371,620,393,379,153,004,301,136,096,632,219
,477,184,361,459,647,073,663,110,750,484
characters. At 1.75 * 10^102, it's more than a Googol
characters. This means the Hello World program, if
stored at the atomic level (counting individual atoms
to determine the program), would be larger than the
size of the known Universe.
```

A somewhat more "practical" version of Lenguage is Spoon, which lets you just write the number representing the length of the input sequence for Lenguage:

```markdown
Spoon, created by S. Goodwin in 1998, took
brainfuck and represented each of the commands
with a binary sequence, similar to Lenguage. Where
Lenguage took a minimalist approach to variety in
input, Spoon allows us to simply write the number,
rather than use the length of the sequence of the
number. Furthermore, Spoon uses Huffman-encoded
binary sequences, meaning the most commonly used
commands (+ and -) are represented with the shortest
sequence in binary digits; + is a single 1, - is 000. Had
Lenguage used Huffman-encoding, its Hello World
program would be only nineteen quattuorvigintillion,
10^76, only the informational content of a one-solar
mass black hole. 
```

And *then* there's Chris Pressey's derivative of Spoon, called You are Reading the Name of this Esolang (pronounced "You are Hearing the Name of this Esolang"); running programs written in it is equivalent to solving the halting problem:

```markdown
It is Spoon with two additional
symbols; opening and closing brackets. Code held in
the brackets are read as complete Spoon programs
in themselves and executed first. If they complete,
they are translated to 1s and dropped back into the
original sequence. If they do not halt (get stuck in an
infinite loop), they are translated into 0s (“You are
Reading the Name of this Esolang - Esolang,” n.d.).

While some trivial infinite loops can be detected, Alan
Turing proved that there is no generalized solution to
determining whether a piece of code will halt; this is
known as the Halting Problem (Turing, 1937). You are
Reading the Name of this Esolang has taken a
fundamental computational problem and moved it
from the performance of code into the lexical analysis
of code. While some You are Reading the Name of
this Esolang programs may be validated by a human
reader or the compiler, it has been proven definitively
that the machine has no general way to validate a
sequence as being a You are Reading the Name of
this Esolang program. It could take exponential time,
or possibly forever, to compile such a program.
Rather than being larger than the universe, You are
Reading the Name of This Esolang is beyond the
reach of any currently conceivable technology.

Traditional programming languages try to remain
unobtrusive, to let us see how the code will function
as clearly as possible, rather than drawing attention
to its actual structure as symbols on a screen,
esolangs frequently bring our attention back to the
surface layer of the language. With a language like
You are Reading the Name of This Esolang, the
name alone is a constant reminder that we are
dealing with something very different, where the
language is not something we can easily see through,
but a structure to be wrestled with, or a puzzle for us
to ponder and consider in its own right.
```


<a name="#INTERCAL"></a>
### INTERCAL
([overview](#overview)) 

INTERCAL was the first esolang. From Daniel Temkin's [Language without code](http://artes.ucp.pt/citarj/article/view/432/212):

```markdown
INTERCAL (somehow short for "Compiler Language
With No Pronounceable Acronym"), generally
considered the first esolang (it was created in 1972),
included a set of documentation filled with
nonsensical diagrams and misleading statements.
Some aspects of the language were left to be
discovered, or intentionally ambiguous. INTERCAL
required the keyword PLEASE scattered throughout
the program. Not enough PLEASEs and the entire
program would be ignored, as the interpreter found
the program too rude. Too many PLEASEs and the
interpreter saw the programmer as simpering and
also ignored the entire thing. The correct proportion
of PLEASEs to commands was not in the
documentation, leaving the programmer to discover
on her own how to get the program running
(Bratishenko, 2009; Smith, 2007). The PLEASE
command also brings our attention to the one aspect
that nearly all programming languages have in
common: the relentlessness of their commanding
tone.

When INTERCAL was rewritten as C-INTERCAL (by
Eric S. Raymond in 1990), making it available to a
wider audience, he had to choose which features
were critical to maintain and which to modernise. He
chose to better document the language (spoiler: it's
"approximately 3 non-polite identifiers for every polite
identifier used")
```

<a name="#Hacking"></a>
## Hacking
([overview](#overview)) 

I defer here to Richard Stallman himself. In [On hacking](https://stallman.org/articles/on-hacking.html) Stallman writes:

```markdown
It is hard to write a simple definition of something as varied as hacking, but
I think what these activities have in common is playfulness, cleverness, and 
exploration. Thus, hacking means exploring the limits of what is possible, in a
spirit of playful cleverness. Activities that display playful cleverness have 
"hack value".

The hacking community developed at MIT and some other universities in the 1960s
and 1970s. Hacking included a wide range of activities, from writing software, 
to practical jokes, to exploring the roofs and tunnels of the MIT campus. Other
activities, performed far from MIT and far from computers, also fit hackers'
idea of what hacking means: for instance, I think the controversial 1950s 
"musical piece" by John Cage, 4'33" (**/**), is more of a hack than a musical 
composition. The palindromic three-part piece written by Guillaume de Machaut in
the 1300s, "Ma Fin Est Mon Commencement", was also a good hack, even better 
because it also sounds good as music. Puck appreciated hack value.

The concept of hacking excludes wit and art as such. The people who began to speak
of their activities as "hacking" were familiar with wit and art, and with the
names of the various fields of those; they were also doing something else, 
something different, for which they came up with the name "hacking". Thus,
composing a funny joke or a beautiful piece of music may well involve playful 
cleverness, but a joke as such and a piece of music as such are not hacks, however
funny or beautiful they may be. However, if the piece is a palindrome, we can say
it is a hack as well as music; if the piece is vacuous, we can say it is a hack on
music.

Hackers typically had little respect for the silly rules that administrators like 
to impose, so they looked for ways around. For instance, when computers at MIT 
started to have "security" (that is, restrictions on what users could do), some
hackers found clever ways to bypass the security, partly so they could use the
computers freely, and partly just for the sake of cleverness (hacking does not
need to be useful). However, only some hackers did this—many were occupied with
other kinds of cleverness, such as placing some amusing object on top of MIT's 
great dome (*/*), finding a way to do a certain computation with only 5 
instructions when the shortest known program required 6, writing a program to 
print numbers in roman numerals, or writing a program to understand questions in
English. (Hacking does not have to be without practical use.)
```

The chopsticks hack personal anecdote:

```markdown
In June 2000, while visiting Korea, I did a fun hack that clearly illustrates the 
original and true meaning of the word "hacker".

I went to lunch with some GNU fans, and was sitting down to eat some tteokbokki, 
when a waitress set down six chopsticks right in front of me. It occurred to me 
that perhaps these were meant for three people, but it was more amusing to imagine
that I was supposed to use all six. I did not know any way to do that, so I 
realized that if I could come up with a way, it would be a hack. I started thinking.
After a few seconds I had an idea.

First I used my left hand to put three chopsticks into my right hand. That was not
so hard, though I had to figure out where to put them so that I could control them 
individually. Then I used my right hand to put the other three chopsticks into my 
left hand. That was hard, since I had to keep the three chopsticks already in my 
right hand from falling out. After a couple of tries I got it done.

Then I had to figure out how to use the six chopsticks. That was harder. I did not 
manage well with the left hand, but I succeeded in manipulating all three in the 
right hand. After a couple of minutes of practice and adjustment, I managed to pick
up a piece of food using three sticks converging on it from three different 
directions, and put it in my mouth.

It didn't become easy—for practical purposes, using two chopsticks is completely 
superior. But precisely because using three in one hand is hard and ordinarily never
thought of, it has "hack value", as my lunch companions immediately recognized. 
Playfully doing something difficult, whether useful or not, that is hacking.

I later told the Korea story to a friend in Boston, who proceded to put four 
chopsticks in one hand and use them as two pairs—picking up two different pieces of
food at once, one with each pair. He had topped my hack. Was his action, too, a hack? 
I think so. Is he therefore a hacker? That depends on how much he likes to hack.
```

"Hacking" shouldn't be a bad word, but for definitional drift(?); fortunately Stallman and friends have rehabbed it:

```markdown
Yet when I say I am a hacker, people often think I am making a naughty admission, 
presenting myself specifically as a security breaker. How did this confusion develop?

Around 1980, when the news media took notice of hackers, they fixated on one narrow 
aspect of real hacking: the security breaking which some hackers occasionally did.
They ignored all the rest of hacking, and took the term to mean breaking security,
no more and no less. The media have since spread that definition, disregarding our
attempts to correct them. As a result, most people have a mistaken idea of what we
hackers actually do and what we think.

You can help correct the misunderstanding simply by making a distinction between 
security breaking and hacking—by using the term "cracking" for security breaking. 
The people who do it are "crackers". Some of them may also be hackers, just as some 
of them may be chess players or golfers; most of them are not.

I coined the term "cracker" in the early 80s when I saw journalists were equating 
"hacker" with "security breaker".

The campaign to reclaim the word "hacker" from association with security breaking is
doing pretty well, as witness the widespread usage of terms such as "hacklab" and 
"hackathon".
```

<a name="#Operating-systems"></a>
## Operating systems
([overview](#overview)) 

<a name="#why-operating-systems"></a>
### Why operating systems
([overview](#overview)) 

From Neal Stephenson's [In the beginning was the command line](http://cristal.inria.fr/~weis/info/commandline.html), which also talks about why a secret OS is a contradiction in terms:

```markdown
But the basic idea of re-creating an operating system from scratch was perfectly 
sound and completely doable. It has been done many times. It is inherent in the 
very nature of operating systems.

Operating systems are not strictly necessary. There is no reason why a sufficiently
dedicated coder could not start from nothing with every project and write fresh 
code to handle such basic, low-level operations as controlling the read/write heads
on the disk drives and lighting up pixels on the screen. The very first computers 
had to be programmed in this way. But since nearly every program needs to carry out 
those same basic operations, this approach would lead to vast duplication of effort.

Nothing is more disagreeable to the hacker than duplication of effort. The first and
most important mental habit that people develop when they learn how to write computer
programs is to generalize, generalize, generalize. To make their code as modular and
flexible as possible, breaking large problems down into small subroutines that can be
used over and over again in different contexts. Consequently, the development of
operating systems, despite being technically unnecessary, was inevitable. Because at
its heart, an operating system is nothing more than a library containing the most 
commonly used code, written once (and hopefully written well) and then made available
to every coder who needs it.

So a proprietary, closed, secret operating system is a contradiction in terms. It goes
against the whole point of having an operating system. And it is impossible to keep
them secret anyway. The source code--the original lines of text written by the 
programmers--can be kept secret. But an OS as a whole is a collection of small
subroutines that do very specific, very clearly defined jobs. Exactly what those 
subroutines do has to be made public, quite explicitly and exactly, or else the OS is 
completely useless to programmers; they can't make use of those subroutines if they
don't have a complete and perfect understanding of what the subroutines do.

The only thing that isn't made public is exactly how the subroutines do what they do. 
But once you know what a subroutine does, it's generally quite easy (if you are a 
hacker) to write one of your own that does exactly the same thing. It might take a
while, and it is tedious and unrewarding, but in most cases it's not really hard.

What's hard, in hacking as in fiction, is not writing; it's deciding what to write.
And the vendors of commercial OSes have already decided, and published their decisions. 

This has been generally understood for a long time. MS-DOS was duplicated, functionally,
by a rival product, written from scratch, called ProDOS, that did all of the same things
in pretty much the same way. In other words, another company was able to write code that 
did all of the same things as MS-DOS and sell it at a profit. If you are using the Linux
OS, you can get a free program called WINE which is a windows emulator; that is, you can
open up a window on your desktop that runs windows programs. It means that a completely
functional Windows OS has been recreated inside of Unix, like a ship in a bottle. And 
Unix itself, which is vastly more sophisticated than MS-DOS, has been built up from 
scratch many times over. Versions of it are sold by Sun, Hewlett-Packard, AT&T, Silicon
Graphics, IBM, and others.

People have, in other words, been re-writing basic OS code for so long that all of the 
technology that constituted an "operating system" in the traditional (pre-GUI) sense of
that phrase is now so cheap and common that it's literally free. Not only could Gates 
and Allen not sell MS-DOS today, they could not even give it away, because much more
powerful OSes are already being given away. Even the original Windows (which was the 
only windows until 1995) has become worthless, in that there is no point in owning 
something that can be emulated inside of Linux--which is, itself, free.

In this way the OS business is very different from, say, the car business. Even an old 
rundown car has some value. You can use it for making runs to the dump, or strip it for
parts. It is the fate of manufactured goods to slowly and gently depreciate as they get
old and have to compete against more modern products.

But it is the fate of operating systems to become free.
```

<a name="#Operating-systems-as-stack-of-metaphors"></a>
### Operating systems as stack of metaphors
([overview](#overview))

From Neal Stephenson's [In the beginning was the command line](http://cristal.inria.fr/~weis/info/commandline.html):

```markdown
When Ronald Reagan was a radio announcer, he used to call baseball games by reading
the terse descriptions that trickled in over the telegraph wire and were printed out
on a paper tape. He would sit there, all by himself in a padded room with a
microphone, and the paper tape would eke out of the machine and crawl over the palm
of his hand printed with cryptic abbreviations. If the count went to three and two, 
Reagan would describe the scene as he saw it in his mind's eye: "The brawny left-
hander steps out of the batter's box to wipe the sweat from his brow. The umpire 
steps forward to sweep the dirt from home plate." and so on. When the cryptogram on
the paper tape announced a base hit, he would whack the edge of the table with a 
pencil, creating a little sound effect, and describe the arc of the ball as if he 
could actually see it. His listeners, many of whom presumably thought that Reagan
was actually at the ballpark watching the game, would reconstruct the scene in their
minds according to his descriptions.

This is exactly how the World Wide Web works: the HTML files are the pithy description
on the paper tape, and your Web browser is Ronald Reagan. The same is true of Graphical
User Interfaces in general.

So an OS is a stack of metaphors and abstractions that stands between you and the 
telegrams, and embodying various tricks the programmer used to convert the information
you're working with--be it images, e-mail messages, movies, or word processing documents--
into the necklaces of bytes that are the only things computers know how to work with.
When we used actual telegraph equipment (teletypes) or their higher-tech substitutes
("glass teletypes," or the MS-DOS command line) to work with our computers, we were
very close to the bottom of that stack. When we use most modern operating systems,
though, our interaction with the machine is heavily mediated. Everything we do is 
interpreted and translated time and again as it works its way down through all of the
metaphors and abstractions.
```

<a name="#Selling-operating-systems-was-a-radical-idea"></a>
### Selling operating systems was a radical idea
([overview](#overview)) 

From Neal Stephenson's [In the beginning was the command line](http://cristal.inria.fr/~weis/info/commandline.html):

```markdown
About twenty years ago Jobs and Wozniak, the founders of Apple, came up with the very 
strange idea of selling information processing machines for use in the home. The
business took off, and its founders made a lot of money and received the credit they
deserved for being daring visionaries. But around the same time, Bill Gates and Paul
Allen came up with an idea even stranger and more fantastical: selling computer 
operating systems. This was much weirder than the idea of Jobs and Wozniak. A computer
at least had some sort of physical reality to it. It came in a box, you could open it
up and plug it in and watch lights blink. An operating system had no tangible 
incarnation at all. It arrived on a disk, of course, but the disk was, in effect,
nothing more than the box that the OS came in. The product itself was a very long 
string of ones and zeroes that, when properly installed and coddled, gave you the 
ability to manipulate other very long strings of ones and zeroes. Even those few who
actually understood what a computer operating system was were apt to think of it as a
fantastically arcane engineering prodigy, like a breeder reactor or a U-2 spy plane,
and not something that could ever be (in the parlance of high-tech) "productized."

Yet now the company that Gates and Allen founded is selling operating systems like
Gillette sells razor blades. New releases of operating systems are launched as if they
were Hollywood blockbusters, with celebrity endorsements, talk show appearances, and 
world tours. The market for them is vast enough that people worry about whether it has 
been monopolized by one company. Even the least technically-minded people in our society
now have at least a hazy idea of what operating systems do; what is more, they have 
strong opinions about their relative merits. It is commonly understood, even by
technically unsophisticated computer users, that if you have a piece of software that 
works on your Macintosh, and you move it over onto a Windows machine, it will not run. 
That this would, in fact, be a laughable and idiotic mistake, like nailing horseshoes
to the tires of a Buick.
```

<a name="#Complex-systems-and-systems-theory"></a>
## Complex systems and systems theory
([overview](#overview)) 

See also [Software complexity](#Software-complexity).

The Waterloo Institute for Complexity and Innovation has the following nice extensional suggestive-first-attempt definition from their [very nice webpage](https://uwaterloo.ca/complexity-innovation/about/what-are-complex-systems):

```markdown
Complex systems are all around us. They are seen in the ways that migrating birds organize
themselves into flocking formations and that ants communicate to successfully forage. 
They are seen in the ways in which humans form social networks, and in the patterns of 
communication, social capital, and reputation that emerge from these networks. They are
seen in the emergent power-law or fractal structures of plants, snowflakes, landslides,
and galaxies, as well as in similar structural patterns of wealth and income distribution,
stock market fluctuations, population distributions between cities, and patterns of urban 
development. Complex systems are often referred to as “wholes that are more than the sum 
of their parts,” wholes whose behaviour cannot be understood without looking at the 
individual components and how they interact.

Complex behaviour arises from the interplay, in densely interconnected systems, between
multiplicative causation and positive and negative feedbacks. A signature of such systems
is radically disproportional causation (i.e., small causes do not always produce small 
effects) or what is often called “nonlinearity.” Nonlinear systems can undergo sudden 
flips between stable states or equilibria. A second signature is the “emergence” of
structured macroscopic patterns that are the outcome of the independent microscopic 
interactions of the entities in the system. These macroscopic patterns — be they 
hurricanes in Earth’s atmosphere or boom-bust cycles in global financial markets — often 
have enormous causal power.

Complex *adaptive* systems — predominantly living systems, including human social systems
— exhibit all these features; but, in addition, they survive and reproduce within dynamic 
selection environments. To do so, they have sets of embedded rules that guide their action
in response to their external environments. These rules evolve under selection pressure.

Mathematically, complex adaptive systems are multi-state variable dynamical systems 
characterized by a moderate degree of structured interactions and interconnections. State 
variables in these systems are often characterized by heterogeneous parameter sets and 
updating rules. Spatial and network relationships are often non-uniform and violate mean 
field theory assumptions. As a result, mathematical representations of these systems often
do not have analytical solutions. Further, system behaviour is characterized by path 
dependence, nonlinearities, bifurcations, and threshold behaviour. Higher-scale or 
aggregate output patterns are often characterized by power-law statistical distributions.
```

Cosma Shalizi's [notebook on the topic](http://bactra.org/notebooks/complexity.html) has the following bit where he poses some natural-sounding questions we're still struggling with:

```markdown
A definition would be nice. So would an ordinal if not a cardinal measure. Is it clear
that humans are more complex than whales? Than chimpanzees? Than termites? Than termite
mounds?

Is there any trend towards greater complexity over time among living things? On the 
Earth as a whole? The universe as a whole? Is there any deep explanation (élan vital 
anyone?) or can it be accounted for by the usual suspects --- natural selection, "plenty
of room at the top," chance? --- Even if we do come up with a measure of complexity, it
will be very difficult to apply to the fossil record, since the soft parts are pretty 
well gone, and so we can't know (much) about the innards of the brain, or the immune 
system. (In fact, could you infer the existence of immune systems from the fossil record?
This is important, since it's complex if anything is, and if we can't infer it, how do we
know there weren't other things, also confined to the soft tissues, which weren't 
comprably complex?)

The "sciences of complexity" are very much a potpourri, and while the name has some 
justification --- chaotic motion seems more complicated than harmonic oscillation, for 
instance --- I think the fact that it is more dignified than "neat nonlinear nonsense" 
has not been the least reason for its success.
```

This particular notebook has *many* more outbound links to other notebooks in Cosma's repertoire than any other notebook I've found, which tells you a lot.

Wikipedia's [Complex systems](https://en.wikipedia.org/wiki/Complex_system#Overview) page has a surprisingly nice and gentle overview of the key concepts of complex systems:

- systems
- complexity
- networks
- nonlinearity
- emergence (including spontaneous order and self-organization)
- adaptation (special case)

as well as their salient features:

- cascading failures
- openness
- memoryful
- nestedness (Matrioshka dolls, not hierarchy)
- feedback loops

Compare with the key concepts in [systems theory](https://en.wikipedia.org/wiki/Systems_theory#General_systems_research_and_systems_inquiry), which feels a bit more [Borgesian](https://github.com/monastri/monastri.github.io/blob/master/poetry.md#the-celestial-emporium-of-benevolent-knowledge):

- System: An organized entity made up of interrelated and interdependent parts.
- Boundaries: Barriers that define a system and distinguish it from other systems in the environment.
- Homeostasis: The tendency of a system to be resilient towards external factors and maintain its key characteristics.
- Adaptation: The tendency of a self-adapting system to make the internal changes needed to protect itself and keep fulfilling its purpose.
- Reciprocal Transactions: Circular or cyclical interactions that systems engage in such that they influence one another.
- Feedback Loop: The process by which systems self-correct based on reactions from other systems in the environment.
- Throughput: Rate of energy transfer between the system and its environment during the time it is functioning.
- Microsystem: The system closest to the client.
- Mesosystem: Relationships among the systems in an environment.
- Exosystem: A relationship between two systems that has an indirect effect on a third system.
- Macrosystem: A larger system that influences clients, such as policies, administration of entitlement programs, and culture.
- Chronosystem: A system composed of significant life events that can affect adaptation.

A bit more on each -- I've curated and edited them for my own benefit.

Systems:

```markdown
A system, broadly defined, is a set of entities that, through their interactions, 
relationships, or dependencies, form a unified whole. It is always defined in terms
of its boundary, which determines the entities that are or are not part of the system.
Entities lying outside the system then become part of the system's environment.

A system can exhibit properties that produce behaviors which are distinct from the 
properties and behaviors of its parts; these system-wide or global properties and 
behaviors are characteristics of how the system interacts with or appears to its 
environment, or of how its parts behave (say, in response to external stimuli) by 
virtue of being within the system. The notion of behavior implies that the study of
systems is also concerned with processes that take place over time (or, in 
mathematics, some other phase space parameterization). 
```

Complexity and its variants:

```markdown
Systems exhibit complexity means that their behaviors cannot be easily implied from
the very properties that make them difficult to model, and the complex behaviors are
governed entirely, or almost entirely, by the behaviors those properties produce. 
Any modeling approach that ignores such difficulties or characterizes them as noise,
then, will necessarily produce models that are neither accurate nor useful. 

As yet no fully general theory of complex systems has emerged for addressing these
problems, so researchers must solve them in domain-specific contexts. Researchers in 
complex systems address these problems by viewing the chief task of modeling to be 
capturing, rather than reducing, the complexity of their respective systems of interest.

While no generally accepted exact definition of complexity exists yet, there are many 
archetypal examples of complexity. Systems can be complex if, for instance, 

- they have chaotic behavior (behavior that exhibits extreme sensitivity to initial 
conditions), 

- they have emergent properties (properties that are not apparent from their components
in isolation but which result from the relationships and dependencies they form when 
placed together in a system), 

- they are computationally intractable to model (if they depend on a number of 
parameters that grows too rapidly with respect to the size of the system)
```

Networks:

```markdown
The interacting components of a complex system form a network, which is a collection of
discrete objects and relationships between them, usually depicted as a graph of vertices 
connected by edges.

Networks often describe the sources of complexity in complex systems. Studying complex 
systems as networks therefore enables many useful applications of graph theory and 
network science. Some complex systems, for example, are also complex networks, which 
have properties such as phase transitions and power-law degree distributions that 
readily lend themselves to emergent or chaotic behavior. 

The fact that the number of edges in a complete graph grows quadratically in the number
of vertices sheds additional light on the source of complexity in large networks: as a
network grows, the number of relationships between entities quickly dwarfs the number 
of entities in the network.
```

Nonlinearity:

```markdown
Nonlinearity describes systems in which a change in the size of the input does not produce
a proportional change in the size of the output. For a given change in input, such systems
may yield significantly greater than or less than proportional changes in output, or even 
no output at all, depending on the current state of the system or its parameter values.

Of particular interest to complex systems are nonlinear dynamical systems, which are 
systems of differential equations that have one or more nonlinear terms. Some nonlinear
dynamical systems, such as the Lorenz system, can produce a mathematical phenomenon known
as chaos. Chaos as it applies to complex systems refers to the sensitive dependence on 
initial conditions, or "butterfly effect," that a complex system can exhibit. In such a 
system, small changes to initial conditions can lead to dramatically different outcomes.
Chaotic behavior can therefore be extremely hard to model numerically, because small 
rounding errors at an intermediate stage of computation can cause the model to generate
completely inaccurate output. 

Furthermore, if a complex system returns to a state similar to one it held previously, 
it may behave completely differently in response to exactly the same stimuli, so chaos 
also poses challenges for extrapolating from past experience.
```

Emergence:

```markdown
Emergent behaviors and properties are traits of a system which are not apparent from its
components in isolation but which result from the interactions, dependencies, or
relationships they form when placed together in a system.

While emergence is often used to refer only to the appearance of unplanned organized
behavior in a complex system, emergence can also refer to the breakdown of organization; 
it describes any phenomena which are difficult or even impossible to predict from the 
smaller entities that make up the system.

One example of complex system whose emergent properties have been studied extensively is
cellular automata. In a cellular automaton, a grid of cells, each having one of finitely
many states, evolves over time according to a simple set of rules. These rules guide the
"interactions" of each cell with its neighbors. Although the rules are only defined 
locally, they have been shown capable of producing globally interesting behavior, for
example in Conway's Game of Life.

When emergence describes the appearance of unplanned order, it is spontaneous order (in 
the social sciences) or self-organization (in physical sciences). 

Spontaneous order can be seen in herd behavior, whereby a group of individuals coordinates
their actions without centralized planning. 

Self-organization can be seen in the global symmetry of certain crystals, for instance the
apparent radial symmetry of snowflakes, which arises from purely local attractive and 
repulsive forces both between water molecules and between water molecules and their
surrounding environment.
```

Adaptation:

```markdown
Complex adaptive systems are special cases of complex systems that are adaptive in that 
they have the capacity to change and learn from experience. 

Examples of complex adaptive systems include the stock market, social insect and ant 
colonies, the biosphere and the ecosystem, the brain and the immune system, the cell and 
the developing embryo, the cities, manufacturing businesses and any human social group-
based endeavor in a cultural and social system such as political parties or communities.
```

<a name="#How-complex-systems-fail"></a>
### How complex systems fail
([overview](#overview)) 

This is mostly from Richard Cook's excellent short treatise/summary overview [How Complex Systems Fail](https://web.mit.edu/2.75/resources/random/How%20Complex%20Systems%20Fail.pdf). Read the paper for the full version; I'm quoting only the parts that spoke to me. 

Complex systems are intrinsically hazardous systems:

```markdown
All of the interesting systems (e.g. transportation, healthcare, power generation) are
inherently and unavoidably hazardous by the own nature. The frequency of hazard
exposure can sometimes be changed but the processes involved in the system are
themselves intrinsically and irreducibly hazardous. It is the presence of these hazards
that drives the creation of defenses against hazard that characterize these systems.
```

Complex systems are heavily and successfully defended against failure:

```markdown
The high consequences of failure lead over time to the construction of multiple layers of
defense against failure. These defenses include obvious technical components (e.g.
backup systems, ‘safety’ features of equipment) and human components (e.g. training,
knowledge) but also a variety of organizational, institutional, and regulatory defenses
(e.g. policies and procedures, certification, work rules, team training). The effect of these
measures is to provide a series of shields that normally divert operations away from
accidents.
```

Catastrophe requires multiple failures – single point failures are not enough:

```markdown
The array of defenses works. System operations are generally successful. Overt
catastrophic failure occurs when small, apparently innocuous failures join to create
opportunity for a systemic accident. Each of these small failures is necessary to cause
catastrophe but only the combination is sufficient to permit failure. Put another way,
there are many more failure opportunities than overt system accidents. Most initial
failure trajectories are blocked by designed system safety components. Trajectories that
reach the operational level are mostly blocked, usually by practitioners.
```

Complex systems contain changing mixtures of failures latent within them, so they run in degraded mode:

```markdown
The complexity of these systems makes it impossible for them to run without multiple
flaws being present. Because these are individually insufficient to cause failure they are
regarded as minor factors during operations. Eradication of all latent failures is limited
primarily by economic cost but also because it is difficult before the fact to see how such
failures might contribute to an accident. The failures change constantly because of
changing technology, work organization, and efforts to eradicate failures.

A corollary to the preceding point is that complex systems run as broken systems. The
system continues to function because it contains so many redundancies and because
people can make it function, despite the presence of many flaws. After accident reviews
nearly always note that the system has a history of prior ‘proto-accidents’ that nearly
generated catastrophe. Arguments that these degraded conditions should have been
recognized before the overt accident are usually predicated on naïve notions of system
performance. System operations are dynamic, with components (organizational, human,
technical) failing and being replaced continuously. 
```

Because of this, catastrophe is always just around the corner:

```markdown
Complex systems possess potential for catastrophic failure. Human practitioners are
nearly always in close physical and temporal proximity to these potential failures –
disaster can occur at any time and in nearly any place. The potential for catastrophic
outcome is a hallmark of complex systems. It is impossible to eliminate the potential for
such catastrophic failure; the potential for such failure is always present by the system’s
own nature. 
```

Post-accident attribution accident to a ‘root cause’ is fundamentally wrong:

```markdown
Because overt failure requires multiple faults, there is no isolated ‘cause’ of an accident.
There are multiple contributors to accidents. Each of these is necessary insufficient in
itself to create an accident. Only jointly are these causes sufficient to create an accident.
Indeed, it is the linking of these causes together that creates the circumstances required
for the accident. Thus, no isolation of the ‘root cause’ of an accident is possible. The
evaluations based on such reasoning as ‘root cause’ do not reflect a technical
understanding of the nature of failure but rather the social, cultural need to blame
specific, localized forces or events for outcomes.
```

Hindsight biases post-accident assessments of human performance:

```markdown
Knowledge of the outcome makes it seem that events leading to the outcome should have
appeared more salient to practitioners at the time than was actually the case. This means
that ex post facto accident analysis of human performance is inaccurate. The outcome
knowledge poisons the ability of after-accident observers to recreate the view of
practitioners before the accident of those same factors. It seems that practitioners “should
have known” that the factors would “inevitably” lead to an accident. Hindsight bias
remains the primary obstacle to accident investigation, especially when expert human performance
is involved.
```

All practitioner actions are gambles:

```markdown
After accidents, the overt failure often appears to have been inevitable and the
practitioner’s actions as blunders or deliberate willful disregard of certain impending
failure. But all practitioner actions are actually gambles, that is, acts that take place in the
face of uncertain outcomes. The degree of uncertainty may change from moment to
moment. That practitioner actions are gambles appears clear after accidents; in general, 
post hoc analysis regards these gambles as poor ones. But the converse: that successful
outcomes are also the result of gambles; is not widely appreciated. 
```

This one is pretty personal to me --  human expertise in complex systems is constantly changing:

```markdown
Complex systems require substantial human expertise in their operation and
management. This expertise changes in character as technology changes but it also
changes because of the need to replace experts who leave. In every case, training and
refinement of skill and expertise is one part of the function of the system itself. At any
moment, therefore, a given complex system will contain practitioners and trainees with
varying degrees of expertise. Critical issues related to expertise arise from (1) the need to
use scarce expertise as a resource for the most difficult or demanding production needs
and (2) the need to develop expertise for future use.
```

Safety is a characteristic of systems and not of their components:

```markdown
Safety is an emergent property of systems; it does not reside in a person, device or
department of an organization or system. Safety cannot be purchased or manufactured; it
is not a feature that is separate from the other components of the system. This means that
safety cannot be manipulated like a feedstock or raw material. The state of safety in any
system is always dynamic; continuous systemic change insures that hazard and its
management are constantly changing.
```

People continuously create safety:

```markdown
Failure free operations are the result of activities of people who work to keep the system
within the boundaries of tolerable performance. These activities are, for the most part,
part of normal operations and superficially straightforward. But because system
operations are never trouble free, human practitioner adaptations to changing conditions
actually create safety from moment to moment. These adaptations often amount to just
the selection of a well-rehearsed routine from a store of available responses; sometimes,
however, the adaptations are novel combinations or de novo creations of new approaches.
```

<a name="#practical-magic"></a>
## Practical magic
([overview](#overview))

From Steve Yegge's post [Practical magic](https://sites.google.com/site/steveyegge2/practical-magic):

```markdown
I wrestle with the whole abstraction question, and I'm still not sure where a good engineer these
days should draw the line — the one below which it's all just magic.

We all have that line somewhere; I encountered mine in school, back in my semiconductors course. 
We were (ostensibly) learning how semiconductors work, but it was perfectly clear to me that this
was just magic, and I was never going to understand it — in part, because I didn't want to make 
what was clearly going to be a HUGE effort to get it. There was all this crap about K-spaces and 
lattices and who knows what else. Maybe they'd listed the prerequisites wrong, but I did not have
the math foundations to understand what was going on. ...

It took me an extra year, but I finished in CS instead of CE, which allowed me to conveniently 
pretend that computer hardware, starting somewhere down at the level of the doping barrier in a 
silicon semiconductor, is just pure magic. Parts of the hardware above that level are still a little
murky, but I have a pretty good idea how computers can be made by assembling successively larger 
components together from smaller ones. Given time and a gun to my head, I could probably start with
any set of smaller components and derive how to build higher-level abstractions: transistors into 
logic gates, logic gates into larger assemblies that do arithmetic and boolean computing, those into 
state machines and ALUs, and so on. I'd suck at it, but I get the general idea, so it's not really 
"magic".

It's magic when you have absolutely no frigging clue how it works, not the first clue. It just works. 
That's how it is for me and semiconductors.
```

Steve says he's okay with that:

```markdown
I'm OK with treating semiconductors as "atoms" (or axioms, anyway) in our little programming universe
. Chips are like molecules, CPUs are compounds, and Von Neumann machines can be bricks and mortar.
Well, I'm sure you could come up with a way better metaphor. Whatever.

The point is, the computers and networks and power supplies and so on are all amazingly complex under
the hood, but usually I can just pretend they work a certain way, and not worry about how, any more
than I have to worry about my Amazing Eye in order to pour myself another glass of fine wine, which
I will doubtless use to polish my keyboard if I don't finish this blog entry soon.
```

What he's not sure about is when magic itself is okay to a developer:

```markdown
I don't know. I'd really LIKE to know. I'm constantly trying to find better abstractions for my 
everyday work as a programmer. You can't build large systems without having some fairly bulletproof 
abstractions to build on. If you're building an e-commerce system, for instance, you need a 
transactional data store, and you rely on the semantics of transactionality when you're coding; if 
you don't, you'll wind up with all this crap in your code that tries to fake transactions.

I'm comfortable relying on certain abstractions working for me — for instance, if I compile with
optimizations turned on, I know the compiler won't discard correctness in favor of performance, or 
if it does do that, it'll be documented so I know I shouldn't use that flag. Compiler optimization 
can be treated like a black box of sorts: I turn it on and see if performance seems any better, but
I don't expect to need to re-test all my loops to make sure the variables are all still being adjusted 
in the same order as before.

What I'm NOT sure about is where I'm allowed to forget how things work, or never know in the first 
place, and start getting by with incantations that seem to work.

For instance, I know that I can type 'ls' in a shell to get a directory listing. How much do I have
to really know about how unix 'ls' works in order to be an effective developer? 
```

He sees two arguments for this (actually three) — "so cleanly divided in opinion, in fact, that I can picture which of my friends are marching directly into one camp or the other right now":

```markdown
One argument is that you DO need to know a lot about how 'ls' works, because there are all sorts of
situations in which it can fail, and you'll need to figure out how to fix it. It could simply not 
show up ("command not found", say), or it could stop working on certain of my directories, or it could
crash every once in a while instead of producing a directory listing, or it could go on a rampage and 
start deleting files. I think I've seen all of these happen with 'ls' in my time, even the last one,
when my linux filesystem was corrupted.

Another argument is that you DO NOT need to know much about how 'ls' works. Probably all you need to
know is that it's a unix command-line tool, a binary that was compiled for your OS, probably written 
in C, that it lives in a standard place in the filesystem, and that standard binary locations are 
looked up in an environment variable called PATH. But you don't need to know how it traverses the 
filesystem inode entries, or whether it's a statically or dynamically linked version of 'ls', or
whatever else there is to know about 'ls'.

The second camp argues that software development is a community effort, and your community should have
a Unix Guy Or Gal who knows all the ins and outs of how lses and diffs and their ilk work. A sort of 
tribal shaman who you go to, and desperately plead with: please help me! There's a bug in qsort! The 
shaman frowns at your screen, and pokes and prods things a bit, and announces that your pilfer grommit
is no longer connected to your weasel pins, and that the easiest fix is to reinstall the OS.

A third, possibly even more abstract camp, would argue that 'ls' is way too complicated, and that you
should be developing on systems in which everything is managed by navigating menus and waiting for your
Auto Updater to tell you that a new Service Pak is available for download. And for all I know, they 
might be right. I have no idea how Exchange works, for example, and yet I trust it with my email every
day. When it's broken, I put in Stupid Remedy Tickets saying I haven't received email in 10 days, and
I don't feel the least bad about that, since it's not my responsibility; I made all the right incantations,
and spilled all the right wine, and by golly, I'm not getting email anymore.

The second and third camps want to use J2EE, and they recount with some pride how they've managed just
fine for years without ever having had to learn a scripting language, or become proficient with some
cryptic unix editor, or any of that arcane crapola. They didn't see any need, because they were off
building the FrooSingletonManager service, and it's all finished now, while I'm still mucking around
with my broken 'ls' command.

Moreover, many of them say they don't see any need to know how to implement an n log(n) sorting algorithm,
because the damn things are already provided in libraries for every platform in the universe, including 
programming languages that are deader than Latin or Sanskrit.

And you know, I wonder sometimes whether they're right.
```

Steve straddles both camps:

```markdown
One the one hand, I think nobody in their right mind would try to write a gigantic system in C++ now that
Java has become an obviously far superior way to build large systems. You can argue that in C++ you really 
have to know what you're doing, or that you love the smell of freshly-brewn pointer arithmetic in the early
morning, or whatever the hell you like about C++. I'm not arguing that you LIKE it — I know you do. I liked
assembly language when I was using it daily. I'm just saying that the game has moved on, and if you're using
C++ to build large systems because you like C++, it's like competing in the Indy 500 with your 1980 5.8-liter
Pontiac Firebird. It gets you around, and it's fun to tinker with, which is good 'cause it breaks down all the
time, but you're not going to win any world championships with it.

On the OTHER hand (remember, we were just on the one back there), I think nobody in their right mind would 
write a huge system in Java without first knowing how the whole thing is implemented, under the covers, in C++
and (below that) assembly language. As of today, anyway, I don't believe the JVM is allowed to be on the "it's
magic" side of the line. And as for J2EE, which provides so much abstraction that you can snap together an 
enterprise architecture with it after one or two introductory programming courses, it's WAY too much magic. 
I definitely think that (as of today) if your Magic Line stops at the J2EE framework APIs and the Java 
Programming Language, then you're a wuss.
```

But these two views are mutually inconsistent! Steve:

```markdown
1. using abstraction makes you MORE effective, because to build large, interesting things in any 
reasonable amount of time, you need to work with high-level abstractions and be able to assume that
they work as advertised.

This part of me believes that someday we'll be programming in purely declarative languages, telling the
computer what to do, and letting it figure out how.

2. relying too much on abstraction makes you LESS effective, because you're unable to cope when your 
framework isn't working right, or when you're trying to do something with it that it wasn't designed
for, or whatever.

This part of me believes that my other belief is on crack if it thinks it'll happen during my lifetime.
```

Honestly I feel #2 very keenly with Python. It's so ridiculously high-level that stuff is either trivial to do in it or nigh-impossible and requires magic incantations.

Steve's current compromise is "know thy abstractions":

```markdown
1. you know more or less how it works; i.e. what other abstractions it's built on top of, and approximately
how it was built.

2. you know where the abstraction leaks: i.e. what the gotchas are, failure modes, what the most common
incantations are to get it working again.

3. You need at least SOME level of tv-repairman ability for the things you use — you should be able to 
install any of the software you rely on, for instance. Or you should have a plausible backup plan handy 
if you need to throw this abstraction away and use another one.

4. you need to be able to reason about the performance characteristics of the abstraction, and understand
how its performance and reliability degrade as you put pressure on it.

5. you know where to look, or who to ask, if it doesn't seem to be working.
```

<a name="#yegges-conservative-liberal-axis"></a>
## Yegge's conservative-liberal axis
([overview](#overview))

Steve Yegge's post/rant/essay [Notes from the Mystery Machine Bus](https://plus.google.com/110981030061712822816/posts/KaSKeg4vQtz) begins, after a meandering half-drunken introduction, with the following theses:

```markdown
I've spent the past eight years (starting back in June 2004) writing elaborate rants about a bunch
of vaguely related software engineering issues. I was doing all that ranting because I've been 
genuinely perplexed by a set of "bizarre" world-views held dear by -- as far as I can tell -- about
half of all programmers I encounter, whether online or in person.

Last week, after nearly a decade of hurling myself against this problem, I've finally figured it out.
I know exactly what's been bothering me. Here is the thesis of this looooong essay. It is the root
cause that motivated over half of my ranting all these years, starting at Amazon and continuing here 
at Google.

1) Software engineering has its own political axis, ranging from conservative to liberal.

2) The notions of "conservative" and "liberal" on this political axis are specialized to software 
engineering. But they exhibit some strong similarities to their counterparts in real-world politics.

3) Everyone in the software industry who does stuff related to programming computers falls somewhere
fairly precise on this political spectrum, whether they realize it or not.

Just as in real-world politics, software conservatism and liberalism are radically different world
views. Make no mistake: they are at odds. They have opposing value systems, priorities, core beliefs 
and motivations. These value systems clash at design time, at implementation time, at diagnostic time,
at recovery time. They get along like green eggs and ham.
```

What's so important about recognizing this distinction?

```markdown
It probably won't help us agree on anything, pretty much by definition. Any particular issue only 
makes it onto the political axis if there is a fundamental, irreconcilable difference of opinion about
it. Programmers probably won't -- or maybe even can't -- change their core value systems.

But the political-axis framework gives us a familiar set of ideas and terms for identifying areas of 
fundamental disagreement. This can lead to faster problem resolution. Being able to identify something
quickly as a well-defined political issue means we can stop wasting time trying to convince the other
side to change their minds, and instead move directly into the resolution phase, which (just as in 
politics) generally boils down to negotiation and compromise. Or, you know, Watergate.

Or at the very least, the conservative/liberal classification should help the two camps steer clear of
each other. I think it is probably better to have a harmonious team of all-liberals or all-conservatives
than a mixed team of constantly clashing ideologies. It's a lot like how vehicle-driving philosophies 
can differ regionally -- it's OK if everyone drives in some crazy way, as long as they ALL drive that way.
```

I'm honestly not that interested in the minutiae of Real Politics (TM) (even though "politics is interested in You! Yes, YOU!!"), so I'll go straight to the quotes that caught my fancy. 

What's a "software liberal/conservative"?

```markdown
It's easiest to talk first about conservatives, and then define liberals in terms of what conservatives 
are not. This is because conservatives tend to have a unified and easily-articulated value system, whereas 
liberals tend to be more weakly organized and band together mostly as a reaction to conservatism. ...

Conservatism, at its heart, is really about risk management. ...

Liberalism doesn't lend itself quite as conveniently to a primary root motivation. But for our purposes
we can think of it as a belief system that is motivated by the desire above all else to effect change. 
In corporate terms, as we observed, it's about changing the world. In software terms, liberalism aims 
to maximize the speed of feature development, while simultaneously maximizing the flexibility of the 
systems being built, so that feature development never needs to slow down or be compromised.

To be sure, conservatives think that's what they're maximizing too. But their approach is... well, 
conservative. Flexibility and productivity are still motivators, but they are not the primary motivators.
Safety always trumps other considerations, and performance also tends to rank very highly in the software-
conservative's value system.

The crux of the disagreement between liberals and conservatives in the software world is this: how much
focus should you put on safety? Not just compile-time type-safety, but also broader kinds of "idiot-
proofing" for systems spanning more than one machine.
```

How they view each other is the same as in real-world politics:

```markdown
Software liberals are viewed by conservatives as slovenly, undisciplined, naive, unprincipled, downright
"bad" engineers. And liberals view conservatives as paranoid, fearmongering, self-defeating bureaucrats.
```

Conservatives would rate these example statements much higher-importance than liberals:

```markdown
1. Software should aim to be bug free before it launches. (Banner claim: "Debugging Sucks!") Make sure
your types and interfaces are all modeled, your tests are all written, and your system is fully
specified before you launch. Or else be prepared for the worst!

2. Programmers should be protected from errors. Many language features are inherently error-prone and 
dangerous, and should be disallowed for all the code we write. We can get by without these features, 
and our code will be that much safer.

3. Programmers have difficulty learning new syntax. We should limit the number of languages used at our
company, so that nobody has to learn a new syntax when a system goes down in the middle of the night 
on Christmas Eve. And we should never permit features that allow defining new syntax, nor changing the
semantics of existing syntax. (Common examples: no operator overloading, and NO metaprogramming!)

4. Production code must be safety-checked by a compiler. Any code that cannot be statically checked 
should in general be avoided. In specific cases where it is strictly necessary, uses of it must be 
approved by a central committee. (Examples: eval, dynamic invocation, RTTI).

5. Data stores must adhere to a well-defined, published schema. Relational databases must be in third-
normal form and adhere to a UML or equivalent schema definition. XML should have a DTD. NoSQL databases
and name/value stores -- both of which should be avoided in general -- must have a separate physical 
schema that defines all permissible keys and their corresponding value types.
 
6. Public interfaces should be rigorously modeled. Data should never be stored in strings or untyped 
collections. All input and output entities should be thorougly and explicitly specified via statically-
checkable, ideally object-oriented models.

7. Production systems should never have dangerous or risky back-doors. It should never be possible to
connect to a live production system via a debugger, telnet shell, nor any other interface that allows
the developer to manipulate the runtime operation of the code or data. The only ports into a production
system should be read-only monitoring channels.

8. If there is ANY doubt as to the safety of a component, it cannot be allowed in production -- no 
matter how teams may cry and wail that they need it to make forward progress. (I'm talkin' to you, FUSE).

9. Fast is better than slow. Everyone hates slow code. Code should perform well. You should engineer 
all your code for optimum speed up front, right out of the box. Otherwise it might not be fast enough. 
Avoid using languages or DSLs or libraries that have a reputation for being slow.  Even if they're 
fast enough for your current purposes, the requirements (or callers) could change, and suddenly the
software would be too slow!
```

Liberals would instead agree more with the following example statements:

```markdown
1. Bugs are not a big deal. They happen anyway, no matter how hard you try to prevent them, and somehow
life goes on. Good debuggers are awesome pieces of technology, and stepping through your code gives you 
insights you can't get any other way. Debugging and diagnosing are difficult arts, and every programmer
should be competent with them. The Christmas Eve Outage scenario never, ever happens in practice --
that's what code freeze is for. Bugs are not a big deal! (This belief really may be the key dividing
philosophy between Conservative and Liberal philosophies.)

2. Programmers are only newbies for a little while. The steady state for a programmer's career is being
smart, knowledgeable, creative, resourceful and experienced. Putting a bunch of rules in place to
protect newbies from doing harm (or being harmed) is incorrectly optimizing for the transient case
instead of the steady state.

3. Programmers figure stuff out amazingly fast when their jobs depend on it. People learn to read sheet
music, braille, sign language, and all sorts of other semiotic frameworks. Hell, even gorillas can 
apparently do all that. Programmers don't need protection from syntax. They just need documentation and 
a little slack time to read up on it.

4. Succinctness is power. Code should be kept small. Period. If your static checking tools can't reason 
about the code, then the checking needs to be made smarter (e.g. by incorporating runtime data) rather
than making the code dumber.

5. Rigid schemas limit flexibility and slow down development. Lightweight/partial/optional schemas are a 
better tradeoff. Moreover, the schema is often not well-understood until a lot of data is collected and a
lot of use cases are thorougly exercised. So the schema should follow the code rather than precede it.

6. Public interfaces should above all else be simple, backward-compatible, and future-compatible. Rigorous
modeling is just guessing at how the interface will need to evolve. It makes both forward- and backward-
compatibility almost impossible, resulting in interface churn and customer unhappiness. Public interfaces 
should always do the simplest thing that could possibly work, and grow only as needed.

7. System flexibility can mean the difference between you getting the customer (or contract) vs. your 
competitor nabbing it instead. Security and safety risks in runtime production systems can be mitigated 
and controlled by logging, monitoring and auditing. There are plenty of existence-proofs of large systems 
with root-access backdoors and shells (e.g. RDBMS, online game servers) whose risk is controlled while 
still giving them world-class runtime flexibility.

8. Companies should take risks, embrace progress, and fiercely resist ossification. It doesn't matter how
big your business is: it must grow or die. If you want to stay competitive, you have to make a conscious,
often painful effort to take risks. Which means you'll need good recovery techniques for the inevitable
disasters. But you need those even if you don't take risks.  So take risks!

9. Premature optimization is the root of all evil. Get the code working first, focusing on correctness
over performance, and on iterative prototyping over correctness. Only when your customers list latency 
as the top priority should you begin performing profiler-driven optimizations.
```

Here Steve tosses "a bunch of random technologies, patterns, designs and disciplines each into one of six buckets: "apolitical", "conservative", "centrist", "liberal" buckets, plus two buckets that start Centrist and head Left or Right in the presence of overuse":

```markdown
*Non-political Stuff*: Algorithms, data structures, concrete mathematics, complexity analysis, 
information theory, type theory, computation theory, and so on. Basically all CS theory. These 
disciplines occasionally inspire tempest-in-a-teapot butthurtedness in academia, but when it
happens, it's just similar fish in too small a tank biting on each other. It's to be expected.
Overall, these essentially mathematical disciplines are timeless, and they are all equally 
applicable to both the Liberal and Conservative programming worlds.  Yes, even type theory.

*Conservative Stuff*: Provably sound type systems. Mandatory static type annotations. Nonpublic
symbol visibility modifiers (private/protected/friend/etc.). Strict, comprehensive schemas. all-
warnings-are-errors. Generics and templates. Avoidance of DSLs (XPath, regexps) in favor of 
explicit DOM manipulation and hand-rolled state machines.  Build dependency restrictions.  Forced
API deprecation and retirement.  No type equivalence (i.e. no automatic conversions) for numeric
types.  Checked exceptions.  Single-pass compilers.  Software Transactional Memory.  Type-based
function overloading.  Explicit configuration in preference to convention. Pure-functional data
structures.  Any kind of programming with the word "Calculus" in it.

*Centrist (or flat-out Neutral) Stuff*: Unit testing. Documentation. Lambdas. Threads. Actors.
Callbacks.  Exceptions.  Continuations and CPS.  Byte-compilation.  Just-in-time compilation. 
Expression-only languages (no statements).  Multimethods. Declarative data structures.  Literal
syntax for data structures.  Type dispatch.

*Liberal Stuff*: Eval. Metaprogramming. Dynamic scoping. all-errors-are-warnings. Reflection and 
dynamic invocation. RTTI. The C preprocessor. Lisp macros. Domain-specific languages (for the most
part). Optional parameters. Extensible syntax. Downcasting.  Auto-casting.  reinterpret_cast.  
Automatic stringification.  Automatic type conversions across dissimilar types.  Nil/null as an
overloaded semantic value (empty list, empty string, value-not-present).  Debuggers.  Bit fields.
Implicit conversion operators (e.g. Scala's implicits).  Sixty-pass compilers.  Whole-namespace 
imports.  Thread-local variables.  Value dispatch.  Arity-based function overloading.  Mixed-
type collections.  API compatibility modes.  Advice and AOP.  Convention in preference to
explicit configuration.

*Centrist Stuff that Becomes Conservative If Taken Far Enough*: Type modeling. Relational modeling. 
Object modeling. Interface modeling. Functional (i.e., side-effect-free) programming.

*Centrist Stuff that Becomes Liberal if Taken Far Enough*: Dynamic class loading and dynamic code 
loading. Virtual method dispatch. Buffer-oriented programming.
```

Natural themes arise:

```markdown
 -- implicit is generally liberal; explicit is generally conservative.

 -- performance-oriented is generally conservative; late-optimized is generally liberal.

 -- compile-time binding is generally conservative; runtime/late binding is generally liberal.

 -- concurrency and parallelism in general seem to be politically charged topics, but the 
 disagreement is orthogonal to the liberal/conservative camps.
```

Programming languages:

```markdown
Here are some very rough categorizations. Note that within each language camp there are typically 
liberal and conservative sub-camps. But as a whole, language usage tends to be dominated by what 
the language makes possible (and easy), so the culture tends to follow the features.

This list is just a few representative examples to give you the flavor. I'm only listing general-
purpose languages here, since DSLs and query languages are typically feature-restricted enough to
be hard to categorize.

Assembly language: Batshit liberal.

Perl, Ruby, PHP, shell-script: Extremist liberal.

JavaScript, Visual Basic, Lua: Hardcore liberal.

Python, Common Lisp, Smalltalk/Squeak: Liberal.

C, Objective-C, Scheme: Moderate-liberal.

C++, Java, C#, D, Go: Moderate-conservative.

Clojure, Erlang, Pascal: Conservative.

Scala, Ada, OCaml, Eiffel: Hardcore conservative.

Haskell, SML: Extremist conservative.

One thing that jumps out is that a language doesn't have to be statically-typed or even strongly-
typed in order to be conservative overall. More on that in a bit.

The next thing you might notice from the list is that the liberal and moderate languages are all 
pretty popular, and that popularity declines sharply as languages head into conservative territory.

I think this has a simple explanation: It's possible to write in a liberal language with a conservative 
accent, but it's very hard (and worse, discouraged) to write in a conservative language with a liberal
accent.

For instance, it's straightforward to write JavaScript code in a way that eschews reflection, eval, 
most automatic type casting, prototype inheritance, and other dynamic features. You can write
JavaScript that plods along as unadventurously as, say, Pascal. It doesn't have all the static 
type annotations, but you can replace them with assertions and unit tests and stereotypically 
stolid code organization.

But if you try writing your Haskell code with a bunch of dynamic features, well, you're in for a 
LOT of work. Haskell enthusiasts have managed to implement dynamic code loading and a ton of other
ostensibly dynamic features, but it was only through herculean effort.

What's more, if you write your liberal-language code in a conservative way, people will just look
at it and say: "Well, it's kinda boring, and you could have saved a lot of coding by using some 
dynamic features. But I guess it gets the job done. LGTM."

Whereas if you write your conservative-language code in a liberal way, you run the risk of being 
ostracized by your local language community, because... why are you doing all that dangerous
dynamic stuff in the first place? I'll explore this cultural phenomenon further when I talk about 
Clojure below.

The last big, interesting observation from the list is that a lot of the most popular languages out
there are only moderately conservative -- even if they think of themselves as quite conservative 
compared to their ultra-dynamic cousins.

I've said it before, and it bears repeating here: the reason C++, C# and Java have been particularly
successful in the marketplace is that -- just like effective politicians -- they know how to play
both sides.

C++ allows liberal-biased programmers to program in straight C, and it allows conservative-biased
programmers to layer in arbitrary amounts of static type modeling, depending on how much work they
want to expend in order to feel secure. Java?  Pretty much the same story.

Playing to both the fast-and-loose and lock-your-doors mindsets has proven to be a key ingredient
to market success.  Also marketing, but it helps a LOT to be viewed as philosophically friendly by
both the liberal and conservative camps.

There is a new crop of languages on the horizon (for instance, Google's Dart language, but also new
specs for EcmaScript) that are deliberately courting the centrist crowd -- and also delicately 
playing to grab both the liberals and conservatives -- by offering optional static types. In principle
this is a sound idea. In practice I think it will come down to whether the marketing is any good. 
Which it probably won't be.

Language designers always seem to underestimate the importance of marketing!
```

Tech corporations:

```markdown
1) Facebook -- Diagnosis: Extremist Liberal. Despite their scale, they are still acting like a 
startup, and so far they've been getting away with it. They use primarily C++ and PHP, and they're 
prone to bragging about how their code calls back and forth from PHP to C++ and back into PHP, 
presumably bottoming out somewhere. Their datastore is memcached: just name-value pairs.  No schema.
They dump the data and logs into a backend Hive store and run Hadoop mapreduces for offline data
analysis.  They still hold all-night hackathons every other week or so, which will remain feasible
for them as long as the majority of their programmers are very young males (as was the case last 
time I toured there) and their stock continues to promise great riches (as was not so much the case
last I checked.)  As a company they are tightly knit and strongly biased for action, placing a high
value on the ability of individual programmers to launch features to their website with little to no 
bureaucracy or overhead.  This is pretty remarkable for a company as big as they are, with as many 
users as they have.  Conservatives no doubt regard them with something between horror and contempt.
But Facebook is proving that programmers of any world-view can get a hell of a lot accomplished when 
they gang up on a problem.

2) Amazon.com -- Diagnosis: Liberal. Which is surprising, given how long they've been in business,
how much money is at stake, how mature their Operations division is, and how financially conservative
they are. But "Liberal" is actually quite a retreat compared to their early days. Back in 1998-1999 
they were almost exactly like Facebook is today, with the sole exception that they put everything in
relational databases and did a ton of up-front relational data modeling.  Well, except in Customer 
Service Apps, where we used a name/value store just to be flexible enough to keep up with the mad 
chaotic scramble of the business launches.  All part of my multi-decade indoctrination as a Liberal. 
In any case, despite many corporate improvements with respect to work-life balance (which happened 
after several stock plunges and years of significant double-digit turnover in engineering), Amazon has
retained its liberal, startup-like engineering core values.  Every team owns their own data and makes 
their own decisions, more or less like independent business units.  Amazon still launches and executes 
faster than just about anyone else out there, because they're still willing to take real risks
(incurring occasional huge outages), and to make hard decisions in favor of launching early and often.
Above all else, Amazon has proven conclusively that after fifteen years, they can still innovate like
nobody else.  They've still got it.

3) Google -- Diagnosis: Conservative. They began life as slightly liberal and have grown more 
conservative ever since. Google was only software-liberal in the very very early days, back when the 
search engine itself was written in Python. As they grew, they quickly acquired a software conservatism
driven entirely by the engineers themselves.  Manifestos were written about the dangers of using multiple 
languages, and strict style guides were put in place to severely limit "risky" or "hard to read" language 
features of the few languages they did allow.  Google's JavaScript code is written in an extremely 
conservative style with extensive static type annotations, and eval is forbidden.  The Python style guide 
forbids metaprogramming and other dynamic features, which makes their Python look a lot like untyped Java.
And they have severely limited the use of many C++ language features, with C++11 support rolling out 
literally one feature every few weeks.  (There are over five hundred new features in C++11.)  In internal
surveys, Google engineers commonly cite bureaucracy, churn and complexity as core obstacles to feature 
advancement and rapid launches.  Google has made serious attempts on several occasions to reduce this
bureacracy, but they always get pushback from -- surprise -- the engineers themselves, who have grown so 
staunchly conservative that they actively (and even more often, passively) resist the introduction of more
flexible stacks and technologies.  Most of the major technological shifts within Google over the past half-
decade have been overtly conservative.  For a liberal like me, it has been a very sad process to observe.
But at least I've found myself a niche that's widely regarded (by both camps) as valuable, and within my
own org we can still be pretty liberal and get away with it.

4) Microsoft -- Diagnosis: Batshit Conservative. Microsoft has two geese that lay golden eggs: Office and 
Windows. Microsoft has been reduced to a commercial farmer protecting the geese from all incursions.  The
golden eggs still have value, because customers are locked into the platform by the cost-ineffectiveness
of retraining their fleets.  But Microsoft can no longer innovate in Office or Windows precisely because
of those corporate fleet retraining costs.  Their OEMs are stretched as thin as they can go.  Apple is 
dominating the handheld markets, and Microsoft is actively stifling their own innovation in Windows Phone
because they're afraid it will cannibalize their core Windows business.  Microsoft has not had a 
successful product-level innovation in fifteen, maybe twenty years.  All of their successful products 
have been copies of competitors' products:  IE, XBox, C#, .NET, Bing, Windows Phone, and so on ad
infinitum. All great implementations of someone else's ideas. Microsoft's playbook is to embrace, extend,
and leverage their brand to crush the competition -- or at least it was, until the goverment put an end 
to that circa 2002.  Now the company genuinely doesn't know what the fuck to do with themselves, and
what's more, instead of Bill Gates they now have a lunatic in charge.  Employees are leaving in droves, 
all citing the same internal "existential crisis" and unbearable corporate politics caused by competing
business units actively sabotaging one another.  Microsoft has turned into a caricature of right-wing
corporatism: sitting on their front porch with a shotgun cursing at passers-by, waiting for their 
government bribes to give them another few years of subsidies and shelters while they wait to die. 
I've personally chatted with close to four hundred current and ex-Microsoft employees over the past seven
years.  Oh, the stories I could tell you... someday, maybe.

5) Bonus company: Apple. Diagnosis: no idea, but they're so good at marketing that it's almost
irrelevant. Would love to have more insight into their internal software culture, though.  Any takers? 
Throwaway accounts?  AMA?
```

<a name="#Amazon-vs-Google-2011"></a>
## Amazon vs Google 2011
([overview](#overview))

From Steve Yegge's legendary [platforms rant](https://gist.github.com/chitchcock/1281611). See also [Yegge's 4-way FAGM comparison](yegges-conservative-liberal-axis) w.r.t. the conservative-liberal axis in software development.

Amazon:

```markdown
I was at Amazon for about six and a half years, and now I've been at Google for that long. 
One thing that struck me immediately about the two companies -- an impression that has been
reinforced almost daily -- is that Amazon does everything wrong, and Google does everything 
right. Sure, it's a sweeping generalization, but a surprisingly accurate one. It's pretty 
crazy. There are probably a hundred or even two hundred different ways you can compare the 
two companies, and Google is superior in all but three of them, if I recall correctly. I a
ctually did a spreadsheet at one point but Legal wouldn't let me show it to anyone, even 
though recruiting loved it.

I mean, just to give you a very brief taste: Amazon's recruiting process is fundamentally 
flawed by having teams hire for themselves, so their hiring bar is incredibly inconsistent
across teams, despite various efforts they've made to level it out. And their operations 
are a mess; they don't really have SREs and they make engineers pretty much do everything,
which leaves almost no time for coding - though again this varies by group, so it's luck of
the draw. They don't give a single shit about charity or helping the needy or community 
contributions or anything like that. Never comes up there, except maybe to laugh about it.
Their facilities are dirt-smeared cube farms without a dime spent on decor or common meeting 
areas. Their pay and benefits suck, although much less so lately due to local competition 
from Google and Facebook. But they don't have any of our perks or extras -- they just try 
to match the offer-letter numbers, and that's the end of it. Their code base is a disaster,
with no engineering standards whatsoever except what individual teams choose to put in place.

To be fair, they do have a nice versioned-library system that we really ought to emulate, and
a nice publish-subscribe system that we also have no equivalent for. But for the most part 
they just have a bunch of crappy tools that read and write state machine information into
relational databases. We wouldn't take most of it even if it were free.

I think the pubsub system and their library-shelf system were two out of the grand total of 
three things Amazon does better than google.

I guess you could make an argument that their bias for launching early and iterating like mad
is also something they do well, but you can argue it either way. They prioritize launching 
early over everything else, including retention and engineering discipline and a bunch of
other stuff that turns out to matter in the long run. So even though it's given them some
competitive advantages in the marketplace, it's created enough other problems to make it
something less than a slam-dunk. 
```

Google: 

```markdown
That one last thing that Google doesn't do well is Platforms. We don't understand platforms.
We don't "get" platforms. Some of you do, but you are the minority. This has become painfully
clear to me over the past six years. I was kind of hoping that competitive pressure from 
Microsoft and Amazon and more recently Facebook would make us wake up collectively and start 
doing universal services. Not in some sort of ad-hoc, half-assed way, but in more or less the 
same way Amazon did it: all at once, for real, no cheating, and treating it as our top priority
from now on.

But no. No, it's like our tenth or eleventh priority. Or fifteenth, I don't know. It's pretty 
low. There are a few teams who treat the idea very seriously, but most teams either don't think
about it all, ever, or only a small percentage of them think about it in a very small way.

It's a big stretch even to get most teams to offer a stubby service to get programmatic access
to their data and computations. Most of them think they're building products. And a stubby 
service is a pretty pathetic service. Go back and look at that partial list of learnings from
Amazon, and tell me which ones Stubby gives you out of the box. As far as I'm concerned, it's
none of them. Stubby's great, but it's like parts when you need a car. ...

Google+ is a prime example of our complete failure to understand platforms from the very 
highest levels of executive leadership (hi Larry, Sergey, Eric, Vic, howdy howdy) down to the
very lowest leaf workers (hey yo). We all don't get it. The Golden Rule of platforms is that 
you Eat Your Own Dogfood. The Google+ platform is a pathetic afterthought. We had no API at all
at launch, and last I checked, we had one measly API call. One of the team members marched in 
and told me about it when they launched, and I asked: "So is it the Stalker API?" She got all
glum and said "Yeah." I mean, I was joking, but no... the only API call we offer is to get 
someone's stream. So I guess the joke was on me.

Microsoft has known about the Dogfood rule for at least twenty years. It's been part of their
culture for a whole generation now. You don't eat People Food and give your developers Dog Food.
Doing that is simply robbing your long-term platform value for short-term successes. Platforms
are all about long-term thinking.

Google+ is a knee-jerk reaction, a study in short-term thinking, predicated on the incorrect 
notion that Facebook is successful because they built a great product. But that's not why they
are successful. Facebook is successful because they built an entire constellation of products 
by allowing other people to do the work. So Facebook is different for everyone. Some people 
spend all their time on Mafia Wars. Some spend all their time on Farmville. There are hundreds
or maybe thousands of different high-quality time sinks available, so there's something there 
for everyone.

Our Google+ team took a look at the aftermarket and said: "Gosh, it looks like we need some 
games. Let's go contract someone to, um, write some games for us." Do you begin to see how 
incredibly wrong that thinking is now? The problem is that we are trying to predict what people 
want and deliver it for them.

You can't do that. Not really. Not reliably. There have been precious few people in the world,
over the entire history of computing, who have been able to do it reliably. Steve Jobs was one
of them. We don't have a Steve Jobs here. I'm sorry, but we don't.
```

<a name="#platforms"></a>
## Platforms
([overview](#overview))

The following couple of quotes are all from Steve Yegge's legendary [platforms rant](https://gist.github.com/chitchcock/1281611). Yegge starts with the Big Mandate to set things up:

```markdown
One day Jeff Bezos issued a mandate. He's doing that all the time, of course, and people 
scramble like ants being pounded with a rubber mallet whenever it happens. But on one 
occasion -- back around 2002 I think, plus or minus a year -- he issued a mandate that was
so out there, so huge and eye-bulgingly ponderous, that it made all of his other mandates 
look like unsolicited peer bonuses.

His Big Mandate went something along these lines:

1. All teams will henceforth expose their data and functionality through service interfaces.

2. Teams must communicate with each other through these interfaces.

3. There will be no other form of interprocess communication allowed: no direct linking, 
no direct reads of another team's data store, no shared-memory model, no back-doors whatsoever.
The only communication allowed is via service interface calls over the network.

4. It doesn't matter what technology they use. HTTP, Corba, Pubsub, custom protocols -- doesn't
matter. Bezos doesn't care.

5. All service interfaces, without exception, must be designed from the ground up to be
externalizable. That is to say, the team must plan and design to be able to expose the interface 
to developers in the outside world. No exceptions.

6. Anyone who doesn't do this will be fired.

7. Thank you; have a nice day!

Ha, ha! You 150-odd ex-Amazon folks here will of course realize immediately that #7 was a little
joke I threw in, because Bezos most definitely does not give a shit about your day.

#6, however, was quite real, so people went to work. Bezos assigned a couple of Chief Bulldogs to
oversee the effort and ensure forward progress, headed up by Uber-Chief Bear Bulldog Rick Dalzell.
Rick is an ex-Armgy Ranger, West Point Academy graduate, ex-boxer, ex-Chief Torturer slash CIO at 
Wal*Mart, and is a big genial scary man who used the word "hardened interface" a lot. Rick was a 
walking, talking hardened interface himself, so needless to say, everyone made LOTS of forward 
progress and made sure Rick knew about it.

Over the next couple of years, Amazon transformed internally into a service-oriented architecture.
They learned a tremendous amount while effecting this transformation. There was lots of existing 
documentation and lore about SOAs, but at Amazon's vast scale it was about as useful as telling 
Indiana Jones to look both ways before crossing the street. Amazon's dev staff made a lot of 
discoveries along the way. A teeny tiny sampling of these discoveries included:

- pager escalation gets way harder, because a ticket might bounce through 20 service calls before the
real owner is identified. If each bounce goes through a team with a 15-minute response time, it 
can be hours before the right team finally finds out, unless you build a lot of scaffolding and 
metrics and reporting.

- every single one of your peer teams suddenly becomes a potential DOS attacker. Nobody can make any
real forward progress until very serious quotas and throttling are put in place in every single 
service.

- monitoring and QA are the same thing. You'd never think so until you try doing a big SOA. But when
your service says "oh yes, I'm fine", it may well be the case that the only thing still 
functioning in the server is the little component that knows how to say "I'm fine, roger roger, 
over and out" in a cheery droid voice. In order to tell whether the service is actually responding,
you have to make individual calls. The problem continues recursively until your monitoring is doing
comprehensive semantics checking of your entire range of services and data, at which point it's 
indistinguishable from automated QA. So they're a continuum.

- if you have hundreds of services, and your code MUST communicate with other groups' code via these
services, then you won't be able to find any of them without a service-discovery mechanism. And you
can't have that without a service registration mechanism, which itself is another service. So Amazon
has a universal service registry where you can find out reflectively (programmatically) about every
service, what its APIs are, and also whether it is currently up, and where.

- debugging problems with someone else's code gets a LOT harder, and is basically impossible unless
there is a universal standard way to run every service in a debuggable sandbox.

That's just a very small sample. There are dozens, maybe hundreds of individual learnings like these
that Amazon had to discover organically. There were a lot of wacky ones around externalizing services
, but not as many as you might think. Organizing into services taught teams not to trust each other 
in most of the same ways they're not supposed to trust external developers.

This effort was still underway when I left to join Google in mid-2005, but it was pretty far advanced.
From the time Bezos issued his edict through the time I left, Amazon had transformed culturally into 
a company that thinks about everything in a services-first fashion. It is now fundamental to how they
approach all designs, including internal designs for stuff that might never see the light of day 
externally.

At this point they don't even do it out of fear of being fired. I mean, they're still afraid of that;
it's pretty much part of daily life there, working for the Dread Pirate Bezos and all. But they do 
services because they've come to understand that it's the Right Thing. There are without question 
pros and cons to the SOA approach, and some of the cons are pretty long. But overall it's the right
thing because SOA-driven design enables Platforms.
```

Why did Bezos want to platformize Amazon?

```markdown
But Bezos realized long before the vast majority of Amazonians that Amazon needs to be a platform.

You wouldn't really think that an online bookstore needs to be an extensible, programmable platform.
Would you?

Well, the first big thing Bezos realized is that the infrastructure they'd built for selling and
shipping books and sundry could be transformed an excellent repurposable computing platform. So 
now they have the Amazon Elastic Compute Cloud, and the Amazon Elastic MapReduce, and the Amazon 
Relational Database Service, and a whole passel' o' other services browsable at aws.amazon.com. 
These services host the backends for some pretty successful companies, reddit being my personal 
favorite of the bunch.

The other big realization he had was that he can't always build the right thing. I think Larry 
Tesler might have struck some kind of chord in Bezos when he said his mom couldn't use the goddamn
website. It's not even super clear whose mom he was talking about, and doesn't really matter, 
because nobody's mom can use the goddamn website. In fact I myself find the website disturbingly 
daunting, and I worked there for over half a decade. I've just learned to kinda defocus my eyes 
and concentrate on the million or so pixels near the center of the page above the fold.
```

Platforms matter because they allow Accessibility:

```markdown
I'm not really sure how Bezos came to this realization -- the insight that he can't build one 
product and have it be right for everyone. But it doesn't matter, because he gets it. There's
actually a formal name for this phenomenon. It's called Accessibility, and it's the most 
important thing in the computing world.

The. Most. Important. Thing.

If you're sorta thinking, "huh? You mean like, blind and deaf people Accessibility?" then you're
not alone, because I've come to understand that there are lots and LOTS of people just like you:
people for whom this idea does not have the right Accessibility, so it hasn't been able to get 
through to you yet. It's not your fault for not understanding, any more than it would be your
fault for being blind or deaf or motion-restricted or living with any other disability. When 
software -- or idea-ware for that matter -- fails to be accessible to anyone for any reason, 
it is the fault of the software or of the messaging of the idea. It is an Accessibility failure.

Like anything else big and important in life, Accessibility has an evil twin who, jilted by the 
unbalanced affection displayed by their parents in their youth, has grown into an equally 
powerful Arch-Nemesis (yes, there's more than one nemesis to accessibility) named Security. And 
boy howdy are the two ever at odds.

But I'll argue that Accessibility is actually more important than Security because dialing 
Accessibility to zero means you have no product at all, whereas dialing Security to zero can still
get you a reasonably successful product such as the Playstation Network. 
```

Platform-product relationship:

```markdown
A product is useless without a platform, or more precisely and accurately, 
a platform-less product will always be replaced by an equivalent platform-ized product.

I apologize to those (many) of you for whom all this stuff I'm saying is incredibly obvious,
because yeah. It's incredibly frigging obvious. Except we're (Google) not doing it. We don't get 
Platforms, and we don't get Accessibility. The two are basically the same thing, because platforms
solve accessibility. A platform is accessibility.
```


<a name="#Programming-languages"></a>
## Programming languages
([overview](#overview))

<a name="#smalltalk"></a>
### Smalltalk
([overview](#overview))

Alan Kay, in 1998, emphasizing comms/messaging over object properties or even behavior:

```markdown
Just a gentle reminder that I took some pains at the last OOPSLA to try to remind everyone that
Smalltalk is not only NOT its syntax or the class library, it is not even about classes. I’m sorry
that I long ago coined the term “objects” for this topic because it gets many people to focus on
the lesser idea.

The big idea is “messaging” - that is what the kernel of Smalltalk/Squeak is all about (and it’s 
something that was never quite completed in our Xerox PARC phase). The Japanese have a small word
- ma - for “that which is in between” - perhaps the nearest English equivalent is “interstitial”. 
The key in making great and growable systems is much more to design how its modules communicate 
rather than what their internal properties and behaviors should be. Think of the internet - to 
live, it (a) has to allow many different kinds of ideas and realizations that are beyond any single
standard and (b) to allow varying degrees of safe interoperability between these ideas.
```

<a name="#CS-is-beyond-the-glass-ceiling-of-pop-science"></a>
## CS is beyond the glass ceiling of pop science
([overview](#overview))

Greg Kuperberg's comment on Scott Aaronson's post [Logicians on safari](https://www.scottaaronson.com/blog/?p=152), responding to "There are zillions of pop science books about physics, math, biology… but honestly, I can’t think of any notable popular theoretical computer science books":

```markdown
I respect popular science writing as much as anyone, but it is easy to spend too much time 
kicking yourself if your area doesn’t benefit from it. At the end of the day, popular science
is written to entertain people, and hopefully to attract interest, but not to teach them. It 
isn’t another form of school. Popular science will inevitably overreward some areas and 
underreward others.

In particular, popular science has a “glass ceiling” that will prevent you from communicating 
many great ideas. I had an epiphany about this when I was at the house of a relative many years
ago. He was a smart guy with a far-above-average interest in poular science, but he did not 
have advanced training in mathematics. I think that he had more mathematics books than I do;
certainly he had more math biographies.

At one point he was interested in the Rubik’s cube. The Rubik’s cube is different from other 
popular mathematics, becuase it goads you to actually solve the damn thing instead of just 
reading about mathematicians at work. So he bought four books on how to solve the Rubik’s cube.
But with a good understanding of undergraduate group theory, one would have been more than 
enough! Without some solid mathematical intuition of some kind (not necessarily a group theory
course), books on the Rubik’s cube are downright painful. That really revealed the glass ceiling.

It seems that TCS is generally beyond the glass ceiling of popular science. I think that it’s
because TCS is made up of theorems. It’s not so hard explain what a theorem is. But it is hard
to explain, except to those who have joined the club, how much it matters to prove theorems. 
In fact some science journalists have discussed their impression that theorems are just a chore
that can be skipped, postponed, or hopefully soon relegated to computers.
```

And in response to "I have to respectfully disagree about Theoretical Computer Science being beyond the glass ceiling of popular science":

```markdown
The glass ceiling is in different places for different people, and in different venues. I am 
thinking of what gets published in the New York Times Science section. That is not at the 
level of what is written by a PhD that you might find interesting, but rather more at the 
level of what you might write for people on the next rung down the ladder.

Look at how much the Times watered down Sara Robinson’s article on the result that primality 
is in P. It was still a very nice article, but it was radically restricted to the basics. The
Times really seems to believe that the significance of theorems is all but beyond their
readership, that is only worth mentioning when the story is as big as the Poincare Conjecture 
or Fermat’s Last Theorem. Although I personally think that the Times is too conservative on 
this point, they probably aren’t completely wrong.
```

<a name="#Theoretical-CS-contributions"></a>
## Theoretical CS contributions
([overview](#overview))

From Scott Aaronson's post [Logicians on safari](https://www.scottaaronson.com/blog/?p=152), responding to Sean Carroll's claim:

```markdown
I’m happy to admit that I don’t know anything about “one-way functions and interactive proofs.”
So, in what sense has theoretical computer science contributed more in the last 30 years to our
basic understanding of the universe than particle physics or cosmology? (Despite the fact that
I’m a cosmologist, I don’t doubt your statement — I’d just like to be able to explain it in public.)
```

The context for Sean's comment was [this post of Scott's](https://www.scottaaronson.com/blog/?p=151), lamenting and criticquing Steve Lohr's NYT essay that started off like so:

```markdown
Computer science is not only a comparatively young field, but also one that has had to prove it 
is really science. Skeptics in academia would often say that after Alan Turing described the
concept of the “universal machine” in the late 1930’s — the idea that a computer in theory could
be made to do the work of any kind of calculating machine, including the human brain — all that 
remained to be done was mere engineering.

The more generous perspective today is that decades of stunningly rapid advances in processing 
speed, storage and networking, along with the development of increasingly clever software, have
brought computing into science, business and culture in ways that were barely imagined years ago.
The quantitative changes delivered through smart engineering opened the door to qualitative changes.
```

which resulted in Scott's rueful rant:

```markdown
Even among the commenters on this post by Chad Orzel — which Dave Bacon forwarded to me with the
subject line “bait” — awareness of any third possibility seems depressingly rare. Judging from the
evidence, it’s not that people have engaged the mysteries of P versus NP, randomness and 
determinism, one-way functions and interactive proofs, and found them insufficiently deep. Rather, 
as bizarre as it sounds, it’s that people don’t know these mysteries exist — just as they wouldn’t 
know about black holes or the Big Bang if no one told them. If you want to understand why our
subject — which by any objective standard, has contributed at least as much over the last 30 years
as (say) particle physics or cosmology to humankind’s basic picture of the universe — receives a
whopping $5 million a year from the NSF (with even that in constant danger), look no further.
```

Enough backtracking/context-setting. Here's what Scott has to say in response to Sean; this is also the origin of the "theoretical CS is quantitative epistemology" quote:

```markdown
Of course I was joking when I mentioned “objective standards” for ranking scientific fields. 
Depending on which questions keep you up at night, different parts of “humankind’s basic picture
of the universe” will seem larger or smaller. (To say that, of course, is not to suggest any 
relativism about the picture itself.)

What I can do, though, is to tell you why — by my own subjective standards — the contributions 
of theoretical computer science over the last 30 years rival those of theoretical physics or any 
other field I know about. Of course, people will say I only think that because I’m a theoretical 
computer scientist, but that gets the causal arrow wrong: I became a theoretical computer
scientist because, as a teenager, I thought it!

It’s probably best to start with some examples.

1. We now know that, if an alien with enormous computational powers came to Earth, it could prove to
us whether White or Black has the winning strategy in chess. To be convinced of the proof, we would
not have to trust the alien or its exotic technology, and we would not have to spend billions of 
years analyzing one move sequence after another. We’d simply have to engage in a short conversation
with the alien about the sums of certain polynomials over finite fields.

2. There’s a finite (and not unimaginably-large) set of boxes, such that if we knew how to pack those 
boxes into the trunk of your car, then we’d also know a proof of the Riemann Hypothesis. Indeed,
every formal proof of the Riemann Hypothesis with at most (say) a million symbols corresponds to
some way of packing the boxes into your trunk, and vice versa. Furthermore, a list of the boxes 
and their dimensions can be feasibly written down.

3. Supposing you do prove the Riemann Hypothesis, it’s possible to convince someone of that fact, 
without revealing anything other than the fact that you proved it. It’s also possible to write the
proof down in such a way that someone else could verify it, with very high confidence, having only
seen 10 or 20 bits of the proof.

4. If every second or so your computer’s memory were wiped completely clean, except for the input data; 
the clock; a static, unchanging program; and a counter that could only be set to 1, 2, 3, 4, or 5,
it would still be possible (given enough time) to carry out an arbitrarily long computation — just
as if the memory weren’t being wiped clean each second. This is almost certainly not true if the
counter could only be set to 1, 2, 3, or 4. The reason 5 is special here is pretty much the same
reason it’s special in Galois’ proof of the unsolvability of the quintic equation.

5. It would be great to prove that RSA is unbreakable by classical computers. But every known technique 
for proving that would, if it worked, simultaneously give an algorithm for breaking RSA! For example,
if you proved that RSA with an n-bit key took n^5 steps to break, you would’ve discovered an algorithm
for breaking it in 2n^1/5 steps. If you proved that RSA took 2n^1/3 steps to break, you would’ve 
discovered an algorithm for breaking it in n(log n)^2 steps. As you show the problem to be harder,
you simultaneously show it to be easier.

Alright, let me stop before I get carried away. The examples I’ve listed (and hundreds more like them) 
are not exactly discoveries about physics, but they don’t have the flavor of pure math either. And 
even if they have some practical implications for computing (which they do), they certainly don’t have
the flavor of nitty-gritty software engineering.

So what are they then? Maybe it’s helpful to think of them as “quantitative epistemology”: discoveries
about the capacities of finite beings like ourselves to learn mathematical truths. On this view, the
theoretical computer scientist is basically a mathematical logician on a safari to the physical world: 
someone who tries to understand the universe by asking what sorts of mathematical questions can and 
can’t be answered within it. Not whether the universe is a computer, but what kind of computer it is!
Naturally, this approach to understanding the world tends to appeal most to people for whom math (and
especially discrete math) is reasonably clear, whereas physics is extremely mysterious.

In my opinion, one of the biggest challenges for our time is to integrate the enormous body of
knowledge in theoretical computer science (or quantitative epistemology, or whatever you want to call
it) with the rest of what we know about the universe. In the past, the logical safari mostly stayed
comfortably within 19th-century physics; now it’s time to venture out into the early 20th century. 
Indeed, that’s exactly why I chose to work on quantum computing: not because I want to build quantum
computers (though I wouldn’t mind that), but because I want to know what a universe that allows
quantum computers is like.

Incidentally, it’s also why I try hard to keep up with your field. If I’m not mistaken, less than a 
decade ago cosmologists made an enormous discovery about the capacity of finite beings to learn 
mathematical truths: namely, that no computation carried out in the physical world can ever involve
more than 1/Λ ~ 10^122 bits.
```

Or in more straightforward (if impenetrable to me) jargon:

```markdown
Oh, alright:

(1) IP=PSPACE (Shamir 1990).

(2) 3-dimensional bin-packing is NP-complete.

(3) NP has zero-knowledge proofs (Goldreich-Micali-Wigderson 1986); the PCP Theorem.

(4) Width-5 branching programs can compute NC1 (Barrington 1986); corollary pointed out by
Ogihara 1994 that width-5 bottleneck Turing machines can compute PSPACE

(5) Natural proofs (Razborov-Rudich 1993); in particular Wigderson’s observation about
natural proofs for discrete log.
```

Gil Kalai's own list is also great, and admirably straight to the point:

```markdown
Hi Scott

Let me try to suggest a skeleton for a good answer to Sean Carroll on some main insights
developed in theoretical computer science which with more effort can be explained to a 
layperson. I would personally prefer a description which at the end is not polemic, 
apologetic, or too sophisticated.

1. The notion of an algorithm. Some basic insights from the theory of algorithms: the 
importance of storing of hashing and of backtracking

2. The idea that a computer cannot do everything. Intractability and the NP = P problem

3. What computers can (magically) do very quickly. FFT and other basic algorithms in
mathematical and scientific computing.

4. What computers can do but hardly: Linear programming. Semi definite programming and 
related optimization problems.

5. “Beyond a reasonable doubt:” the notion of probabilistic proof

6. The notion of interactive proofs. Like in court, interactive process can raise the 
ability of reaching the truth.

7. Secrets and lies. The depth and fundamental importance of cryptography. (And while 
talking about crypthography, sure, the bizzare and amazing notion of zero-knowledge proofs.)

8. (If we want to reach the cutting edge:) The notion of probabilistically checkable proofs 
and hardness of approximation.

9. Distributed system. The difficulty of cooperation and synchronization.

10. Underatnding, using tools developed in theoretical computer science, the notions of 
“learning” and “knowledge”.

11. Merging computation and economics: lies and strategies.

12. Quantum computation.

Of course, this refer only to a small part of theoretical computer science (STOC/FOCS).
```

In response to Greg's comment that TCS "doesn't sound different from what we do in pure math":

```markdown
Greg: I’m delighted you agree with me that TCS, whatever else it is, is also “perfectly 
satisfactory as pure math”! But alas, not all mathematicians see things the way you do: to
many of them, the goal of “real” or “deep” math is to start from dizzyingly-general theorems
about infinite-dimensional spaces and then generalize them even further. The TCS goal, of 
course, is to take laughably-concrete problems that we can’t solve and then identify special
cases that we still can’t solve. Same standards for deciding what’s true; different aesthetic.

That said, the TCS and math aesthetics drew noticeably closer in just the past decade (see 
Luca’s blog for more on that theme), and maybe they’ll be indistinguishable at some point in 
the future. Basically, I see TCS and math as Galapagos finches that lived on different islands
for quite a while, but that are probably still interfertile.
```

Greg isn't happy at all with Scott's response:

```markdown
Of course I can’t be happy about this description of pure mathematics, and frankly I’m a 
little surprised to hear it from you. As I said, pure math comes in many different flavors.
Naturally, when you see a flavor of it that is far from your own, it might impress you as 
excessively abstract and on top of that pretentious. But wouldn’t it be safe to suppose, if
well-regarded people are doing the research, that their area can also be made to look 
unpretentious and beautiful?

More specifically, the presence of infinite-dimensional spaces is a strange criterion for 
deciding that topic is counting angels on the heads of pins. I don’t see that any of the seven
Clay Prize problems directly refer to infinite-dimensional spaces. The Yang-Mills problem 
comes the closest, but that’s because it’s a problem from physics!

But even if an area does use infinite-dimensional spaces, is that so bad? After all, P (i.e.,
boolean functions computable in polynomial time) is an infinite-dimensional vector space over
the field with two elements, and so is Delta^nP. Should I say that the conjecture that the
polynomial-time hierarchy does not collapse is exactly one of your absurdly general
conjectures about infinite-dimensional spaces?

Granted, non-collapse is a conjecture rather than a theorem. The set of oracles is also an 
infinite-dimensional vector space over Z/2, and the set of generic oracles is a highly 
abstract subset of this vector space. Do you think that it pushes the limits to prove a 
separation result using generic oracles?

But maybe these examples are too clever by half. If any theorem naturally fits the description
of an absurdly general fact about infinite-dimensional spaces, it would be the spectral 
theorem for self-adjoint operators on a Hilbert space. Do you seriously mean to say, given
that you are a quantum information theorist, that the spectral theorem is too abstract to 
matter?

*The TCS goal, of course, is to take laughably-concrete problems that we can’t solve and then
identify special cases that we still can’t solve.*

That is sometimes the goal, except that it’s usually a disingenuous goal because everyone knows
that the special cases are just as hard as the general cases. At least, so it went with Avi 
Wigderson’s special case of P vs #P at the ICM in Madrid.

*That said, the TCS and math aesthetics drew noticeably closer in just the past decade (see 
Luca’s blog for more on that theme), and maybe they’ll be indistinguishable at some point in 
future. Basically, I see TCS and math as Galapagos finches that lived on different islands for
quite a while, but that are probably still interfertile.*

I don’t know quite when or whether TCS drew closer to pure mathematics, but I can point to 
the fact that both Luca and Avi gave invited talks at the International Congress of
Mathematicians. Could the TCS community be disregarding some important olive branches? It is
true that TCS and math are on different “islands”, in the trivial sense of being in different
departments. That, I think, is the only real schism. It’s like what they say about America and
Britain: two nations divided by a common language.
```

<a name="#optimization"></a>
## Optimization
([overview](#overview)) 

<a name="#The-unreasonable-effectiveness-of-a-thousand-small-optimizations"></a>
### The unreasonable effectiveness of a thousand small optimizations
([overview](#overview)) 

From Venkat's [eponymous article](https://us1.campaign-archive.com/?u=78cbbb7f2882629a5157fa593&id=3d9f8e7dc5). 

```markdown
The challenge of building large-scale complex systems often gets caught between
purist visions that never get off the ground and seemingly pragmatic random-walk 
tinkering that slowly grinds to a halt via diminishing returns. How do you break
out of this rock-and-a-hard place impasse?

My friend Keith Adams, veteran of several such complex scaling challenges at 
VMWare, Facebook, and now Slack, pointed out the key insight: what he calls the 
"unreasonable effectiveness of small optimizations." I am going to paraphrase the
version he shared over lunch at the Facebook campus a few years ago and call it
Keith's Law: In a complex system, the cumulative effect of a large number of small
optimizations is externally indistinguishable from a radical leap. If you want to
do big things in a software-eaten world, it is absolutely crucial that you 
understand Keith's Law.
```

The Keith Adams here is precisely *the* Keith Adams that Carlos Bueno worked with in [performance optimization](#Performance-optimization). He happened to write what's effectively a [defense of PHP](https://slack.engineering/taking-php-seriously-cf7a60065329), a novel and daring enough stance that I included it in this notebook as a counterpoint to the usual criticism, made all the more valuable because Venkat pretty much contextualized Keith's PHP-defense within the insight in *this* subsection (read more below).

Intuition pump illustration:

![small-optimizations](https://gallery.mailchimp.com/78cbbb7f2882629a5157fa593/images/93a830e5-27ce-4624-bbab-1691e499af36.png)

```markdown
1/ Let's unpack Keith's Law: *In a complex system, the cumulative effect of a 
large number of small optimizations is externally indistinguishable from a radical
leap*.

5/ Dan Luu discussed scale-effects blindness in his excellent recent post, Why's
that company so big? I could do that in a weekend.

6/ The question reveals a basic inability to switch between weed-level and system-
level perspectives of complexity, and how the two levels relate.

7/ Every great technologist I’ve met, however, with a track record of big 
achievements, seems to intuitively grok Keith’s Law. It is quite amazing how
consistent this trait is: 100% of my sample set.

8/ To understand why, consider what happens as you expand a system's capability,
adding capacity, features, and coverage of increasingly rare corner cases.

9/ As you do this, failure modes become more catastrophic, bugs become more obscure,
and improbable things become probable.

10/ You start to fall behind on situation awareness and urgent starts to outrun
important. Things slow to a crawl along a 1000-project frontier. Work begins to
resemble attrition warfare against chaos.

11/ In companies with mediocre engineering leadership, this can lead to out-of-
control reactive fire-fighting, where huge teams are doing a thousand unrelated
things.

12/ A growing complex system is like a huge machine with a proliferating number 
of tuning/tweaking knobs, each staffed by a small, depressed and stressed-out 
team.

13/ Turning a given knob makes some things better, other things worse. Usually,
the good is concentrated locally, the bad is diffused globally.

14/ The depressed losers give up, the sociopaths switch to zero-sum mode, moving 
the system towards a  "privatize gains, socialize losses" regime of operations. 
The clueless stir in extra chaos.

15/ The knobs also interact to drive emergent behavior. If two knobs are turned a
certain way at the same time, they could trigger higher-dimensional emergent 
behavior. The world gets weirder.

16/ Such systems can be thought of as having significant decision-making slop. 
Small decisions have both local, deterministic effects and global, probabilistic
effects.

17/ The global probabilistic effects constitute decision-making slop, which can
either power a grand systemic random walk to zemblanity, or accumulating 
serendipity: the unreasonable effectiveness.

18/ A random walk does not mean a system stays in the same place. It means it 
will slowly drift. Generally in a “bad” direction, since bad directions outnumber
good ones.

19/ But, with the right people in the right places, the random walk can turn into
slow steady progress in a chosen direction. What do they do that's so special? 
They harness Keith's Law.

20/ At smaller scales, one person with god-level visibility into, and comprehension
of, the system can keep it all in their head and herd the various knob-turnings/
tweakings in a chosen direction.

21/ But in a complex system, where hundreds of people can be doing little things,
this does not work. And more communication is not the answer (at least not the 
whole answer). 

22/ As Keith observed once, most humans can at best understand 1-2 levels of
abstraction above/below their home zone. Beyond, you rely on things like metaphor
and pop sociology.

23/ So architects and leaders being deluged by a firehose of information on ongoing
firefights is useless. At some point even the most formidable genius cannot keep up.
```

Tangent: perhaps the limit is somewhere near Stephen Wolfram with his company. Wolfram [reviews every damn line of code](https://blog.stephenwolfram.com/2008/01/ten-thousand-hours-of-design-reviews/) prior to rolling out new versions of WolframAlpha. Not for him, the [philosophy of perpetual beta](#Perpetual-beta)...

```markdown
24/ OTOH, the naive version of what is sometimes called the “holographic” model,
where everybody sort of has the “DNA” of the whole thing in their head or muscle
memory, is worse.

25/ If the overwhelmed architect leads the troops on a death march, the supposedly
smart "crowd" tears itself apart because shared "DNA" does not equal shared 
direction.

26/ The way out is people with strong “finger-tip feeling” (which we’ve discussed
before), herding the system, which can turn the uncontrolled random walk into 
controlled, cumulative gains. 

27/ They have an intuitive sense of which tactical challenges also have the power 
to herd the whole system in good directions, towards serendipity. It's not think-
global/act local. It's feel-global/act local.

28/ They are able to pick out “herding” knobs whose probabilistic effects have a 
somewhat predictable direction, and are likely to "socialize gains and limit losses"

29/ This effect is most visible where there is an obvious core piece in the system.
In a computer for example, smaller, faster and more memory are all generally good 
things.

30/ This is not the same as the 80-20 principle. 80% of the gains cannot be 
deterministically attributed to 20% of the improvements. That’s the “leverage” view
of complex systems.

31/ The “leverage” view of leads people to go on futile, quixotic quests for the 
“one weird trick” that will magically trigger a big leap in a  system that is 
assumed to be complex in a Rube-Goldberg sense. 
```

Venkat contrasts here with Donella Meadows: [Leverage Points: Places to Intervene in a System](http://donellameadows.org/archives/leverage-points-places-to-intervene-in-a-system/).

```markdown
32/ Architect Indy Johar suggested what might be called the “resonance” view: 
getting the parts of the complex system to harmonize through loose mutual awareness.
This is a probabilistic view.

33/ A system with such resonance is ripe for Keith’s Law to operate. It creates a
system-level harmonies in the environment that can shape positive spillover and 
surplus effects.

34/ In such a resonant system, catalysis, rather than leverage, is key. What things
can you do that makes other things increasingly easier, and cumulative in their 
effects?

35/ This is not a one-shot thing. You have to keep finding new herding knobs as old
ones lose potency and new ones become available due to ongoing growth.

36/ The “herding” potential of a given knob is finite, and limited to a range of 
system behaviors. Leadership is knowing when you've entered the range of a given 
knob, and when you've exited it.

37/ This is the essence of Schwerpunkt — the ability to repeatedly find the “center
of gravity” where effort drives systemic synergy.
```

<a name="#Performance-optimization"></a>
### Performance optimization
([overview](#overview)) 

```markdown
There is a rich & vibrant oral tradition about how to 
write fast programs, and almost all of it is horseshit.
```

Pretty much everything here comes from Carlos Bueno's excellent [handbook on mature optimization practices](http://carlos.bueno.org/optimization/mature-optimization.pdf), including the quote above. He's just endlessly quotable.  

Everyone knows about Donald Knuth's 

```markdown
premature optimization is the root of all evil
```

but few are aware it's part of a longer quote from his book *Structured Programming With go to Statements* that finishes with an important caveat: 

```markdown
Programmers waste enormous amounts of time
thinking about, or worrying about, the speed of non-
critical parts of their programs, and these attempts
at efficiency actually have a strong negative impact
when debugging and maintenance are considered.
We should forget about small efficiencies, say about
97% of the time; premature optimization is the
root of all evil. Yet we should not pass up our op-
portunities in that critical 3%.
```

That's how Carlos begins his introduction. The very next thing he says hooked me, as it contains just an unbelievable amount of good high-level advice:

```markdown
The trickiest part of speeding up a program is not doing it,
but deciding whether it’s worth doing at all. There are few clear
principles, only rules of thumb.

Part of the problem is that optimization is hard to do well.
It’s frighteningly easy to devolve into superstitious ritual and
rationalization. Then again, there can be big payoffs hidden in
surprising places. That’s why expert advice about performance
tends to have a gnomic, self-contradictory flavor: “If you don’t
know what you are doing, don’t do it! You’ll know if you know
what you are doing. And remember to design your programs
for performance.” The experts are acutely worried about en-
couraging more folly, yet can’t quite bring themselves to ignore
the possible gains.

Knuth’s famous quote about premature optimization was
never meant to be a stick to beat people over the head with.
It’s a witty remark he tossed off in the middle of a keen obser-
vation about leverage, which itself is embedded in a nuanced,
evenhanded passage about, of all things, using gotos for fast and
readable code. The final irony is that the whole paper was an
earnest attempt to caution against taking Edsger Dijkstra’s infa-
mous remark about gotos too seriously. It’s a wonder we risk
saying anything at all about this stuff.

*Structured Programming With go to Statements* does make two
valuable points about performance. Optimizing without measurement
to guide you is foolish. So is trying to optimize everything. The
biggest wins tend to be concentrated in a small
portion of the code, “that critical 3%”, which can be found via
careful measurement.

While a proper measurement regime can tell you where optimization is
likely to succeed, it says little about whether doing it is worthwhile.
Knuth ultimately shoves that responsibility onto a hypothetical “good”
and “wise” programmer, who is able to look past the witty remarks and 
dire warnings and decide on the merits. Great, but how? 

I don’t know either. Performance optimization is, or should 
be, a cost/benefit decision. It’s made in the same way you decide just 
how much effort to put into other cross-cutting aspects
of a system like security and testing. There is such a thing as
too much testing, too much refactoring, too much of anything
good. In my experience, it makes most sense on mature systems
whose architectures have settled down.

The age of a piece of code is the single greatest predictor
of how long it will live. Stastically speaking, you encounter a
piece of code somewhere in the middle of its lifespan. If it’s
one month old, the odds are good it will be rewritten in another
month. A five-year-old function is not “ready to be rewritten”,
it’s just getting started on a long career. New code is almost
by definition slow code, but it’s also likely to be ripped out and
replaced as a young program slouches towards beta-test. Unless
your optimizations are going to stick around long enough to
pay for the time you spend making them plus the opportunity
cost of not doing something else, it’s a net loss.

Optimization also makes sense when it’s needed for a program to
ship. Performance is a feature when your system has
unusually limited resources to play with or when it’s hard to
change the software after the fact. This is common in games
programming, and is making something of a comeback with
the rise of mobile computing.
```

Measuring really does matter. Knuth for emphasis:

```markdown
“It is often a mistake to make a priori judgments
about what parts of a program are really critical,
since the universal experience of programmers who
have been using measurement tools has been that
their intuitive guesses fail.
```

A personal anecdote served as warning, and an example of "fixing the wrong problem":

```markdown
Even with all that, there are no guarantees. In the early 2000s
I helped build a system for search advertising. We didn’t have
a lot of money so we were constantly tweaking the system for
more throughput. The former CTO of one of our competitors,
looking over our work, noted that we were handling ten times
the traffic per server than he had. Unfortunately, we had spent
so much time worrying about performance that we didn’t pay
enough attention to credit card fraud. Fraud and chargebacks
got very bad very quickly, and soon after our company went
bankrupt. On one hand, we had pulled off a remarkable engineering
feat. On the other hand, we were fixing the wrong problem.
```

To fix, first know what you're fixing. In "Defining the Problem" Carlos' advice goes:

```markdown
Before you can optimize anything you need a way to measure what
you are optimizing. Otherwise you are just shooting
in the dark. Before you can measure you need a clear, explicit
statement of the problem you are trying to solve. Otherwise, in
a very real sense, you don’t know what you are doing.

Problem definitions often can be taken off the shelf. They
are a lot like recipes. Many people have been this way before
and there is a large body of knowledge available to you. There’s
nothing magical or hard to understand; the key is to be explicit
about the recipe you are following.

It’s impossible to clearly define the problem of clearly defining 
the problem. But there is a way to judge the quality of a
recipe. It must be specific enough to suggest a fix, and have an
unambiguous way to tell whether the fix worked. A problem
definition must be *falsifiable*. You have to risk being wrong to
have a chance at gaining the truth.
```

How might this look like in the real world? A parable:

```markdown
Let’s start with a bad definition and make it better.
 
	“WidgetFactoryServer is too slow.”
	
What does “slow” mean here? It could be that it takes so
long that a human notices (eg, more than 350 milliseconds)
or that some consumer of WFS times out while waiting for
a response, or perhaps it shows up on some measure of slow
components. “Too slow” is a judgement about *walltime*, ie time
passing according to the clock on the wall.

Two things generally contribute to walltime: computation
on the local CPU and time spent waiting for data from storage
or the network. You wrote WFS so you know that it doesn’t
read from disk or network. Another contributor in threaded
code is waiting for locks, but WFS isn’t threaded. So it’s 
probably all in computation. This fits a familiar pattern. 
We can use a ready-made problem definition.

	“WidgetFactoryServer is transactional. It receives
	requests and emits responses. It is probably CPU-bound.
	So if we profile to discover which functions
	take up the most time, and optimize those, the total
	CPU time per transaction should decrease.”
	
Good enough. It states a thesis about what resource is bottlenecked,
suggests a method of finding the right places to optimize, and 
is clear about what result you expect to see. Happily,
since we’re already measuring CPU, there’s no need for a 
separate measurement to test the result.

The actual optimization is almost anticlimactic. Alicia’s profiling 
finds that the most expensive function call in WFS has a
bit of clowniness in a tight loop, say it iterates a list of valid
WidgetTypes over and over again, or recalculates a value that
can be calculated once. Once she sees it, the fix is obvious and
testable. The CPU time drops and there is much rejoicing.
```

This leads to a problem I've encountered in the workplace -- while the lessons learned from past optimizations aren't *useless*, they should *always* be taken under advisement, never codified as law. Always, always measure:

```markdown
There is a rich & vibrant oral tradition about how to write fast
programs, and almost all of it is horseshit. It’s here in the after-
glow of success that it takes root. Alicia finds that eliminating a
piece of code that iterates WidgetTypes speeds up the program
by 10%. She spends the next two weeks searching for this pattern and 
“optimizing” wherever she finds it. “Iterating WidgetTypes is slow!” 
she tells her fellow coders. That might be technically true, but 
does it matter? Are those other instances in the
critical path? Do they show up in the measurements? Probably
not. Yet another folk remedy is born. After all, it worked once.

All of this define-the-problem-then-measure stuff isn’t like
a set of training wheels you cast off once you’ve learned how
to ride on your own. You really do have to approach every act
of optimization as an experiment, starting over from scratch,
making every assumption explicit and testable.

Computer systems are *astoundingly* complex, and it’s silly to
generalize too much from a given a performance bug. “We confi-
gured the number of threads to be twice the number of cores
and saw this speedup” is good science, but it is *not* the same
as “If you up the threads to 2X cores you will see a speedup”.
Wishing doesn’t make it so.

The lessons learned from past optimizations aren’t useless.
They can hint very strongly at where to look. But we are never
justified in trusting them blindly the way we trust, say, gravity.
If someone gives you a performance tip, ask for the data. If they
show you a benchmark, dig into the methodology. If they tell
you “X is slow” or “Y is fast”, take it under advisement. Then
measure it yourself, every time.
```

Carlos can't emphasize how important it is to measure. In "Flying by Instruments":

```markdown
The scariest part of flying a plane is learning to trust your
instruments. Humans are very bad at judging distance and orien-
tation in three dimensions, even pilots. When your eyes and
inner ear are telling you one thing and the ground is telling you
another, the ground wins every time. You have to accept that
there are very real human limitations that cannot be overcome
by talent or practice.

In a similar way, performance work depends on “flying” by
measurement. Humans are bad at predicting the performance
of complex systems, even programmers. *Especially* the programmers.
Our ability to create large & complex systems fools us
into believing that we’re also entitled to understand them. I
call it the Creator Bias, and it’s our number-one occupational
disease. Very smart programmers try to optimize or debug or
capacity-plan without good data, and promptly fall right out of
the sky.

How a program works and how it performs are very different
things. If you write a program or build a system, then of course
you know how it works. You can explain its expected behavior, 
logical flow, and computational complexity. A large part
of programming is playing computer in your head. It’s kind
of our thing. By all means, use your brain and your training to
guide you; it’s good to make predictions. But not all predictions
are good. Never forget that our human-scale understanding of
what’s supposed to happen is only a very rough approximation
of what actually does happen, in the real world on real hard-
ware over real users and data.
```

Big-O complexity is almost never the reason your program is slow in the real world:

```markdown
In the real world, Big-O complexity is almost never the reason your program is slow. Look at the slope of the N-squared
curve. In all probability, either N is so small that it doesn’t really matter, or N is so large and its effects so obvious that any
program with that kind of bug gets fixed quickly.

That means the stuff you have to contend with is the stuff
your professor told you to ignore: coefficients, constant factors,
and variability. Going from O(N2
) to O(N) is easy in the sense
that you can do it on a whiteboard via pure analysis. Complexity bugs are fun and straightforward to teach, so that’s what’s
taught. But how do you take an existing program from 2N to
1N? How do you know what the coefficient even is? (Just how
high is that mountain, anyway? Will you clear it?)

Here, the Creator Bias kicks in again. Why not just analyze
the program more deeply? I’m smart; coefficients don’t sound
that hard. The only problem with this approach is that you have
to throw in everything: the language, the compiler that imple-
ments the language, the operating system and the hardware, all
the data, and a lot more.

Imagine two computers with identical software, configuration, 
environmental conditions, and hardware specs. The only
difference is that one has four 4GB memory chips and the other
has one 16GB chip. Under many –but not all– workloads there
will be a measurable difference in the throughput of these two
systems. Even if you understand why that can happen, your
guess is as good as mine (ie, useless) as to what the actual 
difference will be. It depends on every other aspect of the system.

The more detailed you make a model of a program, the
more it becomes a slow, buggy simulation of that program. It
doesn’t matter how smart you are; it’s a direct consequence of
the Halting Problem. That’s what Turing equivalence *means*.
That’s why being good at programming requires being good at
playing computer. So you have to ask yourself a serious question:
who’s better than you at playing computer? Right. The
computer.

In other words, learn to trust your instruments. If you want
to know how a program behaves, your best bet is to run it and
see what happens.

Even with measurements in hand, old habits are hard to
shake. It’s easy to fall in love with numbers that seem to agree
with you. It’s just as easy to grope for reasons to write off
numbers that violate your expectations. Those are both bad, common
biases. Don’t just look for evidence to confirm your theory. 
Test for things your theory predicts should *never* happen.
If the theory is correct, it should easily survive the evidential
crossfire of positive and negative tests. If it’s not you’ll find out
that much quicker. Being wrong *efficiently* is what science is all
about.
```

From Hamming's "it is better to do the right problem the wrong way than the wrong problem the right way":

```markdown
If you follow all the rules, measure carefully, etc, and it still
doesn’t work, it’s possible that your problem definition isn’t just
falsifiable, it’s *false*. You might be measuring the wrong thing,
or optimizing the wrong layer of the stack, or misled about the
root cause.
```

A particularly striking real-world example is what happened to Facebook's HHVM team:

```markdown
HHVM is a virtual machine for the PHP programming lan-
guage. Some of the time it runs bytecode that is dynamically
generated (“just-in-time” aka JIT), but most of the time is spent
running precompiled C++ code. The implementation wasn’t
completely settled, but there were legitimate reasons for mak-
ing performance a feature.

They started off with a reasonable problem definition, sim-
ilar to the one we used for WidgetFactoryServer. Just find the
functions that consume the most CPU time and optimize them.
But things didn’t work out the way they expected.

Keith Adams:

	HHVM today is about three times faster than it was a year ago.
	Then, as now, it spent about 20% of time in the JIT output, and
	about 80% in the C++ runtime.

	The great mystery for you to ponder, and I would hope for your
	book to explain, is that we got three times faster by focusing
	our optimization efforts on the code that was executing for
	20% of the time, not 80% of the time. Go back and reread
	that.

	When you internalize that this sort of thing really happens, in
	real programs that you're responsible for, and that we're not
	talking about pocket change, but a 3x difference in performance,
	it is scary.

	Learning which functions the CPU cycles are being spent on
	can actively deceive you about what to optimize. The advice
	we give intermediate programmers about "premature optimiza-
	tion" and allowing profiling to drive your optimization efforts is,
	well, untrue. Or rather, it's a heuristic that helps compensate
	for even more dangerously wrong optimization impulses.

So, what happened? How could they get huge wins out of
ignoring the proverbial 80%? Because the minority code had in-
direct influence on the rest. Changes to the JIT code, nomi-
nally responsible for only 20% of CPU time, caused random,
outsized performance effects throughout the system.

To understand why, remember that a computer really does
only two things: read data and write data. Performance comes
down to how much data the computer must move around, and
where it goes. Throughput and latency *always* have the last laugh.
This includes CPU instructions, the bits and bytes of the program, 
which we normally don’t think about.

The kinds of computers in use today have four major levels
of “where data goes”, each one hundreds to thousands of times
slower than the last as you move farther from the CPU.

• Registers & CPU cache: 1 nanosecond
• RAM: 10^2 nanoseconds
• Local drives: 10^5 to 10^7 nanoseconds
• Network: 10^6 to 10^9 nanoseconds

Memory controllers try mightily to keep the first level pop-
ulated with the data the CPU needs because every cache miss
means your program spends 100+ cycles in the penalty box.
Even with a 99% hit rate, most of your CPU time will be spent
waiting on RAM. The same thing happens in the huge latency
gap between RAM and local drives. The kernel’s virtual memory
system tries to swap hot data into RAM to avoid the speed
hit of talking to disk. Distributed systems try to access data
locally instead of going over the network, and so on.

HHVM was essentially “hitting swap” on the CPU. Actual
machine code is data too, and has to be on the CPU in order to
execute. Some JIT code would copy over and execute, pushing
other stuff out of the CPU caches. Then it would pass control
over to some function in the C++ runtime, which would not be
in the cache, causing everything to halt as the code was pulled
back out of RAM. Figuring this out was not easy, to say the
least.

Keith Adams again, on cache effects:

	Cache effects have a reputation for being scarily hard to reason
	about, in part because caches of all kinds are a venue for spooky
	action-at-distance. The cache is a stateful, shared resource that
	connects non-local pieces of your program; code path A may
	only be fast today because the cache line it operates on stays
	in cache across lots of invocations.

	Making a change in unrelated code that makes it touch two
	lines instead of one can suddenly cause A to take a miss every
	time it runs. If A is hot, that "innocent" change becomes a
	performance catastrophe.

	More rarely the opposite happens, which is even more frustrating,
	because of how clearly it demonstrates that you don't understand
	what determines performance in your program. Early
	on in development Jordan DeLong made an individual checkin,
	only affecting the JIT, that was a 14% (?!!) performance win
	overall.

The surface problem was CPU time. But most of the time
wasn’t actually going to computation (ie, moving data around
inside the CPU) it was spent fetching data from RAM into the
CPU. Worse was that normal profiling, even advanced stuff like
VTune and the Linux “perf ” kernel module, weren’t very useful. 
They will happily tell you what functions suffer the most
cache misses. But they don’t tell you why the data wasn’t there.
```

So how did the HHVM team solve the issue?

```markdown
The team had to come up with a different problem definition,
which went something like this:

	CPU time in HHVM is dominated by CPU cache
	misses. If we somehow log both the function which
	suffered a cache miss and the function which replaced
	the data that was missed, we may find that a
	small number of functions cause most of the
	evictions. If we optimize those to use less cache space,
	we expect to see a reduction in both cache misses
	and CPU time spent across the board.

That’s a mouthful, but it worked. To prove this theory they
ended up gathering very expensive and detailed logs, for exam-
ple, every datum accessed or CPU instruction executed. They
then fed that through a cache simulation program, and modified
the simulator to record the causal path from evictor to
evictee, so they knew what functions to blame. Sort the list to
find the worst offenders and optimize them. Not easy, but a lot
more straightforward.
```

"An internet app is more like a power plant than a design for a toaster" is how Carlos essentially sums up Facebook's rapid iterating on live data, an approach other companies are beginning to adopt -- I try to do the same for my reports actually, but this philosophy is a tough sell since it isn't really what management wants:

```markdown
In the age of the personal computer, software was made the
way toasters (and pesos and centavos) are: lots of design up
front, stamped out by the million, then sent off into the world to
fend on their own. It was nearly impossible to get representative
performance data from the field. On the other hand, any copy
was as good as any other. If you made your copy run faster
it would probably run faster everywhere. That is, when and if
everybody upgraded to the newest version.

The other kind of software became dominant again 10 or
15 years ago. An internet app is more like a power plant than
a design for a toaster. It’s a unique, complicated artifact woven
into a global network of other unique, complicated artifacts,
half of them human beings.

Being able to give everyone the same version of your software at 
the same time was the killer feature of the internet.
It’s why we threw out decades of software and infrastructure
and rewrote it inside the browser. But this new (old) model has
other important consequences. To understand them, it’s possible we
should rely less on computer science and more on operations 
research and process control.

When a major component of your system is the entire world
and the people in it, you can’t really put a copy on the bench
and test it out. On the other hand, getting live data and iterating
on what you learn has never been easier. Instead of “versions”
rolled out every year like cars, you constantly push out smaller
changes and measure their effects.

Spot checks and benchmarks aren’t enough in this model.
If something is important enough to worry about, it’s important
enough to measure all the time. You want a continuous,
layered measurement regime. This makes it easy to run performance
experiments in the same way that automated testing
makes it easier to catch errors. It also removes a dependency on
clairvoyance. If you happen to neglect to measure something
you should have, it’s not a disaster. You can start measuring
it tomorrow. Flexibility in the instrumentation and analysis is
key.

Most interestingly, a networked application follows cycles.
Think for a moment about what it means to run a power plant.
During the wee hours of the morning draw is low. Then people
wake up. Alarm clocks and radios turn on (all at the same
minute), then the electric ranges, office buildings, and factories.
Elevators start running. People move from one part of the city
to another and start using electricity there. School bells ring.
Thermostats are tuned to the weather. If you were to chart a
week of power draw, it would look something like this:
(think weekly periods for revenue fluctuations)
```

Computers are onions, or alien artifacts:

```markdown
A good measurement regime is built up in layers. Avoid the
temptation to measure the first thing that comes into your head,
because it won’t be random. It’ll be the thing you feel you under-
stand best, but our feelings are probably wrong. We opti-
mize what we measure. Some things are easier to measure than
others, so those tend to be optimized too much.

Forget for a moment that you built the thing and start from
first principles. Pretend you are examining an alien artifact that
just fell out of the sky. You want to discover how it performs.
Not how it *works8, how it *performs*. What does it consume?
What does it output? Where does that happen? A good place
to start is with basic “temperature and pressure” logs of the
system. Then you add more detailed logging to help zero in
on the hot spots. It’s a process of recursively subdividing mea-
surements to find concentrations of precious resources being
consumed.

Your instrumentation should cover the important use cases
*in production*. Make all the measurements you want in the lab,
but nothing substitutes continuous real-world data. Think about
it this way: optimizing based on measurements you take in a lab
environment is itself a falsifiable theory, ie, that lab conditions
are sufficiently similar to production. The only way to test that
theory is to collect measurements in production too.
```

Storing data and measurements:

```markdown
Our friends in the physical sciences have it worse. A thermometer 
can’t actually measure the temperature at a given point
in time. Heat takes time to transfer so a thermometer can only
give the average temperature over some period. The more sensi-
tive the measurements desired, the more the equipment costs.
And there is always a lag.

You and I can make as many discrete (and discreet) measurements 
as we want. We can even *change* what measurements
are done on the fly based on complex logic. And, of course,
we know how to handle large amounts of data. So why do we
throw the stuff away?

Look at the documentation for a popular
measurement system like RRDtool:

	You may log data at a 1 minute interval, but you might also be
	interested to know the development of the data over the last
	year. You could do this by simply storing the data in 1 minute
	intervals for the whole year. While this would take considerable
	disk space it would also take a lot of time to analyze the data
	when you wanted to create a graph covering the whole year.

	RRDtool offers a solution to this problem through its data conso-
	lidation feature. Using different consolidation functions (CF) 
	allows you to store exactly the type of information that actually
	interests you: the maximum one minute traffic on the LAN, the
	minimum temperature of your wine cellar, the total minutes of
	down time, etc.
	
This approach is dead wrong, and not because of its breezy
claims about performance.Why do we force ourselves to guess
every interesting metric in advance? To save disk space? Com-
puting aggregates then throwing away your raw data is premature
optimization.

In exchange for that saved space, you have created a hidden
dependency on clairvoyance. That only works if all you will
ever need to know is the “maximum one minute traffic”. If later
on you want to know what the average traffic was, or the 95th
percentile, or grouped by protocol, or excluding some hosts, or
anything else, you can’t.

Making sense of a pile of data is a multidimensional search
problem. We’re programmers. We know how to handle search
problems. The key is being able to freely jump around those
dimensions. It’s not possible to predict ahead of time the aggre-
gate metrics, the search paths, you’ll want to use later on.
Storing all the raw data can be expensive, but on the other hand
the combinatorial explosion of all possible metrics that can be
derived from it is much larger. On the third hand, the usefulness
of raw data drops off sharply as it ages.

There is a way to redefine the problem. What’s happening
is a clash between two use-cases. New data needs to be in a
“high-energy” state, very fluid and explorable. Old data can be
lower-energy, pre-aggregated, and needs to be stable over long
periods of time.

So, store raw performance data in a very fast database, but
only for the last few weeks or months. You can explore that raw
data to discover the metrics you care about. *Then* you render it
down to those road-tested metrics and shove them into RRD
or whatever else you want for long-term storage. A buffer of
recent raw data to help you diagnose novel problems, and stable
historical records so you can track how well you’re doing.
```

This makes me understand what my supervisor does!

A pragmatic measurement-driven approach to data modeling, extremely relevant to work:

```markdown
The long-running doctrinal disagreement between relational
entity modeling (third normal form, OLTP, etc) and dimen-
sional modeling (star schemas, data warehousing, OLAP, and
so forth) is largely about the number of table joins needed 
to accomplish the task of analysis. In other words, it’s an
argument over performance.

Well, we know what to do about arguments over performance. 
“Define the problem and measure” applies just as much
to the systems you build for measurement. The flat table struc-
ture described above is at the extreme of trading space for time:
there are zero joins because all the metadata are attached to the
sample. It’s a starting point, but one that can take you a long,
long, long way.

As your measurement system scales up you will likely not
want a totally flat design that attaches obscure metadata like the
the server’s chipset, model number, rack id, etc to every sample.
Instead you might add a small lookup table to the database and
join on it, or implement some kind of dictionary compression.
The point is that complicating your schema is an *optimization*
to be done when the need arises, not because of data model
orthodoxy. Don’t overthink it.
```

Yardsticks vary, and this screws up decisions:

```markdown
The people in the hardware store must have thought my father 
was crazy. Before buying a yardstick, he compared each
one to a yardstick he brought with him. It sounds less crazy
when you learn he’s found differences of over 1/4 inch per yard,
something like 1%. That’s a big deal when you are building. It’s
even worse when you aren’t aware there’s a problem at all.

The yardstick’s reputation is so strong that we use it as a
metaphor for other standards, eg the “yardstick of civilization”.
The entire point of their existence is that they should all be the
same size. How could anyone manage to get that wrong? Well,
manufacturing tolerances drift. Yardsticks are made from other
yardsticks, which are made from others, and so on back in time.
Errors propagate. Measurement is trickier than it appears.

The root cause is that no one bothered to check. Measurement 
software is just as likely to have bugs as anything else we
write, and we should take more care than usual. A bug in user-
facing code results in a bad experience. A bug in measurement
code results in bad *decisions*.

There are simple checks you can do: negative numbers are
almost always wrong. One kind of mistake, which would be
funnier if it didn’t happen so often, is to blindly record a CPU
or walltime measurement of 1.3 billion seconds.6 Other checks
are possible between measurements. CPU time should never
be greater than walltime in a single-threaded program, and the
sum of component times should never be greater than the overall
measure.

Even better is to log something in two different ways, to
bring your own yardstick to the hardware store. To a programmer, 
having two systems that measure the same thing is duplicated work.
To an experimentalist that’s just independent confirmation. The 
more ways you can show something to be true the more likely it *is* 
true. The second log doesn’t have to be fancy. Your database 
probably has enough statistics built in that you can monitor 
periodically and compare with your logs.
```

Names matter, because you have to deal with your choices for a long time (see also [names matter](#names-matter)):

```markdown
Naming things has been half-jokingly called the second-hardest
problem in computer science. Anyone can name the things they
build anything they want, and they do. That’s the problem. The
computer doesn’t care about names. They’re for the benefit of
humans so there are no technical arguments to fall back on.
Excess jargon is the sawdust of new technology, and the mental
friction it imposes is scandalous. Whoever figures out how to
sweep it up does a service to mankind.

Take the word we’ve been using for intervals of real time,
“walltime”. Perhaps it’s more properly called “duration”. Time
spent on the CPU could be called “cpu_duration”; time spent
waiting for the database “db_duration” and so on. And why
not be explicit about the units, eg “duration_cpu_usec”? If you
have a strong preference either way, I humbly suggest that it’s a
matter of taste and not universal truth. Walltime sounds more
natural to me because that was the jargon I was first exposed
to. But who actually has clocks on their walls any more? The
term is as dated as “dialing” a phone number.

For that matter, take instructions. Now that we’ve decided
to round to the nearest thousand, is the name “instructions”
misleading? Is “kilo_instructions” too cumbersome to type? Is
“kinst” too obscure to remember?

This all might sound mincing and pedantic, but a) you have
to pick something and b) you’ll have to deal with your choices
for a long time. So will the people who come after you. You
can’t clean up the world but you can mind your own patch.

Even an ugly scheme, if it’s consistently ugly, is better than
having to remember that walltime here is duration over there
and response_time_usec somewhere else. Whatever ontology
you build, *write it down* somewhere it will be noticed. Explain
what the words mean, the units they describe, and be firm about
consistency
```

I like "you can mind your own patch". Agrees with Scott Alexander's "I just want to tend to my little walled garden". 

Don't overload with visualizations:

```markdown
This might appear counterintuitive, but the fewer types of vi-
sualizations you add to your tool, the better off you’ll be. 
Remember that the goal is not pretty pictures, it’s insight.
A visualization tool should first focus on the fluidity of exploration,
which in turn depends on the composability of its features. A
dataset with ten metadata columns can be thought of as a ten-
dimensional space, with one or more measurements residing
at the points. Helping the user navigate and collapse that space
is the primary task.

The main activities are to describe trends, show the distribution
of a set of samples, to compare sets of samples, and to
find correlations between dimensions. As a general principle,
if you ever catch yourself doing mental arithmetic, or pointing
to two spots on a graph, or (worse) two separate graphs, that
means your tool is missing a feature.

Start with a raw table view. All metadata and measurement
columns are visible, and each row is a raw sample. The first
feature should be the ability to hide the columns that are un-
important to the question being asked. The second feature is to
group rows together by the values in the metadata columns.
The third is to compute aggregate metrics (counts, averages,
percentiles) over the grouped measurements. The fourth is to
overlay two tables on top of each other and calculate the diff-
erences in each cell. This allows you to compare the performance
of two datacenters, or versions of the software, or anything else.
```

Design for chains of reasoning:

```markdown
Another general principle is to design for chains of reasoning, not
just individual views of the data. In the course of finding the
answer to a question, it’s very likely the user will need to run
multiple queries, perhaps narrowing down a previous query, or
rotating along another dimension or metric, or even backtracking
several steps.

The system should be built around the idea of handling the
combinatorial explosion of possible metrics and views on the
data. Only a few of those views are important, and the raw
data ages out relatively quickly. So every query that a human
actually looks at is probably special and should be saved: not
just the description of the query, but the actual data. If you do
it right, this would cost at most a few tens of kilobytes per. Give
each saved view a short, unique URL they can share around.
Collections of those views are a record of a chain of reasoning.

That’s a fancy way of saying “permalink”, and it’s nothing
novel. The ideas in this chapter are only examples. To get the
most out of your hard-won data, apply modern user-experience
design to the task at hand. If the effort is worth it for your users’
experience, it’s worth it for yours
```

How to, and how not to, design good dashboards -- remember they're for monitoring, not diagnosis:

```markdown
Whether you call them greenboards, or gauges, or blinkenlights,
or heads-up displays, a dashboard is the main fusebox of your
system. The metrics on the board should reflect your under-
standing of how the system behaves and misbehaves.

The dashboard is a really good place to apply that trick of
stating theories in terms of what they predict *won’t* happen. 
Finish the following sentence by filling in the blanks:

	While the system is operating normally, the ___
	graph should never ___ .
	
There will be several good answers, and they will tend to
be fundamental things like network traffic, CPU utilization,
and transaction volume. Those answers, expressed as graphs
on your dashboard, should function like electrical fuses: sim-
ple, robust, and not prone to false positives or negatives. A fuse
popping conveys only one bit of information, but it’s an important
bit, and almost always a cause for action.

It’s a common mistake to overload your dashboard with too
much information. The fanciest hospital monitor can describe
something as complex and important as a living being with less
than ten metrics. *While the human is operating normally, the heart
rate graph should never change drastically, go below 60, or above 100*.
You can do the same with a computer system. A dashboard is
for monitoring, not diagnosis. It’s only job is to tell you that
something is wrong, and give a rough clue about where to look
next.

That’s not to say you can’t have lots of graphs. It’s fine to
have lots of graphs, say memory pressure and CPU, one for every 
server. What you don’t want is too many metrics, too many
*kinds* of graphs, confusing the separate duties of monitoring and
diagnosis.
```

Building hierarchies of failure modes to facilitate reasoning-chains-debugging:

```markdown
Over time you build up knowledge about failure modes. Any
time an incident is solved using a non-standard metric, or view,
or filter, or what-have-you it should added to a diagnosis tool,
which is essentially a lookup table for common paths taken during
diagnosis. Here are some metrics that are probably relevant
to any large networked application:

	• Error rates
	• Latency (average, median, low and high percentiles)
	• CPU Time / Instructions
	• Network bytes in & out
	• Requests per second
	• Active users
	• Active servers
	• Server utilization (CPU, RAM, I/O)
	• Database queries
	• Cache hit / miss rates

Never mind that you’ve already filled up a giant display and
I’ve surely missed something important. These metrics should
be further broken down by country, datacenter, WWW versus
API versus mobile, and a half-dozen other dimensions.

Sketch them all out on a big piece of paper or whiteboard,
then start to group them into hierarchies. Animal, vegetable, or
mineral? What metrics lead to other metrics during diagnosis?
How should they be linked? If you could “zoom in” on the
data like an interactive map, which small things should become
larger? Which metrics assure the accuracy of others?

	When the ___ is operating abnormally, the ___
	graph can eliminate ___ as a possible cause.
	
This “diagnosis tool” is something in between the sparse
top-level dashboard and the free-for-all malleable dataset we’ve
built in this book. The minimum possible form it could take is a
collection of links to views on the data that have proven useful
in the past. There’s a good chance you have something like this
already. Whether it’s in your head, your browser’s bookmarks,
or your operations runbook, take the time to curate and share it
with everyone on your team. It embodies most everything you
know about the real behavior of your system.
```

Beware static thresholds:

```markdown
The most powerful tool of the computer programmer is the
computer itself, and we should take every chance to use it. The
job of watching the graphs is important but time-consuming
and errorful. The first instinct of any programmer who has had
that duty is automation. The second instinct is usually to solve
it with thresholds, eg 1,400 msec for walltime, and trigger an
alarm or email when a threshold is crossed.

For every difficult problem there is a solution which is simple, 
obvious, and wrong. Red lines, pressure gauges, and flashing lights
are familiar movie tropes that create an air of urgency
and importance. But, considering everything else Hollywood
writers get wrong about computers, we should think very carefully
about taking design cues from them.

Alert readers will notice three problems with static thresholds. 
First, a dependency on clairvoyance snuck in the back
door: how do you decide what number to use? Second, there’s
only one number! The performance characteristics of internet
applications vary hour-by-hour. The third problem is more subtle: 
you probably want to know when the metric you’re watching falls 
below the expected range, too.

Static thresholds do make sense when making promises about
your system to other people. Service Level Agreements (SLAs)
often include specific response time promises, eg “The API will
always respond in less than 500 msec”. But that’s business, not
science. Declaring an acceptable limit doesn’t help you learn
what actually happens. You can’t have anomaly detection without 
first discovering what defines an anomaly.
```

Okay, so how *do* I do anomaly detection properly?

```markdown
The simplest way to get the job done is to choose a handful
of metadata and measurements that tend to have the most impact 
on performance. Time is the first and most obvious one.
Then comes the transaction type (eg script_path), the machine
or group of machines (host, datacenter), the version of the soft-
ware (build_number) and so on. For each combination of those
dimensions, create a few metrics that characterize the perfor-
mance envelope: say, the 25th, 75th, and 99th percentiles of
walltime and cpu_time. You want the same kind of information that
is on your dashboard, just more of it.

Given those metrics you can determine what values are “normal” for
various times of the day by looking at historical data.
If the 99th percentile walltime for /foo.php between 2:20PM
and 2:40PM for the last few Wednesdays was 455 msec, then
throw an alarm if this Wednesday at 2:25pm the metric deviates
too much from what the data predicts, on a percentage basis or
something fancier like the root mean square error.
How much is too much? You can run experiments to discover how
many alarms would have been thrown for a given
range. Hold back one day (or week) of historical data from the
learning set and run your detection code over it. How much
noise you’re willing to put up with is up to you.
```

Feedback loops are hard, especially for distributed systems! Proceed with caution:

```markdown
Sooner or later, someone on your team is going to try to
feed a system’s performance data back into itself, and teach it
to react. This is simultaneously a wonderful and terrible idea,
fully into the realm of control theory.

The general technique has been around for ages. The float
in a toilet tank, which raises with water level and controls the
flow of water in, works on the same principle. In the graphics
world, closed loop calibration is used to make sure what you
see on a monitor is what you get on the printer. Every serious
measurement device has calibration designed into it.

There are good places and bad places for this sort of advanced 
nerdery. Aside from general correctness, feedback loops
for distributed computer systems come with three hard problems 
you have to solve: reaction time, staircase mode, and oscillation.

**Reaction time** means how quickly the entire system can react
to changes in the feedback it’s collecting. Gathering 5 minutes’
worth of data will obviously limit your loop’s reaction time to
five minutes, unless you calculate some kind of moving average. 
There is also propagation delay: we like to pretend that
state changes happen in an instant. But the more computers
you have, the less and less that’s true.

**Staircase mode** is a quality you want to design for. Elevators
don’t have great failure modes. Escalators, on the other hand,
never really break. They just become staircases. When your
feedback loop fails, and it will, think about whether it becomes
a staircase or a death trap.

**Oscillation** happens when one or more components overcompensate.
Think of those awkward moments when you and someone walking in 
the opposite direction get in each other’s way.
You step to one side but a fraction of a second later they do
too. So you step the other way, but before you can react they
follow, etc.
```

Categories of system performance bottlenecks:

```markdown
There seem to be two rough categories of bottleneck. Incidental
bottlenecks tend to be isolated and fixable without much fuss.
Even if they require a lot of clever work to implement, they
don’t threaten to upend the basic premises of your design, and
their magnitudes can be large. This is the happy case. I wish
you a long career of easy wins from this end of the spectrum.

Fundamental bottlenecks are harder to fix, and harder to
see, because they are caused by some fact of nature or an assump-
tion the system is built around. An infinitely-fast network
application is still subject to the speed of light. A pizza shop’s
fundamental bottleneck is the size of its oven. Rockets are limited
by the need to lift the weight of their own fuel.
```

Related -- why might you be better off shrinking your system response time's variance, even if it bumps up the average?

```markdown
Shrinking the variance of your system’s response time, even
if it makes the average slower, is a huge win that spreads good
effects all over the place. It makes load balancing that much eas-
ier because units of work are more interchangable. It reduces
the possibility of server “spikes”, temporary imbalances, filled
queues, etc etc and so forth. If you could magically optimize a
single metric in any system, it should be the standard deviation.
```

<a name="#Software-complexity"></a>
## Software complexity
([overview](#overview)) 

See also [complex systems](#complex-systems).

<a name="#The-many-faces-of-Software-complexity"></a>
### The many faces of software complexity
([overview](#overview)) 

Eric Raymond's [The Art of Unix Programming](http://www.catb.org/esr/writings/taoup/html/index.html) has lots of gems. Here's some quotes from his page [Speaking of Complexity](http://www.catb.org/esr/writings/taoup/html/ch13s01.html), in *Chapter 13: Complexity*, where he introduces a 3x3 matrix for classifying various kinds of software complexity (yep, not just your average consultant 2x2 matrix, a *3x3* matrix!! Gosh!?!). 

The impetus behind writing the chapter:

```markdown
As with previous issues about modularity and interface design, Unix programmers react 
to a set of distinctions they have often learned from experience without knowing how 
to articulate. Therefore we'll need to start by developing some terminology.

We will start by defining what software complexity is. We will make some *horizontal* 
distinctions between different flavors of complexity, which sometimes have to be traded
off against each other. 

We will finish by making some even more important *vertical* distinctions, between the 
kinds of complexity we must live with and the kinds we have the option to eliminate.
```

Why does complexity matter so much? 

```markdown
Underlying the Unix programmer's passion for simplicity is a pragmatic fact: complexity
costs. Complex software is harder to think about, harder to test, harder to debug, and 
harder to maintain — and above all, harder to learn and use. The costs of complexity, 
rough as they are during development, bite hardest after deployment. Complexity creates
places for bugs to nest, from which they will emerge to trouble the world through the 
entire lifetime of their software.
```

Sources of complexity -- implementation, interface, codebase size (correlates with bugcount):

```markdown
So what exactly do we mean by ‘complexity’? This point is worth pinning down, because
it varies by observer.

Unix programmers (like other programmers) tend to focus on *implementation* complexity — 
basically, the degree of difficulty a programmer will experience in attempting to 
understand a program so he or she can mentally model or debug it.

Customers and users, on the other hand, tend to see complexity in terms of the program's
*interface* complexity. In Chapter 11 we discussed the quality of ease and its inverse, 
mnemonic load. To a user, complexity correlates closely with mnemonic load. Poor 
expressiveness and concision can matter too, if a weak interface forces the user to 
perform lots of error-prone or merely tedious low-level operations rather than a few 
high-level ones.

Driven by both of these is a third measure that is much simpler: the total number of lines
of code in the system, its *codebase size*. In terms of life-cycle costs, this is usually the
most important measure. The reasons go back to perhaps the most important empirical result
in software engineering, one we've cited before: the defect density of code, bugs per
hundred lines, tends to be a constant independent of implementation language. More lines 
of code means more bugs, and debugging is the most expensive and time-consuming part of 
development.
```

In attempts to avoid them, software designers commonly fall into a number of traps, which result from the fact that sometimes these measures need to be traded off against one another. Here are the three main ones:

```markdown
We've already mentioned one situation in which two measures vary in opposite directions:
a user interface that has been designed primarily to preserve implementation simplicity,
or keep codebase size down, may simply dump low-level tasks on the user. (A crude example
of this, barely imaginable to a Unix programmer but all too common elsewhere, might be 
an editor that lacked a global-replace feature.) Though this sort of design failure is 
all too common, it does not traditionally have a name. We'll call it a *manularity trap*.

Pressure to keep the codebase size down by using extremely dense and complicated 
implementation techniques can cause a cascade of implementation complexity in the system,
leading to an un-debuggable mess. This used to happen frequently when fitting programs onto
very small systems demanded assembler programming or tricks like self-modifying code; 
nowadays it is uncommon except in embedded systems, and rapidly becoming rare even there. 
This kind of design failure doesn't have a traditional name, but one might call it a *blivet
trap*, after an old Army term for the results of attempting to stuff ten pounds of horse 
manure into a five-pound bag.

The blivet trap won't appear in our case studies, but we've defined it for contrast with
its opposite. It can happen that the designers of a project are so wary of implementation
complexity that they reject a complex but unified way to solve a whole class of problems 
in favor of lots of duplicative, ad-hoc code that solves each individual one in turn. The
result is bloat in the size of the codebase, and maintainability problems more severe than
if the unified method had been accepted. For example, a Web project that really needs a
centralized relational database behind its pages might instead spawn several different 
keyed data files containing information that has to be reintegrated at page generation time. 
This sort of failure is all too common. It doesn't have a traditional name; we'll call it 
an *adhocity trap*.
```

I really like Eric's discussion on the tradeoff between interface and implementation complexity:

```markdown
One of the most perceptive observations ever made about the Unix tradition by someone 
standing outside it was contained in Richard Gabriel's paper called Lisp: Good News,
Bad News, and How to Win Big. Gabriel is a long-time leader of the Lisp community, and
the paper was primarily an argument for a particular style of Lisp design, but the 
author himself acknowledges that it is now remembered primarily for the section called 
‘The Rise of Worse Is Better’.

The paper argued that Unix and C have the characteristics of viruses, and that in the
evolutionary struggle among software designs traits like implementation simplicity and
portability which lead to rapid propagation (infectiousness) are more effective than 
correctness and completeness of the design. ... 

Less remembered is that the Gabriel's central argument was about a very specific tradeoff 
between implementation and interface complexity, one which rather exactly fits the
categories we have examined in this chapter. Gabriel contrasts an ‘MIT’ philosophy most 
valuing interface simplicity with a ‘New Jersey’ philosophy most valuing implementation 
simplicity. He then proposes that although the MIT philosophy leads to software that is 
better in the abstract, the (worse) New Jersey model has better propagation characteristics. 
Over time, people pay more attention to software written in the New Jersey style, so it 
improves faster. Worse becomes better.

One epochal example not mentioned in Gabriel's paper is from distributed hypertext systems.
Early distributed-hypertext projects such as NLS and Xanadu were severely constrained by 
the MIT-philosophy assumption that dangling links were an unacceptable breakdown in the user
interface; this constrained the systems to either browsing only a controlled, closed set of
documents (such as on a single CD-ROM) or implementing various increasingly elaborate 
replication, caching, and indexing methods in an attempt to prevent documents from randomly
disappearing. Tim Berners-Lee cut through this Gordian knot by punting the problem in classic
New Jersey style. The simplicity of implementation he bought by allowing “404: Not Found” as
a response was what made the World Wide Web lightweight enough to propagate and succeed.

We cannot offer a one-size-fits-all answer. As with most of the large questions in this 
chapter, good taste and engineering judgement will demand different answers in different 
situations. The important thing is to develop the habit of thinking carefully about this 
issue on each and every one of your designs. As we have observed before in discussing 
software modularity, complexity is a cost you must budget very carefully.
```

Orthogonal to the sources of complexity are the *kinds* of complexity -- essential, accidental, and optional:

```markdown
One of the unfortunate things about reality is that it often poses complex problems 
that demand complex solutions. You can't control a jetliner with an elegant ten-line
procedure. There are too many pieces of equipment, too many channels and interfaces, 
too many different processors — too many different subsystems defined by independently
operating human beings who often don't agree even on fundamental conventions. Even if 
you are successful at making all the individual software parts of an avionics system 
elegant, integration is likely to produce a large, complex, and grubby body of code 
with (one hopes) the single virtue that it will actually work.

Jetliners have *essential* complexity. There is a rather sharp point past which it's not 
possible to trade away features for simplicity, because the plane has to stay in the 
air. Because of that very fact, avionics control systems do not tend to spawn religious
wars about complexity — and Unix programmers tend to stay away from them.

To sharpen our vision, we need to begin by noticing a difference between accidental 
complexity and optional complexity. *Accidental* complexity happens because someone didn't 
find the simplest way to implement a specified set of features. Accidental complexity 
can be eliminated by good design, or good redesign. *Optional* complexity, on the other 
hand, is tied to some desirable feature. Optional complexity can be eliminated only by 
changing the project's objectives.

When we fail to distinguish between optional and accidental complexity, design debates
become seriously confused. Questions about what a project's objectives are get confused
with questions about the aesthetics of simplicity, and whether people have been 
sufficiently clever.
```

Examples of each:

```markdown
• Accidental interface complexity often comes from non-orthogonality in the interface 
design — that is, failing to carefully factor the interface operations so that each does
exactly one thing
• Accidental code complexity (making code more complicated than it needs to be to get the
job done) often results from premature optimization
• Accidental codebase bloat often results from violating the SPOT rule, duplicating code 
or organizing it poorly so that opportunities for reuse aren't recognized.

• Essential interface complexity usually can't be cut without trimming the basic functional
requirements for the software
• Essential codebase size is related to choice of development tools because, if the feature
list is held constant, the most important factor in codebase size is probably the choice of
implementation language

Sources of optional complexity are the most difficult to make useful generalizations about,
because they so often depend on delicate judgments about which features it is worth paying
the complexity cost for:

• Optional interface complexity often comes from adding convenience features that make life
easier for users but aren't essential to the function of the program
• Optional increases in codebase size (supposing the user-visible features and the algorithms
used are held constant) can often come from various sorts of practices intended to make it 
more maintainable — adding mode comments, using long variable names, and so forth
•  Optional implementation complexity tends to be driven by *everything* that touches a 
project
```

So how to deal with these kinds of complexity?

```markdown
The sources of complexity have to be grappled with in different ways. Codebase size can be
attacked with better tools. Implementation complexity can be addressed with better choice 
of algorithms. Interface complexity has to be addressed with better interaction design, a
skill involving considerations of ergonomics and user psychology. This skill is less common
(and possibly more difficult) than writing code.

Attacking the kinds of complexity, on the other hand, has to be done more with insight than
with methods. You cut accidental complexity by noticing that there is a simpler way to do 
things. You cut optional complexity by making context-dependent judgments about what 
features are worthwhile. You can only cut essential complexity by having an epiphany, 
fundamentally redefining the problem you are addressing.
```

<a name="#You-cannot-write-a-better-Google-in-a-weekend"></a>
### You cannot write a better Google in a weekend
([overview](#overview)) 

From Dan Luu's essay [I could do that in a weekend!](https://danluu.com/sounds-easy/). Dan happens to be [the lemons guy](https://slatestarcodex.com/2017/11/30/book-review-inadequate-equilibria/) in Eliezer Yudkowsy's *Inadequate Equilibria*. Ties to software-at-scale, complex systems in general, and [reality being surprisingly detailed](https://github.com/monastri/monastri.github.io/blob/master/notes-philosophy-erisology-altruism-culture-spirituality.md#Reality-has-a-surprising-amount-of-detail). 

Why are these people wrong?

```markdown
Businesses that actually care about turning a profit will spend a lot of time
(hence, a lot of engineers) working on optimizing systems, even if an MVP for
the system could have been built in a weekend. There's also a wide body of 
research that's found that decreasing latency has a roughly linear effect on
revenue over a pretty wide range of latencies for some businesses. Increasing
performance also has the benefit of reducing costs. Businesses should keep 
adding engineers to work on optimization until the cost of adding an engineer
equals the revenue gain plus the cost savings at the margin. This is often 
many more engineers than people realize.

And that's just performance. Features also matter: when I talk to engineers 
working on basically any product at any company, they'll often find that there
are seemingly trivial individual features that can add integer percentage points
to revenue. Just as with performance, people underestimate how many engineers 
you can add to a product before engineers stop paying for themselves.

Additionally, features are often much more complex than outsiders realize. If 
we look at search, how do we make sure that different forms of dates and phone
numbers give the same results? How about internationalization? Each language has
unique quirks that have to be accounted for. In french, “l'foo” should often 
match “un foo” and vice versa, but American search engines from the 90s didn't 
actually handle that correctly. How about tokenizing Chinese queries, where words
don't have spaces between them, and sentences don't have unique tokenizations? 
How about Japanese, where queries can easily contain four different alphabets? How
about handling Arabic, which is mostly read right-to-left, except for the bits 
that are read left-to-right? And that's not even the most complicated part of 
handling Arabic! It's fine to ignore this stuff for a weekend-project MVP, but 
ignoring it in a real business means ignoring the majority of the market! Some of
these are handled ok by open source projects, but many of the problems involve
open research problems.

There's also security! If you don't “bloat” your company by hiring security people,
you'll end up like hotmail or yahoo, where your product is better known for how 
often it's hacked than for any of its other features.

Everything we've looked at so far is a technical problem. Compared to organizational
problems, technical problems are straightforward. Distributed systems are considered
hard because real systems might drop something like 0.1% of messages, corrupt an 
even smaller percentage of messages, and see latencies in the microsecond to 
millisecond range. When I talk to higher-ups and compare what they think they're 
saying to what my coworkers think they're saying, I find that the rate of lost 
messages is well over 50%, every message gets corrupted, and latency can be months
or years. 

	Recently, I was curious why an org that's notorious for producing unreliable
	services produces so many unreliable services. When I asked around about why,
	I found that that upper management were afraid of sending out any sort of 
	positive message about reliability because they were afraid that people would
	use that as an excuse to slip schedules. Upper management changed their 
	message to include reliability about a year ago, but if you talk to individual
	contributors, they still believe that the message is that features are the #1
	priority and slowing down on features to make things more reliable is bad for
	your career (and based on who's getting promoted the individual contributors 
	appear to be right). Maybe in another year, the org will have really gotten 
	the message through to the people who hand out promotions, and in another 
	couple of years, enough software will have been written with reliability in
	mind that they'll actually have reliable services. Maybe. That's just the first-
	order effect. The second-order effect is that their policies have caused a lot 
	of people who care about reliability to go to companies that care more about 
	reliability and less about demo-ing shiny new features. They might be able to
	fix that in a decade. Maybe. That's made harder by the fact that the org is in
	a company that's well known for having PMs drive features above all else. If
	that reputation is possible to change, it will probably take multiple decades.

When people imagine how long it should take to build something, they're often 
imagining a team that works perfectly and spends 100% of its time coding. But that's
impossible to scale up. The question isn't whether or not there will inefficiencies,
but how much inefficiency. A company that could eliminate organizational inefficiency
would be a larger innovation than any tech startup, ever. But when doing the math on 
how many employees a company “should” have, people usually assume that the company is
an efficient organization.

This post happens to use search as an example because I ran across some people who 
claimed that Lucene was going to surpass Google's capabilities any day now, but there's
nothing about this post that's unique to search. If you talk to people in almost any 
field, you'll hear stories about how people wildly underestimate the complexity of the
problems in the field. The point here isn't that it would be impossible for a small 
team to build something better than Google search. It's entirely plausible that someone
will have an innovation as great as PageRank, and that a small team could turn that into
a viable company. But once that company is past the VC-funded hyper growth phase and 
wants to maximize its profits, it will end up with a multi-thousand person platforms org,
just like Google's, unless the company wants to leave hundreds of millions or billions
of dollars a year on the table due to hardware and software inefficiency. And the company
will want to handle languages like Thai, Arabic, Chinese, and Japanese, each of which is
non-trivial. And the company will want to have relatively good security. And there are 
the hundreds of little features that users don't even realize that are there, each of 
which provides a noticeable increase in revenue. It's "obvious" that companies should 
outsource their billing, except that when you talk to companies that handle their own
billing, they can point to individual features that increase conversion by single or 
double digit percentages that they can't get from Stripe or Braintree. That fifty person
billing team is totally worth it, beyond a certain size. And then there's sales, which 
most engineers don't even think of. 

	For a lot of products, the sales team is more important than the engineering 
	team. If we build out something rivaling Google search, we'll probably also 
	end up with the infrastructure required to sell a competitive cloud offering.
	Google actually tried to do that without having a serious enterprise sales
	force and the result was that AWS and Azure basically split the enterprise 
	market between them.

The exact same line of reasoning that applies to optimization also applies to sales --
as long as marginal benefit of adding another salesperson exceeds the cost, you should
expect the company to keep adding salespeople, which can often result in a sales force
that's larger than the engineering team. There's also research which, almost by
definition, involves a lot of bets that don't pan out!

It's not that all of those things are necessary to run a service at all; it's that 
almost every large service is leaving money on the table if they don't seriously address
those things. This reminds me of a common fallacy we see in unreliable systems, where 
people build the happy path with the idea that the happy path is the “real” work, and
that error handling can be tacked on later. For reliable systems, error handling is more
work than the happy path. The same thing is true for large services -- all of this stuff
that people don't think of as “real” work is more work than the core service.
```

Damn Dan, you wrote this stream-of-consciousness? You've got yourself a new fan. 

<a name="#codebase-as-organism"></a>
### Codebase as organism
([overview](#overview))

Kevin Simler's blog [Melting Asphalt](https://meltingasphalt.com/about/) is always a great read. Here's one of my favorite essays of his, [A Codebase is an Organism](https://meltingasphalt.com/a-codebase-is-an-organism/).

The introduction alone is gold:

```markdown
Here's what no one tells you when you graduate with a degree in computer science and take
up a job in software engineering:

*The computer is a machine, but a codebase is an organism.*

This will make sense to anyone who's worked on a large or even medium-sized software project
— but it's often surprising to new grads. Why? Because nothing in your education prepares you
for how to deal with an organism.

Computer science is all about how to control the machine: to make it do exactly what you want,
during execution, on the time scale of nano- and milliseconds. But when you build real software
— especially as part of a team — you have to learn how to control not only the (very obedient) 
machine, but also a large, sprawling, and often unruly codebase.

This turns out to require a few 'softer' skills. Unlike a computer, which always does exactly 
what it's told, code can't really be bossed around. Perhaps this is because code is ultimately
managed by people. But whatever the reason, you can't tell a codebase what to do and expect to
be obeyed. Instead, the most you can do (in order to maximize your influence) is try to steward
the codebase, nurture it as it grows over a period of months and years.

When you submit a CS homework assignment, it's done. Fixed. Static. Either your algorithm is 
correct and efficient or it's not. But push the same algorithm into a codebase and there's a
very real sense in which you're releasing it into the wild.

Out there in the codebase, all alone, your code will have to fend for itself. It will be 
tossed and torn, battered and bruised, by other developers — which will include yourself, of
course, at later points in time. Exposed to the elements (bug fixes, library updates, drive-by
refactorings), your code will suffer all manner of degradations, "the slings and arrows of 
outrageous fortune... the thousand natural shocks that flesh is heir to."
```

The nursing metaphor, or "codebase as sick patient":

```markdown
The organic nature of code manifests itself in the dual forces of growth and decay.

Let's start with decay. Realizing that code can wither, decay, or even die leads us to the
nursing metaphor, or codebase as sick patient.

Code doesn't decay on its own, of course. Left completely untouched, it will survive as long 
as you care to archive it. Decay — often called code rot or software rot — only sets in when 
changes are made, either to the code itself or to any of its dependencies. So as a rule of thumb,
we can say that most code is decaying during most of its existence. It's like entropy. You never
'win' against entropy; you just try to last as long as you can.

In a healthy piece of code, entropic decay is typically staved off by dozens of tiny interventions 
— bug fixes, test fixes, small refactors, migrating off a deprecated API, that sort of thing.
These are the standard maintenance operations that all developers undertake on behalf of code
that they care about. It's when the interventions stop happening, or don't happen often enough,
that code rot sets in.

We can assess a module in terms of 'risk factors' for this kind of decay. The older a module is,
for example, the more likely it is to be suffering from code rot. More important than age, however, 
is the time since last major refactor. (Recently-refactored code is a lot like new code, for good
or ill.) Also, the more dependencies a module has, and the more those dependencies have recently 
changed, the more likely the module is to have gone bad.

But all of these risk factors pale in importance next to how much execution a piece of code has
been getting. Execution by itself isn't quite enough, though — it has to be in a context where 
someone is paying attention to the results. This type of execution is also known as testing.

Testing can take many forms — automated or manual, ad hoc developer testing, and even 'testing' 
through use in production. As long as the code is getting executed in a context where the results
matter, it counts. The more regularly this happens, of course, the better.

I find it useful to think of execution as the lifeblood of a piece of code — the vital flow of
control? electronic pulse? — and testing as medical instrumentation, like a heart rate monitor. 
You never know when a piece of code, which is rotting all the time, will atrophy in a way that 
causes a serious bug. If your code is being tested regularly, you'll find out soon and will be 
able to intervene. But without testing, no one will notice that your code has flatlined. Errors
will begin to pile up. After a month or two, a module can easily become so rotten that it's 
impossible to resuscitate.

Thus teams are often confronting the uncomfortable choice between a risky refactoring operation 
and clean amputation. The best developers can be positively gleeful about amputating a diseased 
piece of code (even when it's their own baby, so to speak), recognizing that it's often the best
choice for the overall health of the project. Better a single module should die than continue to
bog down the rest of the project.
```

Code growth:

```markdown
Now you might assume that while decay is problematic, growth is always good. But of course it's 
not so simple.

Certainly it's true that a project needs to grow in order to become valuable, so the problem 
isn't growth per se, but rather unfettered or opportunistic growth. Haphazard growth. Growth by
means of short-sighted, local optimizations. And this kind of growth seems to be the norm —
perhaps because developers are often themselves short-sighted and opportunistic, if not outright
lazy. But even the best, most conscientious developers fall pitifully short of making globally-
optimal decisions all the time.

Left to 'its' own devices, then, a codebase can quickly devolve into a tangled mess. And the more
it grows, the more volume it has to maintain against the forces of entropy. In this way, a project
can easily collapse under its own weight.

For these reasons, any engineer worth her salt soon learns to be paranoid of code growth.

She assumes, correctly, that whenever she ceases to be vigilant, the code will get itself into 
trouble. She knows, for example, that two modules will tend to grow ever more dependent on each 
other unless separated by hard ('physical') boundaries. She's had to do that surgery — to separate
two modules that had become inappropriately entangled with each other. Afraid of such spaghetti 
code (rat's nests), she strives relentlessly to arrange her work (and the work of others) into
small, encapsulated, decoupled modules.

Faced with the necessity of growth but also its dangers, the seasoned engineer therefore seeks a
balance between nurture and discipline. She knows she can't be too permissive; coddled code won't
learn its boundaries. But she also can't be too tyrannical. Code needs some freedom to grow at the
optimal rate.

In this way, building software isn't at all like assembling a car. In terms of managing growth, it's
more like raising a child or tending a garden.
```

The benefit of failing fast -- failure as conflict of interest between computer and codebase:

```markdown
Finally, here's an idea that took me many years to appreciate on a gut level (but which is completely
obvious now in hindsight): the benefits of failing fast. What I should have understood is that failure
(on unexpected inputs) reflects a conflict of interest between the computer and the codebase.

From the perspective of the machine on which the code is executing right now, it's better not to fail 
and hope that everything will be OK — hope that some other part of the stack will handle the failure 
gracefully. Maybe we can recover. Maybe the user won't notice. Why crash when we could at least try 
to keep going? And everything in my CS education taught me to do what's right for the machine.

But from the perspective of the codebase — whose success depends not on any single execution, but
rather on long-term health — it's far better to fail fast (and loud), in order to call immediate 
attention to the problem so it can be fixed.

Coddled code will fester. Spare the rod, spoil the child.
```

<a name="#Second-system-effect"></a>
### Second-system effect
([overview](#overview))

From Wikipedia:

```markdown
The second-system effect (also known as second-system syndrome) is the tendency of small,
elegant, and successful systems, to be succeeded by over-engineered, bloated systems, due 
to inflated expectations and overconfidence.
```

This *always* reminds me of that *great* Quora answer I've never been able to find, about an enterprise-level solution to an exceedingly trivial coding problem. First-class dry humor. 

Bit of nuance here. This is what Adam Turoff [has to say about software rewrite projects](http://notes-on-haskell.blogspot.com/2007/08/rewriting-software.html):

```markdown
One of the clearest opinions is from Joel Spolsky, who says rewrites are “the single worst 
strategic mistake that any software company can make”. His essay is seven years old, and in
it, he takes Netscape to task for open sourcing Mozilla, and immediately throwing all the 
code away and rewriting it from scratch. Joel was right, and for a few years Mozilla was a 
festering wasteland of nothingness, wrapped up in abstractions, with an unhealthy dose of
gratuitous complexity sprinkled on top. 

But this is open source, and open source projects have a habit of over-estimating the short
term and under-estimating the long term. ...

What’s missing from the discussion is an idea from Brian Eno about the differences between 
the “small here” vs. the “big here”, and the “short now” vs. the “long now”. Capsule summary:
we can either live in a “small here” (a great apartment in a crappy part of town) or a “big 
here” (a beautiful city in a great location with perfect weather and amazing vistas), and we 
can live in a “short now” (my deadline is my life) or a “long now” (how does this project 
change the company, the industry or the planet?).

On the one hand, Joel’s logic is irrefutable. If you’re dealing with a small here and a short
now, then there is no time to rewrite software. There are revenue goals to meet, and time 
spent redoing work is retrograde, and in nearly every case poses a risk to the bottom line 
because it doesn’t deliver end user value in a timely fashion.

On the other hand, Joel’s logic has got more holes in it than a fishing net. If you’re dealing 
with a big here and a long now, whatever work you do right now is completely inconsequential 
compared to where the project will be five years from today or five million users from now. 
Requirements change, platforms go away, and yesterday’s baggage has negative value — it leads
to hard-to-diagnose bugs in obscure edge cases everyone has forgotten about. The best way to 
deal with this code is to rewrite, refactor or remove it.

Joel Spolsky is arguing that the Great Mozilla rewrite was a horrible decision in the short 
term, while Adam Wiggins is arguing that the same project was a wild success in the long term.
Note that these positions do not contradict each other. Clearly, there is no one rule that fits
all situations.

The key to estimating whether a rewrite project is likely to succeed is to first understand when
it needs to succeed. If it will be evaluated in the short term (because the team lives in a small
here and a short now), then a rewrite project is quite likely to fail horribly. On the other hand,
if the rewrite will be evaluated in the long term (because the team lives in a big here and a long
now), then a large rewrite project just might succeed and be a healthy move for the project.
```

Why might rewrites be bad? Neil Gunton's [Rewrites Considered Harmful? When is "good enough" enough?](http://www.neilgunton.com/doc/?o=1mr&doc_id=8583):

```markdown
You might read all this and think what an idiot I am for suggesting that older, crappier, buggier,
dirtier, messier, more complex software might be better than newer, cleaner, faster rewrites. Well,
the point is a subtle one - in a nutshell, when you rewrite, you lose all those little fixes and 
improvements that made the older version good to use and reliable. New software always introduces 
new bugs. Often, the rewrite process seems to be driven by a desire to make the product somehow 
more theoretically consistent and complete - which in turn often ends up losing the simplicity and 
elegance that made the original so compelling and useful. Rewriting, especially when it breaks 
existing systems, results in multiple versions of software that makes it confusing for new users and
perplexing for old users.

And, let's face it - programmers just like to write new code. It's natural. We all do it - it's easier
to start from scratch than it is to make the old version better. Also, it's more glamorous - everybody
wants to be credited with creating something themselves, rather than maintaining and developing an 
existing thing. So, I can quite understand why things are the way they are.

Mind you, I am not saying that we should never rewrite code - sometimes it's just a necessary thing,
because of new platforms or changes to underlying API's. It's all a question of degree - do you 
totally rewrite, or do you evolve existing, working code? Rewrites are so often done without any
regard to the old code at all. In my experience, new programmers often come on board, and it's just 
too much trouble to look through and really understand all the little nooks and crannies. We have
seen it plenty of times in business - there is an old version of the application, but you're brought
in to put together a new version. Usually the new spec has so many functional/UI differences from 
the old one that the old is simply discarded as being irrelevant. And yet, many times, the underlying
functional differences are not actually all that great. So, unfortunately, years of patches, special
cases and wisdom are just abandoned.

There is a "cost" involved with totally rewriting any application, in terms of "lost wisdom". If you
have a package that is very popular, used by many people and has had a lot of bugfixes and patches 
applied over time, then it is more likely that a total rewrite will have a higher cost. Also if you
change the way it works in the process, you create a chasm between the new and old versions that has
to be crossed by users, and this causes stress. Which version to use - the old, reliable, well known
but out-of-date version, or the newer, sleaker, incompatible, more buggy version? Hmmm. If your
software (or standard) is not used by many people and doesn't have any significant history behind it
(in terms of "accumulated wisdom") then clearly there are no real issues involved in rewriting - the
cost is low. So I am not making a blanket statement that rewriting is bad; the whole point of this
article was to focus on tools and standards that have attained great success and are used by many
people. Such software/standards will inevitably have had a large amount of wisdom invested over time, 
because nothing is perfect first time out. Thus it is the most popular tools and packages that are
most likely to be casualties of total rewrites.

So in summary, I would say that the "cost" of a total rewrite depends on three factors:

1. Amount of "accumulated wisdom" (bug fixes, tweaks and useful patches) in the old version that will be discarded
2. How incompatible the new version is with the old version (API, data formats, protocols etc)
3. How many people used the old version and will be affected by the changes

A suggestion: If you have a very successful application, don't look at all that old, messy code as
being "stale". Look at it as a living organism that can perhaps be healed, and can evolve. You can 
refactor, you can rewrite portions of the internals to work better, many things can be accomplished
without abandoning all the experience and error correction that went into that codebase. When you 
rewrite you are abandoning history and condemning yourself to relive it.
```

Neil's last remark reminds me of Kevin Simler's [A Codebase is an Organism](https://meltingasphalt.com/a-codebase-is-an-organism/), which is a distinct enough idea that I also want to remember that I've created [its own subheading](#codebase-as-organism).

<a name="#Single-handedly-designing-large-codebases"></a>
### Single-handedly designing large codebases
([overview](#overview))

From Stephen Wolfram's [Ten thousand hours of design reviews](https://blog.stephenwolfram.com/2008/01/ten-thousand-hours-of-design-reviews/).

Motivation:

```markdown
It’s not easy to make a big software system that really fits together. It’s 
incredibly important, though. Because it’s what makes the whole system more
than just the sum of its parts. It’s what gives the system limitless
possibilities—rather than just a bunch of specific features.

But it’s hard to achieve. It requires maintaining consistency and coherence 
across every area, over the course of many years. But I think it’s something 
we’ve been very successful at doing with Mathematica.

I’ve been the chief architect and chief designer of Mathematica‘s core 
functionality. And particularly for Mathematica 6, there was a huge amount of
design to do. Actually, I think much more even than for Mathematica 1.

In fact, I just realized that over the course of the decade during which were 
developing Mathematica 6—and accelerating greatly towards the end—I spent 
altogether about 10,000 hours doing what we call “design reviews” for 
Mathematica 6, trying to make all those new functions and pieces of 
functionality in Mathematica 6 be as clean and simple as possible, and all fit
together.
```

Software design analogized to fundamental science, Wolfram's first stomping ground:

```markdown
At least the way I do it, doing software design is a lot like doing
fundamental science.

In fundamental science, one starts from a bunch of phenomena, and then one
tries to drill down to find out what’s underneath them—to try to find the 
root causes, the ultimate primitives, of what’s going on.

Well, in software design, one starts from a bunch of functionality, and then 
one needs to drill down to find out just what ultimate primitives one needs 
to support them.

In science, if one does a good job at finding the primitives, then one can
have a very broad theory that covers not just the phenomena one started from,
but lots of others too.

And in software design, it’s the same kind of thing.

If one does a good job at finding the primitives, then one can build a very 
broad system that gives one not just the functionality one was first thinking
about, but lots more too.
```

Design review process for making the entire codebase "cohere together holistically":

```markdown
Over the years, we’ve developed a pretty good process for doing design 
reviews.

We start with some particular new area of functionality. Then we get a
rough description of the functions—or whatever—that we think we’ll need
to cover it. Then we get down to the hard job of design analysis. Of 
trying to work out just what the correct fundamental primitives to cover
the area are. The clean, simple functions that represent the essence of
what’s going on—and that fit together with each other, and with the rest
of Mathematica, to cover what’s needed.

Long ago I used to do design analysis pretty much solo.

But nowadays our company is full of talented people who help. The focal
point is our Design Analysis group, which works with our experts in
particular areas to start the process of refining possible designs.

At some point, though, I always get involved. So that anything that’s a 
core function of Mathematica is always something that I’ve personally 
design reviewed.

I sometimes wonder whether it’s crazy for me to do this. But I think 
having one person ultimately review everything is a good way to make
sure that there really is coherence and consistency across the system. 
Of course, when the system is as big as Mathematica 6, doing all those 
design reviews to my level of perfection takes a long time—about 10,000
hours, in fact.

Design reviews are usually meetings with somewhere between two and twenty
people. (Almost always they’re done with web conferencing, not in person.)

The majority of the time, there’s a preliminary implementation of whatever
it is that we’re reviewing. Sometimes the people who are in the design 
review meeting will say “we think we have this mostly figured out”. 
Sometimes they’ll say “we can’t see how to set this up; we need your help”. 
Either way, what usually happens is that I start off trying out what’s 
been built, and asking lots and lots of questions about the whole area 
that’s involved.

It’s often a very grueling process. Progressively polishing things until 
they are as clean and simple as possible.

Sometimes we’ll start a meeting with things looking pretty complicated. A 
dozen functions that use some strange new construct, and have all sorts of
weird arguments and options.

It’s usually pretty obvious that we have to do better. But figuring out how
is often really hard.

There’ll usually be a whole series of incremental ideas. And then a few big 
shifts—which usually come from getting a clearer understanding of what the
true core functionality has to be.
```

Big-picture generalist's wet dream quote, the one impression I vaguely garnered most from this essay actually:

```markdown
It’s sometimes a little weird. One hour I’ll be intensely thinking about 
the higher mathematics of number theory functions. And the next hour I’ll
be intensely focused on how we should handle data about cities around the 
world. Or how we should set up the most general possible interfaces to 
external control devices.

But although the subject matter is very varied, the principles are at some
level the same.

I want to understand things at the most fundamental level—to see what the 
essential primitives should be. Then I want to make sure those primitives
are built so that they fit in as well as possible to the whole existing
structure of Mathematica—and so they are as easy as possible for people to
understand, and work with.

Doing design reviews and nailing down the functional design of Mathematica 
is a most satisfying intellectual activity. It’s incredibly diverse in
subject matter. And in a sense always very pure.

It’s about a huge range of fundamental ideas—and working out how to fit them
all together to create a coherent system that all makes sense.

It’s certainly as hard as anything I know about in science. But in many ways
it’s more creative. One’s not trying to decode what exists in the world. One’s
trying to create something from scratch—to build a world that one can then work
within.
```

Established precedent as design default for many reasons:

```markdown
Often we’ll be talking quite a bit about precedents elsewhere in Mathematica.
Because the more we can make what we’re designing now be like something we’ve
done before in Mathematica, the better.

For several reasons. First, because it means we’re using approaches that we’ve
tested somewhere else before.

Second, because it means that what we’re doing now will fit in better to what
already exists.

And third, because it means that people who are already familiar with other 
things Mathematica does will have an easier time understanding the new things
we’re adding.
```

So breaking away from established precedent needs reasons:

```markdown
But some of the most difficult design decisions have to do with when to break
away from precedent. When is what we’re doing now really different from anything
else that we’ve done before? When is it something sufficiently new—and big—that 
it makes sense to create some major new structure for it?

At least when we’re doing design reviews for Mathematica kernel functions, we 
always have a very definite final objective for our meetings: we want to actually
write the reference documentation—the “function pages”—for what we’ve been talking
about.

Because that documentation is what’s going to provide the specification for the 
final implementation—as well as the final definition of the function.

It always works pretty much the same way: I’ll be typing at my computer, and 
everyone else will be watching my screen via screen-sharing. And I’ll actually be 
writing the reference documentation for what each function does. And I’ll be asking 
every sentence or so: “Is that really correct? Is that actually what it should do?”
And people will be pointing out this or that problem with what we’re saying.

It’s a good process, that I think does well at concentrating and capturing what we
do in design analysis.
```
