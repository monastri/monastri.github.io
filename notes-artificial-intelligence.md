*[Word count](https://wordcounter.net/): 5,100*

## What is this?

This is the "artificial intelligence" section of [this notebook](https://github.com/monastri/monastri.github.io/blob/master/quotes.md), last updated Apr 6, 2019, which got so big (1.2 million char) that GitHub refused to render the whole page anymore, ruining my original dream of having my entire notebook in one long page for two purposes: (1) zero-latency clickthrough to make up for my working memory's sand-thru-sieve transience; (2) lower activation energy for continuous document-wide refactoring, to aid recall and cross-domain interlinking.

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


1. [Digital evolution and artificial life](#Digital-evolution-and-artificial-life)
	1. [The evolved radio](#The-evolved-radio)
	2. [The evolved ear](#The-evolved-ear)
2. [Levels of Organization in General Intelligence](#Levels-of-Organization-in-General-Intelligence)
   
---------------------------------

<a name="#Levels-of-Organization-in-General-Intelligence"></a>
## *Levels of Organization in General Intelligence*
([overview](#overview))

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

<a name="#Digital-evolution-and-artificial-life"></a>
## Digital evolution and artificial life
([overview](#overview)) 

<a name="#The-evolved-radio"></a>
### The evolved radio
([overview](#overview)) 

[This footnote](https://intelligence.org/2017/04/12/ensuring/#footnote_10_15407) from (the transcript to) Nate Soares’s recent talk at Google on the AI value alignment problem sent chills up my spine:

```markdown
Consider Bird and Layzell’s example of a very simple genetic algorithm that was 
tasked with evolving an oscillating circuit. Bird and Layzell were astonished to
find that the algorithm made no use of the capacitor on the chip; instead, it had
repurposed the circuit tracks on the motherboard as a radio to replay the 
oscillating signal from the test device back to the test device.

This was not a very smart program. This is just using hill climbing on a very small
solution space. In spite of this, the solution turned out to be outside the space
of solutions the programmers were themselves visualizing. In a computer simulation,
this algorithm might have behaved as intended, but the actual solution space in the
real world was wider than that, allowing hardware-level interventions.

In the case of an intelligent system that’s significantly smarter than humans on 
whatever axes you’re measuring, you should by default expect the system to push 
toward weird and creative solutions like these, and for the chosen solution to be 
difficult to anticipate.
```

The full paper by Bird and Layzell is [The Evolved Radio and its Implications for Modelling the Evolution of Novel Sensors](https://people.duke.edu/~ng46/topics/evolved-radio.pdf). 

Abstract:

```markdown
Sensor evolution research typically uses evolutionary algorithms (EAs) to generate
sensors that near-optimally satisfy large numbers of constraints. This is 
qualitatively different from the phylogenetic process found in nature that has 
resulted, for example, in the mammalian auditory ossicles evolving from the jaw 
bones of amphibians and reptiles, that in turn had previously acted as gill arches
in fish.

This paper describes an evolvable hardware experiment that resulted in a network of
transistors sensing and utilising the radio waves emanating from nearby PCs. We 
argue that this evolved ‘radio’ is only the second device ever whose sensors were
constructed in a way that in key aspects is analogous to that found in nature. We 
highlight the advantages and disadvantages of this approach and show why it is 
practically impossible to implement a similar process in simulation.
```

The last sentence above pretty much summarizes the purpose of the paper, but they hammer it home in the introduction:

```markdown
Darwin was one of the first to observe that, “throughout nature almost every part 
of each living being has probably served, in a slightly modified condition, for 
diverse purposes” ….

This paper shows why it is practically impossible to implement an analogous process
in a simulated environment. This is an important issue for two reasons. Firstly, it
is necessary to be clear about the differences between EAs and natural evolution if
the aim is a theoretical understanding of the evolution of novel sensors in 
organisms [7,8]. Secondly, from an engineering perspective, when designing robot 
sensors it is essential to be aware of the limitations, as well as the strengths, of
particular methodologies.

A key advantage of testing in real-world, physical environments is that the circuits
are free to take advantage of a wide range of environmental invariants, none of which
have to be specified by the experimenter at the outset. This range is further
extended when the constraints adopted in conventional electronic engineering to 
ensure robust and predictable operation are relaxed [9]. Evolution is then free to 
explore very unusual designs: circuits with strange structures and intricate dynamical
behaviours beyond the scope of conventional design. In unconstrained HE, the circuit
primitives do not have their behaviour constrained within specific input and output 
ranges or by temporal coordination, nor are they restricted to playing specific
functional roles. Consequently, the process of unconstrained intrinsic HE is more like 
tinkering than conventional engineering [10,11] and in some key aspects is analogous to
natural evolution.

This paper details an unconstrained, intrinsic HE experiment where a network of 
transistors sensed and utilised the radio waves emanating from a nearby PC. 
Essentially, the EA led to the construction of a radio. This is, as far as the authors
know, only the second example of a physical device whose sensors were constructed by a 
process analogous to that of phylogenetic change. We compare the circuit to the first 
device constructed in this way: Gordon Pask’s electrochemical ear [12]. We argue that 
both of these devices display three key characteristics: they were constructed and
tested in real environments; their basic primitives were not constrained to 
experimenter specified functional roles; and the primitives were sensitive to a wide 
range of environmental stimuli. We highlight the difficulties in implementing 
comparable processes in simulation and argue that only unconstrained physical systems
situated in real-world environments can ever construct novel sensors in a way analogous 
to the phylogenetic process found in nature.
```

(See [here](#the-evolved-ear) for Gordon Pask's electrochemical ear.)

An aside: there’s a neat little table in the paper that says, look, evolution isn’t so much *engineer* as *tinkerer*: it isn’t goal-directed, it uses whatever is at hand (instead of being free of the constraints of previous designs), it comes up with whatever works (instead of aiming for the best solution given constraints), and it freely combines systems and even transforms them for new uses (instead of insulating subsystems and minimizing side effects).

This segues nicely into the quote below:

```markdown
Sensor evolution research using EAs tends to use *static* fitness functions; this is
very much the engineering methodology where the goal is to find a near-optimal solution 
to a well-defined problem. This is clearly not analogous to natural evolution, where the
fitness landscape is dynamic and there is no clearly defined goal.

Some sensor evolution research tries to make the search less constrained by allowing 
limited changes in the dimensionality of the search space. For example, the number of 
sensors and/or the size of the controller, that maps sensor states to behaviour, are
varied [3,5,19]. Menczer and Belew [20] argue that fitness functions should be implicit, 
for example, based on energy levels, in order to allow “creative, ‘open-ended’ evolution”.

However, these approaches cannot overcome a fundamental constraint in simulating sensor 
evolution: the experimenter sets a bound on the possible interactions between the agent 
and the environment. This is a direct consequence of the simulation process: firstly, the
experimenter has to model *explicitly* how different environmental stimuli change the state
of the sensors; secondly, experimenters only simulate those aspects of the environment 
that they think are relevant to their experiment, otherwise the simulation would become
computationally intractable.

These constraints make it very difficult to see how there can be a simulation of the 
evolution of novel sensors, as the possible sensor/environment interactions are 
prespecified and cannot vary: an external observer can model the system deterministically.

It might be argued that a simulation can model the evolution of a novel sensor from an
*agent’s* perspective. However, constructing a novel sensor does not involve selecting 
which environmental stimulus to utilise from a prespecified finite list. Lewontin [22] 
points out that the world can be partitioned a priori into an infinite number of 
ecological niches but that we can only know which of these partitions are niches by the 
presence of an organism. The same argument holds for environmental stimuli, which can only
be defined by reference to an organism. Novel sensors are constructed when a device,
rather than an experimenter, determines which of the infinite number of environmental 
perturbations act as useful stimuli.
```

This whole quote, and especially that last paragraph above, had the feel of groping-in-the-dark natural philosophy being slowly turned into engineering, which is I suppose something that happens at the frontier of research all the time, but is arguably more prevalent in a field as confused as general AI where the goal is to literally *build minds*; more relevantly, this field is where I get that sensation most frequently—is there a name for it? Wonderment tinged with fear? It’s closely related to, albeit not really the same as, the feeling of touching the Divine—which is partly why I keep returning to browse its publications every now and then.

<a name="#The-evolved-ear"></a>
### The evolved ear
([overview](#overview)) 

These weren't just ears, they were pH sensors and magnetism detectors, all not explicitly designed. What the hell...

In [the evolved radio](#the-evolved-radio) I quoted the following passage:

```markdown
This paper details an unconstrained, intrinsic HE experiment where a network of 
transistors sensed and utilised the radio waves emanating from a nearby PC. 
Essentially, the EA led to the construction of a radio. This is, as far as the authors
know, only the second example of a physical device whose sensors were constructed by a 
process analogous to that of phylogenetic change. We compare the circuit to the first 
device constructed in this way: Gordon Pask’s electrochemical ear.
```

Naturally I had to look up Pask's evolved ear. 

Turns out the summary is *fascinating*. Note that this was sixty years ago—talk of a field of research “not being mature enough to absorb a particular contribution”, which seems to crop up in math a lot, feels more apropos here (although othat's probably just my ignorance talking).

Pask's devices sounded nothing like AI -- they were pure hardware, indeed pure electrochemistry:

```markdown
In 1958 Gordon Pask demonstrated a number of remarkable mechanisms that were able to 
construct novel sensors and thereby determine the relations between their own states 
and the environment. In other words, these devices were able to generate and explore 
their own state space. Any observer trying to model the behaviour of these devices 
would be forced to change the dimensionality of their model over time as the devices 
can transform the underlying generative system.

The devices are electrochemical assemblages consisting of a number of small platinum 
electrodes that are inserted in a dish of ferrous sulphate solution and connected to 
a current limited electrical source. Depending on the activity of the system, these 
electrodes can act as sinks or sources of current. Metallic iron threads tend to form
between electrodes where maximum lines of current are flowing. These metallic threads
have a low resistance relative to the solution and so current will tend to flow down 
them if the electrical activation is repeated. Consequently, the potentials at the 
electrodes are modified by the formation of threads. If no current passes through a
thread, then it tends to dissolve back into the acidic solution. 

The system therefore fundamentally consists of two opposing processes: one which builds
metallic threads out of ions on relatively negative electrodes (sinks); and one that
dissolves metallic threads back into ions. The trial and error process of thread
development is also constrained by the concurrent development of neighbouring threads
and also by previously developed structures. Slender branches extend from a thread in
many directions and most of these dissolve except for the one following the path of 
maximum current. If there is an ambiguous path then a thread can bifurcate. 

As the total current entering the system is restricted, threads compete for resources.
However, when there are a number of neighbouring unstable structures, the threads can
amalgamate and form one cooperative structure. Over time a network of threads can form 
that is dynamically stable: the electrochemical mechanism literally *grows*.

It is possible to associate some of the electrodes with output devices that enable the
behaviour of the system to be assessed by a user. A reward consists of an increase in 
the limited current supply to the assemblage and is therefore a form of positive 
reinforcement. Regardless of how the electrodes are configured, the assemblage will
develop a thread structure that leads to current flowing in such a way that the user 
rewards the system. Importantly, the reward is simply an increased capacity for growth 
and there is not any specification of what form it should take.

Critically, the system is not just electrically connected to the external world: due to 
the physical nature of the components, thread formation is also sensitive to temperature,
chemical environment, vibrations and magnetic fields. Any of these arbitrary disturbances
can be viewed as an input to the system, especially if they affect the performance of the
mechanism so that its current supply is changed. The system can grow structures that are
sensitive to different environmental stimuli. 

Pask was able to train an assemblage to act as an ‘ear’ that could discriminate between 
a 50 Hz and 100 Hz tone in about half a day. He was also able to grow a system that could
detect magnetism and one that was sensitive to pH differences. The development of sensors
constitutes a change in the state space of the assemblage that was not specified by a
designer explicitly.
```
