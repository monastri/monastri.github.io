### Overview

I've sorted the quotes below into the following provisional categories:

1. General intelligence
2. Miscellaneous
3. [link](#misc)

## General intelligence

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

<a name="misc"></a>

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


## Miscellaneous

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
