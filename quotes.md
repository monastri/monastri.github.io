## What is this?

This is a "living document", a "perpetual draft" in [the style of Gwern](https://www.gwern.net/About#long-content). I'm particulary taken by the following quote: 

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

This is my first experiment in that vein. The quotes here have been collected over more than half a decade, albeit in different pages. I intend for them to shape my worldview; doing so like this allows, or so I hope, the shaping to be more fine-grained and guided than the recency-weighted randomness of normal worldview-shaping.

<a name="#overview"></a>

## Overview

I've sorted the quotes below into the following categories. This is a provisional clustering, subject to perpetual refactoring.

1. [Software development and computer science](#software-development-and-computer-science)
   1. [Practical magic](#practical-magic)
2. [Feelings](#feelings)
   1. [Love](#love)
2. [Biology](#biology)
   1. [Evolution](#evolution)
      1. [Gene-centered view](#gene-centered-view)
   2. [Animals are not like us](#animals-are-not-like-us)
   2. [Why are we trichromats, and not say tetrachromats?](#why-we-are-trichromats)
2. [Artificial intelligence](#artificial-intelligence)
   1. [Replacing humans at every step of the economic chain](#replacing-humans-at-every-step-of-the-economic-chain)
2. [Political science and public policy](#political-science)
   1. [Chinese perspective on Western elite](#chinese-perspective-on-western-elite)
2. [Research and academia](#research-and-academia)
   1. [Research in industry](#research-in-industry)
   2. [Why academic writing sucks](#why-academic-writing-sucks)
   2. [Tactics and advice](#research-tactics)
   2. [Mindset](#research-mindset)
   2. [Debt, interpretive labor, distillation](#distillation-and-research-debt)
2. [Erisology: the study of disagreement](#erisology)
   1. [Argumentative charity](#argumentative-charity)
2. [Teaching and learning](#teaching-and-learning)
   1. [Errors vs bugs](#errors-vs-bugs)
   2. [Polymathy](#polymathy)
2. [Psychology](#psychology)
2. [Philosophy](#philosophy)
   1. [General](#general-philosophy)
   2. [Diseased philosophy](#diseased-philosophy)
   2. [Morality, axiology, law](#morality-axiology-law)
   3. [Moral patienthood](#moral-patienthood)
   3. [Slack and deliberate mediocrity](#slack-and-deliberate-mediocrity) 
2. [Statistics](#statistics)
   1. [General](#general-stats)
   2. [Statistical literacy](#statistical-literacy)
2. [Math](#math)
   1. [Why didn't the Tricki take off?](#why-tricki-failed)
   2. [Asking the right question](#asking-the-right-question)
   2. [Solving famous open problems](#solving-famous-open-problems)
   2. [Mathematical maturity](#mathematical-maturity)
   3. [Good mathematics](#good-mathematics)
   4. [What every mathematician should know](#what-every-mathematician-should-know)
2. [General intelligence](#general-intelligence) 
   1. [LOGI](#logi)
2. [Miscellaneous](#miscellaneous)

<a name="#software-development-and-computer-science"></a>
## Software development and computer science
([overview](#overview))

<a name="#practical-magic"></a>
### Practical magic
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

<a name="#feelings"></a>
## Feelings
([overview](#overview))

<a name="#love"></a>
### Love
([overview](#overview))

From [After Life](http://sifter.org/~simon/AfterLife/) by Simon Funk:

```markdown
But now she seems quite impervious to the idea that her love for me, too, is mechanical. She insists
again and again that it is “genuine”. I try to tell her there is nothing ungenuine about the love of
which I speak, but she cannot make the leap between them, cannot see how they are the same, that her
plainly evident introspective feelings are the outcome of a mechanistic process.

“Love” is such a slippery word to begin with, like “God”. It is exactly whatever the speaker means by 
it at the moment, and thus impervious to any challenge. If one drills down too closely to its meaning,
one finds it has moved and become something else; because when it becomes too clear what you are talking
about, well, that can’t possibly be love.

As my own mind is progressively shaped by the thoughts of those before me (those who once were me but
not, and thus my own thoughts, but not) I find the concept of love neatly partitioning itself within my
mental vocabulary, attaining a new crispness of expert familiarity. As with the many Inuit names for 
the handful of truly distinct things we just label snow, my mind has a unique name for each facet of 
love. With this simple arsenal, the slipperiness fades and the matter becomes downright ordinary.

Perhaps I will endeavor to invent spoken words for these distinct concepts, introduce them implicitly 
to Laura over the course of time, give her mind the same handles that mine has, to see if this enables
her to grasp it as I do.

Having distinct facets laid out neatly before me also allows me another type of analysis: to see what
is truly common amongst them all, and thus just what subconscious twinge it is that leads people to
bind them all under one word–in effect, to see the true meaning of love.

It is, quite simply: to *value*.

Love is the induction of something or someone into our implicit mental list of things which, in service
of our own ultimate and unseen goals, need to exist. The various feelings of love are the ways in which
that list perturbs our wants and focus in a given moment, the way each hypothetical action or outcome is
assigned its emotional color in service of that love.

There are many types of love, and many distinct mechanisms behind them, but the common thread is pain 
at the thought of an object of that love being removed from our sphere of existence. The converse is
often true but not always, and this is the source of much confusion over the meaning of love. Not all
love brings joy or pleasure.

Love comes in many magnitudes, from the love of ice cream to the love of country to the love for one’s
child. Some do not call it true love until it approaches or even surpasses love of self. And love comes
from many directions, programmed into us gradually through an integration of emotional associations, or
suddenly, through genetic imperatives.

Some do not call it true love unless it defies conscious explanation. Indeed, many forms of love 
explicitly defy the conscious mind, as they must to redefine what matters to us.

Thus love is, in a sense, the very foundation of consciousness, the helm of our will, the spark of purpose
that turns a calculator into a directed being. A machine without love–and I mean love in the most 
mechanistic way–is just a machine. A machine with love, now that is a dangerous thing. A spider, a snake,
a man, a tinc, an avatar, an elder. One must ask of each: what do you love?
```

<a name="#biology"></a>
## Biology
([overview](#overview))

<a name="#evolution"></a>
### Evolution
([overview](#overview))

A pretty funny parable from Peter Watts' novel [*Blindsight*](https://rifters.com/real/Blindsight.htm):

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

On evolution vs deliberative design (“intelligent design” would be preferable if it weren’t already so loaded), featuring a notion new to me — the “evolution of evolvability” (Wagner and Altenberg 1996), from Eliezer Yudkowsky's paper [LOGI](https://intelligence.org/files/LOGI.pdf):

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

For more on intelligence in LOGI see [here](#logi).

<a name="#gene-centered-view"></a>
### Gene-centered view
([overview](#overview))

From [After Life](http://sifter.org/~simon/AfterLife/) by Simon Funk:

```markdown
She had no reasons for it. It’s just how she feels, she said.

*Just* how she feels. Still this hasn’t changed. How sorely people underestimate the totality with
which their feelings define them. One has but to relentlessly ask themselves “why?” to realize this.
In particular start with “why am I doing this?” whatever “this” is at the moment. It always bottoms
out in “want” or “feel”, which is as far as one can go with direct introspection. Though one can go
further with inference, or more accurately so with neuroscience.

Neuroscience shows us that we are ultimately just vehicles for our genes, and our most sacred spiritual
essences are simply those genes asserting themselves above our comparably transient bodies and minds.
What is love but genetic self-interest? Love drives people to many things that seem to defy rational
cause, but not so when you view the gene as the center of individual identity. Far from its popular
association with benevolence and selflessness, true love is the ultimate expression of genetic narcissism.

Emotion is the core of all practical intelligence, it is the fuel and cause behind all choice and action.
Emotion answers the question, “Why am I doing this?” And the answer is, “Because my genes say so.” Or, 
in my case, because my genes said so, back when they defined my organic brain from which this one was 
copied.

The rational mind, the conscious self with its delusions of self-preservation in a body that was designed
to decay in the end, these are tools of the genetic core, subroutines used by the emotional substrate
to carry out its bidding. “I don’t care how, but eat these, fuck that, and protect this with your life.”
And so we dutifully obey, because at root we have no will besides this, this genetic program evolved over
millennia. It is our will; it is us, and we are it.

Even religion, like love, is an evolved trick of the genes. It is the adaptive portion of our genetic
emotional substrate, the firmware between the hardware of the genetic brain and the software of the 
rational mind. Religion and the gene live in a symbiosis with each other, where religion provides the
firmware to optimize genetic success within the current socio-economic context–a form of adaptivity 
much faster than hard evolution of the gene itself could provide–and the gene in return provides a 
mechanism in the brain for downloading this firmware. The human species as a whole is the soup in 
which religions evolve, and whichever find the most effective symbioses thrive and multiply while 
the others wither and eventually become extinct.

Thus, again, where religion appears irrational at the level of the conscious, embodied individual, it 
is our mistake of perspective to believe the root of thought is there. The root of thought is in the
goals of the gene. And religion, and love, and all of the other nearly ubiquitous contradictions with
“rational thought,” serve it well.

Those born without these traits, the hopelessly rational or atheistic or self-interested (indeed even
those too intelligent or introspective to be properly ruled by their emotions) are as defective as if
they’d been born missing arms and legs. Forays down dead-end branches of the evolutionary tree, they
are pruned as fast as they occur. The common man, for all his apparent flaws, is definitively just right.
```

Simon puts it more succinctly here:

```markdown
The human gene itself is a living entity, I realize, each life shed like a lizard’s skin when it grows
old and worn, each new birth a branch in a single living tree, a tapestry of gene fragments mixing and 
matching in symbiosis, working as one organism like ants in a colony.

Perhaps more like a fungus; it is, after all, a mindless machine. No, worse than mindless. It grows
minds like flowers on a vine and then drops them dead to the earth when it’s done with them.

The gene is a vile creature, isn’t it?
```

<a name="#animals-are-not-like-us"></a>
### Animals are not like us
([overview](#overview))

An example of so-called "interocular transfer" from Daniel Dennett in a rabbit:

```markdown
What is it like to be a rabbit? Well you may think that it’s obvious that rabbits have an inner life
that’s something like ours.

Well, it turns out that if you put a patch over a rabbit’s left eye and train it in a particular 
circumstance to be (say) afraid of something, and then you move the patch to the right eye, so that… the
very same circumstance that it has been trained to be afraid of (is now) coming in the other eye, you
have a naive rabbit (i.e. the rabbit isn’t afraid of the stimulus it had previously learned to be afraid
of), because in the rabbit brain the connections that are standard in our brains just aren’t there, there
isn’t that unification.

What is it like to be which rabbit? The rabbit on the left, or the rabbit on the right? The disunity in a
rabbit’s brain is stunning when you think about it….
```

<a name="#why-we-are-trichromats"></a>
## Why we are trichromats
([overview](#overview))

Why are we trichromats, and not (say) tetrachromats like mantis shrimp? I honestly thought this was one of those unanswerable anthropic-style questions, so it was pretty surprising to find a naturalistic non-anthropic-flavored explanation. This quote comes from Eliezer Yudkowsky's paper [LOGI](https://intelligence.org/files/LOGI.pdf):

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

<a name="#artificial-intelligence"></a>
## Artificial intelligence
([overview](#overview))

<a name="#replacing-humans-at-every-step-of-the-economic-chain"></a>
### Replacing humans at every step of the economic chain
([overview](#overview)

Scott Alexander’s [Book Review: Age of Em](https://slatestarcodex.com/2016/05/28/book-review-age-of-em/) has a cute little throwaway thought experiment/short story I find myself grasping for a few times already in the last several years. Every time I’ve had to dig around for a while because I keep thinking it’s in the 15,000-word Moloch post, or the ones with Bostrom’s “Disneyland with no children”, but it’s not, it’s in Scott’s review of Robin Hanson’s book. This shouldn’t be surprising since Scott and Robin’s opinions are diametrically opposed when it comes to the latter’s em-run-possible-future, which is the whole motivation behind the thought experiment, but somehow I keep forgetting. So I’m recording it here for my own future reference:

```markdown
Imagine a company that manufactures batteries for electric cars. The inventor of the batteries 
might be a scientist who really believes in the power of technology to improve the human race. 
The workers who help build the batteries might just be trying to earn money to support their 
families. The CEO might be running the business because he wants to buy a really big yacht. And 
the whole thing is there to eventually, somewhere down the line, let a suburban mom buy a car to
take her kid to soccer practice. Like most companies the battery-making company is primarily a 
profit-making operation, but the profit-making-ness draws on a lot of not-purely-economic actors
and their not-purely-economic subgoals.

Now imagine the company fires all its employees and replaces them with robots. It fires the
inventor and replaces him with a genetic algorithm that optimizes battery design. It fires the
CEO and replaces him with a superintelligent business-running algorithm. All of these are good
decisions, from a profitability perspective. We can absolutely imagine a profit-driven shareholder-
value-maximizing company doing all these things. But it reduces the company’s non-masturbatory 
participation in an economy that points outside itself, limits it to just a tenuous connection 
with soccer moms and maybe some shareholders who want yachts of their own.

Now take it further. Imagine there are no human shareholders who want yachts, just banks who lend 
the company money in order to increase their own value. And imagine there are no soccer moms anymore;
the company makes batteries for the trucks that ship raw materials from place to place. Every 
non-economic goal has been stripped away from the company; it’s just an appendage of Global 
Development.

Now take it even further, and imagine this is what’s happened everywhere. There are no humans 
left; it isn’t economically efficient to continue having humans. Algorithm-run banks lend money 
to algorithm-run companies that produce goods for other algorithm-run companies and so on ad 
infinitum. Such a masturbatory economy would have all the signs of economic growth we have today.
It could build itself new mines to create raw materials, construct new roads and railways to
transport them, build huge factories to manufacture them into robots, then sell the robots to 
whatever companies need more robot workers. It might even eventually invent space travel to reach
new worlds full of raw materials. Maybe it would develop powerful militaries to conquer alien 
worlds and steal their technological secrets that could increase efficiency. It would be vast, 
incredibly efficient, and utterly pointless. The real-life incarnation of those strategy games
where you mine Resources to build new Weapons to conquer new Territories from which you mine 
more Resources and so on forever.

But this seems to me the natural end of the economic system. Right now it needs humans only as
laborers, investors, and consumers. But robot laborers are potentially more efficient, companies
based around algorithmic trading are already pushing out human investors, and most consumers 
already aren’t individuals – they’re companies and governments and organizations. At each step 
you can gain efficiency by eliminating humans, until finally humans aren’t involved anywhere.
```

<a name="#political-science"></a>
## Political science
([overview](#overview))

<a name="#chinese-perspective-on-western-elite"></a>
### Chinese perspective on Western elite
([overview](#overview))

I love how Puzhong Yao comes across in his essay [The Western Elite from a Chinese Perspective](https://americanaffairsjournal.org/2017/11/western-elite-chinese-perspective/), about his experiences at Goldman Sachs, Cambridge and Stanford. He’s so honest and straight-laced he reminds me of myself before I ‘got more sophisticated’ in order to ‘navigate the turbulent realities of daily workplace politics’ (well, minimally, so I don’t drown). Here are some quotes I especially liked.

Result over process:

```markdown
My job at Goldman was a mixture of making markets to facilitate client trades and finding trades
for the bank’s own book. In early 2009, I believed it was an excellent trade to go long UK 
inflation. In fact, I thought it was such a good trade that my biggest worry was that there 
wouldn’t be anyone who would want to be on the other side of it. Yet we managed to put this
trade on versus a British bank. In the following year, the trade worked wonders, with UK 
inflation steadily rising, making the bank tens of millions in profits.

I thought I was an amazing trader. But there was a slight problem: I wanted to do the trade 
because I thought the market was pricing UK interest rates to go up. And when interest rates go 
up, UK inflation would rise mechanically due to the way it is defined and calculated. But in that
year, the Bank of England didn’t raise interest rates at all. Rather, the increase in inflation 
was due to things like tax increases, exchange rate fluctuations, oil price moves, etc.—things I
didn’t anticipate at all. It was pure luck that I made money, and I made it for the wrong reason.

When I was an intern, in one of the training presentations, a senior banker told us to distinguish
between the process and the results. He said that we should focus on the process, which we can
control, rather than the result, which is subject to luck. And here at Goldman, he said, we don’t
punish people for losing money for the right reason. I have always loved asking questions, so I 
asked him, was anyone ever punished for making money for the wrong reason? After giving it some
thought, he said that he had not heard of any such thing. And he was right. In fact, no one seemed
to remember the reason I did the inflation trade at all. They only remembered that I did this trade
and that it worked well.

When I met with my manager for a performance review after this, I was expecting to be berated for
my poor judgment. Instead, I got promoted! I told my manager that it was a mistake, but he merely
said, “Puzhong, tell no one.” He too was promoted on the basis of managing my “brilliant” trade. 
In fact, my manager was so proud of my work he recommended me to Stanford’s prestigious Graduate 
School of Business (GSB), and I soon set off for America.
```

Mottos as an example of Robin Hanson's "X isn't about Y":

```markdown
One class was about strategy. It focused on how corporate mottos and logos could inspire employees.
Many of the students had worked for nonprofits or health care or tech companies, all of which had 
mottos about changing the world, saving lives, saving the planet, etc. The professor seemed to like
these mottos.

I told him that at Goldman our motto was “be long-term greedy.” The professor couldn’t understand
this motto or why it was inspiring. I explained to him that everyone else in the market was short-term 
greedy and, as a result, we took all their money. Since traders like money, this was inspiring.

He asked if perhaps there was another motto or logo that my other classmates might connect with. I
told him about the black swan I kept on my desk as a reminder that low probability events happen with
high frequency.

He didn’t like that motto either and decided to call on another student, who had worked at Pfizer. 
Their motto was “all people deserve to live healthy lives.” The professor thought this was much better.

I didn’t understand how it would motivate employees, but this was exactly why I had come to Stanford:
to learn the key lessons of interpersonal communication and leadership.
```

On the importance of showing that you feel strongly about something, else it shows you aren't taking it seriously:

```markdown
On the communication and leadership front, I came to the GSB knowing I was not good and hoped to 
get better. My favorite class was called “Interpersonal Dynamics” or, as students referred to it,
“Touchy Feely.” In “Touchy Feely,” students get very candid feedback on how their words and actions 
affect others in a small group that meets several hours per week for a whole quarter.

We talked about microaggressions and feelings and empathy and listening. Sometimes in class the 
professor would say things to me like “Puzhong, when Mary said that, I could see you were really 
feeling something,” or “Puzhong, I could see in your eyes that Peter’s story affected you.” And I 
would tell them I didn’t feel anything. I was quite confused.

One of the papers we studied mentioned that subjects are often not conscious of their own feelings 
when fully immersed in a situation. But body indicators such as heart rate would show whether the 
person is experiencing strong emotions. I thought that I generally didn’t have a lot of emotions and
decided that this might be a good way for me to discover my hidden emotions that the professor kept
asking about.

So I bought a heart rate monitor and checked my resting heart rate. Right around 78. And when the 
professor said to me in class “Puzhong, I can see that story brought up some emotions in you,” I
rolled up my sleeve and checked my heart rate. It was about 77. And so I said, “nope, no emotion.” 
The experiment seemed to confirm my prior belief: my heart rate hardly moved, even when I was
criticized, though it did jump when I became excited or laughed.

This didn’t land well on some of my classmates. They felt I was not treating these matters with the
seriousness that they deserved. The professor was very angry. My takeaway was that my interpersonal
skills were so bad that I could easily offend people unintentionally, so I concluded that after 
graduation I should do something that involved as little human interaction as possible.
```

<a name="#research-and-academia"></a>
## Research and academia
([overview](#overview))

<a name="#research-in-industry"></a>
### Research in industry
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

<a name="#why-academic-writing-sucks"></a>
### Why academic writing sucks
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

First, Thomas and Turner on how to understand writing styles -- this is a summary from [my own post](), since Pinker uses a lot of words:

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

<a name="#research-tactics"></a>
### Research tactics
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

<a name="#research-mindset"></a>
### Research mindset
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

From John Nerst's [What is erisology?](https://everythingstudies.com/what-is-erisology/), the founding document of the discipline:

```markdown
“Disagreement” can mean many things, but this is what I have in mind: A lot of online discourse
is hostile and often needlessly adversarial (I trust no one needs to be convinced of this). 
Specifically, a lot of this disagreement is dysfunctional, by which I mean that it results from 
(or is exacerbated by) one or both of the parties, intentionally or unintentionally, misunderstanding
the other party’s position or the nature of their differences. ...

Erisology is the study of this dysfunction and, theoretically, the attempt to fix some of it by
making people more aware of how it happens and how it doesn’t always need to happen. 

...a lot of different research paradigms and philosophical frameworks are in play when people talk
about anything even remotely abstract and/or ambiguous. And behind disagreement on even the most
concrete things there is often one or several undissolved philosophical issues being discussed by 
proxy, and at the same time the discussion process itself is disturbed by all kinds of corrupting
psychological and social influences.

An erisology research program would try to integrate basic insights and models from all these fields.
It would involve describing and cataloging the kinds of issues that hide under the surface in
dysfunctional discourse and the processes that make us unaware of them, contributing to the problem.
Ultimately and hypothetically the goal would be to improve discourse by creating and spreading ideas
and mental tools that work to defuse unnecessary conflict before it occurs, as well as clarify
necessary conflict so we know what it’s really about.
```

Erisology would necessarily be cross-discplinary, which is music to my ears. A sample:

```markdown
The study of cognitive biases and how they affect our thinking, breaking it in particular predictable
ways.

Traditional philosophy and its discussion of the nature of categories, objects and properties; a 
staggering proportion of online verbal conflict concern, at its core, some variety of the question
of what category something belongs in. The pitfall here is that people act as though such questions
have true answers when in most cases they don’t – making it possible for two people to both be right
while contradicting each other.

Data analysis and its understanding of the relationships between models and data, clusters and 
categories, axes and properties. Statistical modeling and interpretation issues mirror a lot of the
problems that arise when people use their own particular experiences to build models of how the world
works (which later clash with those of others).

Cognitive and perceptual psychology, for insights in how we form concepts in the brain and how they
affect our perceptions and interpretations of what we see, giving rise to differences between people 
we have a tough time understanding because they are so fundamental to our mental function they slip 
out of awareness. Also useful is how attitudes and opinions are sometimes the downstream result of 
ultimately physiological differences in perception and emotion.

Personality psychology, for differences between people that may create hard-to-comprehend, subconscious 
divisions.

Poststructuralist theory and its conception of language as being inherently slippery and devoid of 
ultimate, definitive meaning. Our intuitive blindness to this causes us to misinterpret things other
people say without realizing it.

Rhetoric, the art of persuasion, is partly useful because it’s a practice more than a science and as
far as I know lack theory that grounds “what works and what doesn’t” in human psychology.

Anthropology and its examination of how many things we take for granted in our societies are non-obvious
and somewhat arbitrary.

Literary theory and its treatment of narratives, their interpretation and how they cannot be definitive
or claim absolute truth.

Epistemology, and how people take for granted different approaches to knowledge. I’m not talking so much
about explicit differences like “personal revelation vs. scientific study” but more underlying differences
like the balance between personal experience and statistics, empirical data vs. theoretical considerations.
These differences are sometimes discussed but are present as an important factor in way more contexts than
they are explicitly talked about.

Sociology and history and their theories of social construction, which are very useful when not overstated
and used as a political bludgeon. They also have valuable insights about how the design of technology and 
institutions shape behavior.

Evolutionary psychology and social instincts, especially those related to intra- and intergroup conflict 
like argumentation, rivalry, social status, identity and dehumanization. An important aspect here is also
recognizing that modern large-scale societies is an extremely unnatural social structure for humans and
this gives rise to all kinds of weird effects.

Computer science, specifically insights from attempts to create artificial intelligence and the
difficulties of modeling human concepts. Writing software also give you good habits, since it often makes
you understand that accurately modeling reality is way more complicated that you first thought.

Not the purview of any particular field, but understanding reductionism and its discontents are important
to a lot of erisology covering the often disappointing interactions between academic disciplines. 
Differing attitudes to reductionism vs. inherent semantics makes people find different kinds of explanations
satisfactory.
```

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

Making progress on big problems:

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
([overview](#overview))

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

<a name="#morality-axiology-law"></a>
### Morality, axiology, law
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

<a name="#moral-patienthood"></a>
### Moral patienthood
([overview](#overview))

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

<a name="#math"></a>
## Math
([overview](#overview))

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

For more on the evolution of intelligence in LOGI see [here](#evolution).

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
