*[Word count](https://wordcounter.net/): 15,100*

## What is this?

This is the "artificial intelligence and life" section of [this notebook](https://monastri.github.io/). 

<a name="#overview"></a>

## Overview

I've sorted the quotes below into the following categories. This is a provisional taxonomy, subject to perpetual refactoring. The reason it has a [Borgesian flavor](https://github.com/monastri/monastri.github.io/blob/master/poetry.md#the-celestial-emporium-of-benevolent-knowledge) is that it's meant to aid recall and idea-building. The categories are ordered alphabetically; the actual quotes (the top-level categories that is) are chronologically added.

1. [Animals are not like us](#animals-are-not-like-us)
2. [ChinAI](#ChinAI)
2. [Digital evolution and artificial life](#Digital-evolution-and-artificial-life)
	1. [The evolved radio](#The-evolved-radio)
	2. [The evolved ear](#The-evolved-ear)
1. [Evolution](#evolution)
	1. [Evolution as alien god](#evolution-as-alien-god), where I first learned that there are many evolutions, as many as reproducing populations
	1. [Gene-centered view](#gene-centered-view)	
2. [Levels of Organization in General Intelligence](#Levels-of-Organization-in-General-Intelligence)
2. [Microbiology](#Microbiology)
	1. [Cells are very fast and crowded places](#Cells-are-very-fast-and-crowded-places)
3. [Machine learning and statistical inference](#Machine-learning)
	2. [Deep learning](#Deep-learning)
		1. [Limitations of deep learning](#Deep-learning-limitations)
	2. [Program synthesis](#Program-synthesis)
3. [Why are we trichromats, and not say tetrachromats?](#why-we-are-trichromats)
3. [Xenology](#Xenology)
   
---------------------------------

<a name="#ChinAI"></a>
## ChinAI
([overview](#overview))

From Jeffrey Ding's [What I Learned from a Year of ChinAI](https://chinai.substack.com/). Jeff is a grad student at Oxford's Center for the Governance of AI, Future of Humanity Institute. 

What is this? How and why did it start?

```markdown
These are Jeff Ding's (sometimes) weekly translations of writings on AI policy and
strategy from Chinese thinkers. I'll also include general links to all things at the
intersection of China and AI.

I started ChinAI with an email to a small group of colleagues and friends with chapter
translations of a book co-authored by Tencent and a Chinese gov’t think tank on a
National Strategic Initiative on AI. ...

...my hope is that other researchers and translators can use this as a platform to 
share their work.
```

Apparently Ding's newsletter is affiliated with the Center for the Governance of AI at Oxford’s Future of Humanity Institute, and "has been pumped up" by Miles Brundage. 

Key takeaways:

1. There is a language asymmetry in the Chinese-speaking community’s understanding of the global AI landscape and that of the English-speaking community.
2. Western observers consistently overinflate Chinese AI capabilities. While some of this exaggeration is a product of media sensationalism or deliberate overestimation on the part of interest groups to drive momentum for their own agenda, another significant factor behind the overinflation is a misunderstanding of what is happening at the technical level of AI development in Chinese companies.
3. In addition to AI’s significance for economic growth and military security, the Chinese government sees AI as a tool to improve social governance, which makes public security applications a large driver of China’s AI development. This also means that some Chinese AI companies are complicit with China’s mass surveillance of Xinjiang, an effort that disproportionately targets ethnic Uyghurs.

Language asymmetry in the Chinese-speaking community’s understanding of the global AI landscape and that of the English-speaking community:

```markdown
Big developments covered in Western outlets — the publication of the Malicious Use
of AI report, any breakthrough made by Deepmind or OpenAI, an op-ed about human-
centered AI by Fei-fei Li — are translated within a day or two and analyzed in Chinese
outlets. This short turnaround time is a product of a China’s vigorously competitive
and quickly expanding S&T (science and technology) media landscape. Many of my
translations this year drew from outlets such as xinzhiyuan, Leiphone, and jiqizhixin,
many of which are outpacing their Western outlets in terms of output of content and 
scale.

Andrew Ng referenced a similar language asymmetry with regards to AI technical research
in an article in The Atlantic:

	The language issue creates a kind of asymmetry: Chinese researchers usually
	speak English so they have the benefit of access to all the work disseminated
	in English. The English-speaking community, on the other hand, is much less
	likely to have access to work within the Chinese AI community.
	
I think the growth of ChinAI in this past year is proof that there is a demand from the 
English-speaking world for a deeper awareness of what’s happening in the Chinese-
speaking world, and I hope more people and organizations work to rebalance this language
asymmetry.	
```

Western observers consistently overinflate Chinese AI capabilities, due to media sensationalism or deliberate overestimation on the part of interest groups to drive momentum for their own agenda, also a misunderstanding of what is happening at the technical level of AI development in Chinese companies:

```markdown
In a year that featured the rise of the “AI arms race” meme and headlines like 
“China’s tech giants spending more on AI than Silicon Valley,” few people dug 
underneath the hood to see what China’s so-called AI giants, such as Tencent, were
actually doing regarding AI at the technical level. One exception was a Chinese-
language essay by Li Guofei, a widely respected thinker in China’s investment 
community, which drew on interviews with Tencent insiders. It revealed that 
Tecent’s algorithms “still give a very imprecise profile of users” because
“Tencent’s customer data is scattered in various departments and has become the
‘private property’ of departments” (e.g. WeChat’s advertising algorithms are not
under the purview of the WeChat department but are actually under another
department which does not have access to the data of the WeChat team). Moreover,
the number of Tencent engineers solely dedicated to doing work on improving 
algorithms is “pitifully few” according to Li, and each unit has its own algorithm
engineers so there’s also a lot of low-level, redundant development of algorithms.

Another piece by a writer for Huxiu, a Chinese-language platform for sharing news 
and thinkpieces on S&T issues, argued that, “Only Baidu and Huawei are Really
Doing AI.” It divided the 190 major AI companies that make up China’s AI ecosystem
into three layers (application, technology, and foundation), but found that 
China’s four tech giants (Baidu, Alibaba, Tencent, and Huawei) had promoted a top-
heavy AI industry with few companies producing the foundational technologies (e.g.
deep learning frameworks and chips) that underpin AI development.
```

In addition to AI’s significance for economic growth and military security, the Chinese government sees AI as a tool to improve social governance:

```markdown
According to a report by Yiou intelligence, a consulting firm that publishes reports 
in Mandarin on China’s industry, security + AI companies accounted for the highest
proportion of companies in Yiou’s list of top 100 AI companies. AI startups like 
Mininglamp are positioning themselves as the “Palantir of China” by integrating their
products with public security departments and collaborating with the police to crack
cases related to the production and sales of fake vaccines.

Two of China’s most successful facial recognition startups, Sensetime, and Megvii
(Face++), are involved in China’s efforts to securitize Xinjiang. At the 2017 China-
Eurasia Security Expo, Megvii (Face++) was announced as an official technical support
unit of the Public Security Video Laboratory in Xinjiang. Under the backdrop of the
“Silk Road Economic Belt,” expos like these enable the export of China’s surveillance
technology to Central Asian countries and beyond, as nearly 100 government agencies, 
experts, and procurement companies attended. The 2018 edition of expo featured the 
announcement of a joint venture company called Tang Li Technology by Sensetime and 
Leon Technology, a security systems integrator company that claims it is responsible 
for 50% of "safe city" projects in Urumqi, the capital of Xinjiang, as well as the 
maintenance of surveillance infrastructure for the border between Xinjiang and
neighboring countries. It is also important to be precise about the technical 
capabilities of the security systems actually in implementation, as there are limits
to continuous real-time location tracking due to limitations of facial recognition 
technology, camera costs, and constraints to compute power.
```

<a name="#Microbiology"></a>
## Microbiology
([overview](#overview))

<a name="#Cells-are-very-fast-and-crowded-places"></a>
### Cells are very fast and crowded places
([overview](#overview))

From the [eponymous blog post](http://www.righto.com/2011/07/cells-are-very-fast-and-crowded-places.html) by computer historian/old-school electronic engineer Ken Shirriff -- do visit his page for videos and illustrations!

Cells are packed:

```markdown
I recently learned that cells are extremely crowded and busy places. I knew there's 
a lot of activity in cells, but I didn't realize just how much until I was reading 
*Molecular Biology of the Cell*. ...

I imagined cells as big open spaces with lots of stuff happening, perhaps something 
like Central Park. From the "Inner Life of a Cell" video, or the typical drawing of 
a cell, it looks like a lot of empty space. But it turns out that cells are crammed 
full of stuff, more like New Year's Eve at Times Squares. Proteins are packed tightly
into cells.

I came across another interesting representation of how crowded cells are. This 
diagram shows a synaptic vesicle, which is the part of a neuron that releases 
neurotransmitters from one neuron to another. When I saw this diagram, I assumed that
the authors crammed all the different proteins into the picture so they could create
a nice illustration of the different membrane proteins. But in fact, the diagram below
omits 1/3 of the proteins so real membranes are even more crowded. The paper 
containing this diagram states that instead of thinking of membranes with proteins 
floating in them like icebergs, we should think of membranes as packed with proteins
like a cobblestone pavement. 
```

Intracellular stuff moves fast:

```markdown
You may wonder how things get around inside cells if they are so crowded. It turns out
that molecules move unimaginably quickly due to thermal motion. A small molecule such
as glucose is cruising around a cell at about 250 miles per hour, while a large protein
molecule is moving at 20 miles per hour. Note that these are actual speeds inside the 
cell, not scaled-up speeds. I'm not talking about driving through a crowded Times 
Square at 20 miles per hour; to scale this would be more like driving through Times 
Square at 20 million miles per hour!

Because cells are so crowded, molecules can't get very far without colliding with 
something. In fact, a molecule will collide with something billions of times a second 
and bounce off in a different direction. Because of this, molecules are doing a random 
walk through the cell and diffusing all around. A small molecule can get from one side 
of a cell to the other in 1/5 of a second.

As a result of all this random motion, a typical enzyme can collide with something to 
react with 500,000 times every second. Watching the video, you might wonder how the
different pieces just happen to move to the right place. In reality, they are covering
so much ground in the cell so fast that they will be in the "right place" very 
frequently just by chance.

In addition, a typical protein is tumbling around, a million times per second. Imagine 
proteins crammed together, each rotating at 60 million RPM, with molecules slamming 
into them billions of times a second. This is what's going on inside a cell.

The incredible speed and density of cells also helps explain why it's so difficult to 
simulate what's happening inside a cell. Even with a supercomputer, there's way too much
going on inside a cell to simulate it without major simplifications. Even simulating a 
single ribosome is a huge computational challenge.

Another thing that surprised me about cells is how fast the motors inside cells move. 
Like a mechanical robot with two lumbering feet, a kinesin motor protein can be seen in
the video at the 2 minute mark dragging a monstrous bag-like vesicle along a microtubule
track. These motor proteins move cargo through the cell if diffusion isn't fast enough to
get things to their destination, which is especially important in extremely long cells 
such as neurons. Kinesin motors also help separate cells that are dividing.

It's remarkable enough that cells contain these mechanical walkers, but I recently learned 
that they aren't plodding along, but actually sprint at 100 steps per second. If you watch 
the video again, imagine it sped up to that rate.

Mitochondria also provide a fascinating look at just how fast things are inside cells. You
may know that mitochondria are the power plants of cells; they take in food molecules, 
process it through the famous citric acid cycle, and then use oxygen to extract more energy,
which is provided to the rest of the cell through molecules of ATP, the cell's "energy 
currency".

Mitochondria have many strange features - such as their own DNA separate from the cell's - 
but one of their strangest features is they use electric motors to produce ATP. Mitochondria
use the energy from oxidizing food to pump protons out of the cell, creating a voltage of 
170mV across the cell. This voltage causes a complex enzyme to spin, and the mechanical 
energy of this spinning enzyme creates the ATP molecules that energize the rest of the cell.

Watching the leisurely turning enzymes illustrates one of the amazingly complex mechanisms in
a cell. But what really surprised me was to learn that in real life, these enzymes spin at up
to 700 revolutions per second, which is faster than a jet engine. 
```

<a name="#Machine-learning"></a>
## Machine learning
([overview](#overview))

From Alex Clemmer's [What exactly is the difference between machine learning and statistics?](http://blog.nullspace.io/ml-vs-stats.html). 

Alex espouses the view that ML is "a computational interpretation of statistical inference:

```markdown
To say they’re completely equivalent (which is what I often hear) is probably a 
bit too strong. 

I tend to think of ML as mostly a contribution to the general problem of
statistical inference, particularly as it is applied computationally. 

In contrast, statistics as a field is certainly not entirely devoted to inference.
```

This contextualizes the idiosyncratic differences between ML and stats:

```markdown
Unlike statistics, there are very few ideas that really “unite” ML as a field. 
People seem to have split up work into a set of common tasks (e.g., 
classification, clustering, reinforcement learning), and these tasks really 
only seem to be unified by the fact that they depend on statistical inference.

Statistics tends to focus on longer journal publications, which are heavy on 
mathematics and theoretical analysis. ML tends to focus on shorter publications
at conferences, with empiricism (especially in explaining methodology and
evaluation of results) playing a much bigger role.

Distinctions important to statistical theory (e.g., whether a procedure is 
frequentist or Bayesian) are often not emphasized or are totally absent from 
discussion in ML. In a lot of cases, this is because the discussion of the
empirical results is emphasized, so discussion about the different types of
guarantees given by different theoretical assumptions becomes less meaningful
because the theoretical analysis and guarantees are not given as much play to 
begin with.

ML people tend to import globs of statistics literature as it helps them to 
accomplish the tasks they care about. It is sometimes said that ML is a
computational interpretation of statistical inference, and this is not hard to
see that this is mostly a fair assessment.
```

Or in short:

```markdown
Statisticians care a lot about things like “asymptotics”, “guarantees”, and 
“math.” Machine learning people care a lot about things like “methodology” and
“how do I *actually do* this statistical inference with a computer.”
```

Yeah okay, but what *is* statistical inference? (Should this go under the "stats" subsection?)

```markdown
Statistical inference generally involves inferring some quantity based on some 
set of statistics.

For example, say I have a bin with some number of black balls and white balls 
in it. I draw one at random and show it to you. How many times do I need to 
repeat this before you can accurately estimate the number of ball in the bin?

Statistics! It’s magic!

Of course this is a simple example. Generally you’re doing something dramatically
more complicated.
```

Hm. What's a model again?

```markdown
A model is a concise summary of data that simply retains some statistical property
of the data that you care about. These summaries that “model” your data can be 
used for any number of things:

1. **To simply tell you about the behavior of your data**. For example, the mean is a
model. If you imaging picking numbers at random from 1-10, a mean does summarize 
some useful information about your data. The same with the median and the variance.
These are extremely lossy models, but they are models of your data.

2. **To classify data**. Say you’ve trained a classifier that classifies whether a photo 
contains a cat or not. That classifier concisely summarizes your data as “cat 
photo” or “non-cat photo.”

3. **As a more space-efficient way to represent data for some other task**. For example, 
you might generate paraphrases of some document, and then use that paraphrase to 
classify a document. Or you might present it to a user. etc.

This goes on and on. It also gets dramatically more complicated, of course, but the
idea that we’re providing a concise summary of the data is always true.
```

Why use ML? To save time:

```markdown
Machine learning doesn’t give you perfect answers, but sometimes it can save you a lot 
of time.

For example, some time in 2011, thousands of Sarah Palin’s emails were released. If you
were a reporter, you could read all the emails yourself, or you could hire someone like
Edwin Chen to do machine learning magic to automatically discover all the topics she 
talked about.

Were the topics perfect? Absolutely not; some of them were junk. But would they have 
saved you a lot of time reading? Absolutely.

There are lots of other examples, too. If you’re a programmer, and you want to implement
an algorithm that detects if there’s a cow in a picture, you could write an algorithm, 
or you could get it mostly right most of the time, and just use machine learning.
```

When *not* to use ML? Some heuristics:

```markdown
The first heuristic is two parts. If one of the following is not true, then you might
still be able to use machine learning to solve your problem. But, if neither of the 
following is true, then machine learning probably can’t help you. The heuristic is:

1. If I give all your data to a real person, can they find a pattern?
2. If I give a person your pattern, is it meaningful to them?

So take an example like search engines. If I ask a law librarian to find all relevant
cases for something, they will usually produce good work. Likewise, if a search engine 
produces results for me, I can quickly determine if they’re good or not.

So, at the very least it satisfies both these criteria. And indeed, as we all probably 
know, machine learning has helped search engines along.

In contrast, take music recommendations. If I give you a series of suggested songs, 
can you detect a pattern? If you give a list of your favorite songs to even a really
good friend, can they generate a list of recommendations? I mean, maaaaaaaayyybe they
can, but a lot of times, they can’t. Like, I listen to Bach and also stuff like 
Dillinger Escape Plan. So good luck predicting what else I’ll like.

And this bears out with the rule above. Looking at content recommendation sites, it 
is obvious that machine learning might save you a bit of time, and it might generate
interesting suggestions, but really it’s not so much that the recommendations are 
good as it is that the recommendations are better than nothing.

Of course, it should be noted that if your task passes the above criteria it does not
mean it can or should be solved with machine learning. For example, it takes a lot of 
work to make a good search engine. Those questions only help you throw out a large 
number of possible problems you might approach using machine learning.

Another good question to ask is:

- Can this problem be solved by looking at statistical outcomes?

Actually the answer is “yes” surprisingly often, like in the case of inferring topics
in Sarah Palin’s email (see above). But that was a surprising result even when it came
out. And it is certainly not always true, so when starting out, you should pause and 
think, “ok, but what is the statistical nature of this?”

Avoid it if you can. But a particularly bad time to use it is when you can describe
the phenomenon precisely using some mathematical equation. So, for example, you 
wouldn’t use machine learning to predict when a dropped ball is going to hit the 
ground, because you already know that from math.
```

<a name="#Program-synthesis"></a>
### Program synthesis
([overview](#overview))

Francois Chollet is a great explainer. Here's how he talks about program synthesis in his essay [The future of deep learning](https://blog.keras.io/the-future-of-deep-learning.html):

```markdown
Program synthesis consists in automatically generating simple programs, by using a
search algorithm (possibly genetic search, as in genetic programming) to explore a
large space of possible programs. The search stops when a program is found that 
matches the required specifications, often provided as a set of input-output pairs.
As you can see, is it highly reminiscent of machine learning: given "training data"
provided as input-output pairs, we find a "program" that matches inputs to outputs 
and can generalize to new inputs. The difference is that instead of learning 
parameter values in a hard-coded program (a neural network), we generate source 
code via a discrete search process.
```

<a name="#Deep-learning"></a>
### Deep learning
([overview](#overview))

Francois Chollet is a great explainer. Here's how he talks about deep learning in his essay [The limitations of deep learning](https://blog.keras.io/the-limitations-of-deep-learning.html):

```markdown
The most surprising thing about deep learning is how simple it is. Ten years ago,
no one expected that we would achieve such amazing results on machine perception
problems by using simple parametric models trained with gradient descent. Now, it
turns out that all you need is *sufficiently large* parametric models trained with
gradient descent on *sufficiently many* examples. As Feynman once said about the 
universe, "It's not complicated, it's just a lot of it".

In deep learning, everything is a vector, i.e. everything is a point in a geometric
space. Model inputs (it could be text, images, etc) and targets are first "vectorized",
i.e. turned into some initial input vector space and target vector space. Each layer
in a deep learning model operates one simple geometric transformation on the data that
goes through it. Together, the chain of layers of the model forms one very complex 
geometric transformation, broken down into a series of simple ones. This complex 
transformation attempts to maps the input space to the target space, one point at a
time. This transformation is parametrized by the weights of the layers, which are 
iteratively updated based on how well the model is currently performing. A key
characteristic of this geometric transformation is that it must be differentiable,
which is required in order for us to be able to learn its parameters via gradient 
descent. Intuitively, this means that the geometric morphing from inputs to outputs 
must be smooth and continuous—a significant constraint.

The whole process of applying this complex geometric transformation to the input 
data can be visualized in 3D by imagining a person trying to uncrumple a paper ball:
the crumpled paper ball is the manifold of the input data that the model starts with.
Each movement operated by the person on the paper ball is similar to a simple 
geometric transformation operated by one layer. The full uncrumpling gesture sequence
is the complex transformation of the entire model. Deep learning models are
mathematical machines for uncrumpling complicated manifolds of high-dimensional data.

That's the magic of deep learning: turning meaning into vectors, into geometric
spaces, then incrementally learning complex geometric transformations that map one 
space to another. All you need are spaces of sufficiently high dimensionality in 
order to capture the full scope of the relationships found in the original data.
```

<a name="#Deep-learning-limitations"></a>
### Deep learning limitations
([overview](#overview))

Francois Chollet is a great explainer. Here's how he talks about the limitations of deep learning in his essay [The limitations of deep learning](https://blog.keras.io/the-limitations-of-deep-learning.html) -- in particular, reasoning, long-term planning and algo-like data manipulation are all out of reach:

```markdown
The space of applications that can be implemented with this simple strategy is 
nearly infinite. And yet, many more applications are completely out of reach for
current deep learning techniques—even given vast amounts of human-annotated data.
Say, for instance, that you could assemble a dataset of hundreds of thousands—even
millions—of English language descriptions of the features of a software product, 
as written by a product manager, as well as the corresponding source code
developed by a team of engineers to meet these requirements. Even with this data,
you could not train a deep learning model to simply read a product description and 
generate the appropriate codebase. That's just one example among many. In general,
anything that requires reasoning—like programming, or applying the scientific 
method—long-term planning, and algorithmic-like data manipulation, is out of reach
for deep learning models, no matter how much data you throw at them. Even learning
a sorting algorithm with a deep neural network is tremendously difficult.

This is because a deep learning model is "just" a chain of simple, continuous 
geometric transformations mapping one vector space into another. All it can do is 
map one data manifold X into another manifold Y, assuming the existence of a 
learnable continuous transform from X to Y, and the availability of a dense 
sampling of X:Y to use as training data. So even though a deep learning model can 
be interpreted as a kind of program, inversely most programs cannot be expressed 
as deep learning models—for most tasks, either there exists no corresponding 
practically-sized deep neural network that solves the task, or even if there exists
one, it may not be learnable, i.e. the corresponding geometric transform may be far
too complex, or there may not be appropriate data available to learn it.

Scaling up current deep learning techniques by stacking more layers and using more
training data can only superficially palliate some of these issues. It will not
solve the more fundamental problem that deep learning models are very limited in
what they can represent, and that most of the programs that one may wish to learn 
cannot be expressed as a continuous geometric morphing of a data manifold.
```

Chollet continues by talking about local generalization (what DL does) versus extreme generalization (what we do):

```markdown
There just seems to be fundamental differences between the straightforward 
geometric morphing from input to output that deep learning models do, and the
way that humans think and learn. It isn't just the fact that humans learn by 
themselves from embodied experience instead of being presented with explicit 
training examples. Aside from the different learning processes, there is a 
fundamental difference in the nature of the underlying representations.

Humans are capable of far more than mapping immediate stimuli to immediate 
responses, like a deep net, or maybe an insect, would do. They maintain complex,
abstract models of their current situation, of themselves, of other people, and
can use these models to anticipate different possible futures and perform long-
term planning. They are capable of merging together known concepts to represent
something they have never experienced before—like picturing a horse wearing
jeans, for instance, or imagining what they would do if they won the lottery. 
This ability to handle hypotheticals, to expand our mental model space far
beyond what we can experience directly, in a word, to perform abstraction and 
reasoning, is arguably the defining characteristic of human cognition. I call it
"extreme generalization": an ability to adapt to novel, never experienced before
situations, using very little data or even no new data at all.

This stands in sharp contrast with what deep nets do, which I would call "local
generalization": the mapping from inputs to outputs performed by deep nets
quickly stops making sense if new inputs differ even slightly from what they saw 
at training time. Consider, for instance, the problem of learning the appropriate
launch parameters to get a rocket to land on the moon. If you were to use a deep
net for this task, whether training using supervised learning or reinforcement 
learning, you would need to feed it with thousands or even millions of launch 
trials, i.e. you would need to expose it to a dense sampling of the input space,
in order to learn a reliable mapping from input space to output space. By 
contrast, humans can use their power of abstraction to come up with physical 
models—rocket science—and derive an exact solution that will get the rocket on the
moon in just one or few trials. Similarly, if you developed a deep net controlling
a human body, and wanted it to learn to safely navigate a city without getting hit
by cars, the net would have to die many thousands of times in various situations 
until it could infer that cars and dangerous, and develop appropriate avoidance 
behaviors. Dropped into a new city, the net would have to relearn most of what it
knows. On the other hand, humans are able to learn safe behaviors without having 
to die even once—again, thanks to their power of abstract modeling of hypothetical
situations.

In short, despite our progress on machine perception, we are still very far from
human-level AI: our models can only perform local generalization, adapting to new 
situations that must stay very close from past data, while human cognition is 
capable of extreme generalization, quickly adapting to radically novel situations,
or planning very for long-term future situations.
```

So how might we improve on these limitations? Chollet says we need models capable of abstraction and reasoning (per above). Yeah, like what? Like RNNs, which are "a bit more than a mere geometric transformation: they are geometric transformations *repeatedly applied inside a for loop*":

```markdown
Current AI programs that are capable of basic forms of reasoning are all hard-coded
by human programmers: for instance, software that relies on search algorithms, graph 
manipulation, formal logic. In DeepMind's AlphaGo, for example, most of the 
"intelligence" on display is designed and hard-coded by expert programmers (e.g. Monte-
Carlo tree search); learning from data only happens in specialized submodules (value
networks and policy networks). But in the future, such AI systems may well be fully
learned, with no human involvement.

What could be the path to make this happen? Consider a well-known type of network: 
RNNs. Importantly, RNNs have slightly less limitations than feedforward networks. 
That is because RNNs are a bit more than a mere geometric transformation: they are 
geometric transformations repeatedly applied inside a for loop. The temporal for loop
is itself hard-coded by human developers: it is a built-in assumption of the network.
Naturally, RNNs are still extremely limited in what they can represent, primarily
because each step they perform is still just a differentiable geometric transformation,
and the way they carry information from step to step is via points in a continuous
geometric space (state vectors). Now, imagine neural networks that would be "augmented"
in a similar way with programming primitives such as for loops—but not just a single
hard-coded for loop with a hard-coded geometric memory, rather, a large set of 
programming primitives that the model would be free to manipulate to expand its
processing function, such as if branches, while statements, variable creation, disk 
storage for long-term memory, sorting operators, advanced datastructures like lists,
graphs, and hashtables, and many more. The space of programs that such a network could
represent would be far broader than what can be represented with current deep learning 
models, and some of these programs could achieve superior generalization power.

In a word, we will move away from having on one hand "hard-coded algorithmic 
intelligence" (handcrafted software) and on the other hand "learned geometric 
intelligence" (deep learning). We will have instead a blend of formal algorithmic
modules that provide reasoning and abstraction capabilities, and geometric modules
that provide informal intuition and pattern recognition capabilities. The whole 
system would be learned with little or no human involvement.
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

<a name="#animals-are-not-like-us"></a>
## Animals are not like us
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

<a name="#evolution"></a>
## Evolution
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

<a name="#evolution-as-alien-god"></a>
### Evolution as alien god
([overview](#overview))	

From Eliezer Yudkowsky's [epomymously titled LW essay](https://www.lesswrong.com/posts/pLRogvJLPPg6Mrvg4/an-alien-god), which pretty much set the template for how I think about evolution all those years back:

```markdown
A human being, looking at the natural world, sees a thousand times *purpose*. 
A rabbit's legs, built and articulated for running; a fox's jaws, built and 
articulated for tearing. But what you see is not exactly what is there...

In the days before Darwin, the cause of all this apparent *purposefulness* was
a very great puzzle unto science. The Goddists said "God did it", because you 
get 50 bonus points each time you use the word "God" in a sentence. Yet perhaps
I'm being unfair. In the days before Darwin, it seemed like a much more
reasonable hypothesis. Find a watch in the desert, said William Paley, and you
can infer the existence of a watchmaker.

But when you look at *all* the apparent purposefulness in Nature, rather than
picking and choosing your examples, you start to notice things that don't fit 
the Judeo-Christian concept of one benevolent God. Foxes seem well-designed to
catch rabbits. Rabbits seem well-designed to evade foxes. Was the Creator having
trouble making up Its mind?

When I design a toaster oven, I don't design one part that tries to get
electricity to the coils and a second part that tries to prevent electricity from
getting to the coils. It would be a waste of effort. Who designed the ecosystem,
with its predators and prey, viruses and bacteria? Even the cactus plant, which
you might think well-designed to provide water fruit to desert animals, is 
covered with inconvenient spines.

The ecosystem would make much more sense if it wasn't designed by a unitary Who,
but, rather, created by a horde of deities—say from the Hindu or Shinto religions.
This handily explains both the ubiquitous purposefulnesses, and the ubiquitous
conflicts: More than one deity acted, often at cross-purposes. The fox and rabbit 
were both designed, but by distinct competing deities. ...

Similarly, the Judeo-Christian God is alleged to be benevolent—well, sort of.
And yet much of nature's purposefulness seems downright cruel. Darwin suspected 
a non-standard Creator for studying Ichneumon wasps, whose paralyzing stings
preserve its prey to be eaten alive by its larvae: "I cannot persuade myself,"
wrote Darwin, "that a beneficent and omnipotent God would have designedly
created the Ichneumonidae with the express intention of their feeding within the
living bodies of Caterpillars, or that a cat should play with mice." ...

Evolution doesn't allow just any kind of purposefulness to leak into Nature. 
That's what makes evolution a success as an empirical hypothesis. If evolutionary
biology could explain a toaster oven, not just a tree, it would be worthless. 
There's a lot more to evolutionary theory than pointing at Nature and saying, 
"Now purpose is allowed," or "Evolution did it!" The strength of a theory is not
what it allows, but what it prohibits; if you can invent an equally persuasive
explanation for any outcome, you have zero knowledge.

"Many non-biologists," observed George Williams, "think that it is for their
benefit that rattles grow on rattlesnake tails." Bzzzt! This kind of purposefulness
is not allowed. Evolution doesn't work by letting flashes of purposefulness creep
in at random—reshaping one species for the benefit of a random recipient.

Evolution is powered by a systematic correlation between the different ways that
different genes construct organisms, and how many copies of those genes make it
into the next generation. For rattles to grow on rattlesnake tails, rattle-
growing genes must become more and more frequent in each successive generation.
(Actually genes for incrementally more complex rattles, but if I start describing
all the fillips and caveats to evolutionary biology, we really will be here all 
day.)

There isn't an Evolution Fairy that looks over the current state of Nature, 
decides what would be a "good idea", and chooses to increase the frequency of 
rattle-constructing genes.

I suspect this is where a lot of people get stuck, in evolutionary biology. They 
understand that "helpful" genes become more common, but "helpful" lets any sort 
of purpose leak in. They don't think there's an Evolution Fairy, yet they ask 
which genes will be "helpful" as if a rattlesnake gene could "help" non-rattlesnakes.

The key realization is that *there is no Evolution Fairy*. There's no outside force
deciding which genes ought to be promoted. Whatever happens, happens *because* of 
the genes themselves.

Genes for constructing (incrementally better) rattles, must have somehow ended up
more frequent in the rattlesnake gene pool, because of the rattle. In this case it's
probably because rattlesnakes with better rattles survive more often—rather than 
mating more successfully, or having brothers that reproduce more successfully, etc.

Maybe predators are wary of rattles and don't step on the snake. Or maybe the 
rattle diverts attention from the snake's head.

But that's just a snake's rattle. There are much more complicated ways that a 
gene can cause copies of itself to become more frequent in the next generation.
Your brother or sister shares half your genes. A gene that sacrifices one unit of
resources to bestow three units of resource on a brother, may promote some copies
of itself by sacrificing one of its constructed organisms. 

The main point is that the gene's effect must cause copies of that gene to become
more frequent in the next generation. There's no Evolution Fairy that reaches in 
from outside. There's nothing which decides that some genes are "helpful" and should,
therefore, increase in frequency. It's just cause and effect, starting from the
genes themselves.

This explains the strange conflicting purposefulness of Nature, and its frequent
cruelty. It explains even better than a horde of Shinto deities.

Why is so much of Nature at war with other parts of Nature? Because there isn't 
one Evolution directing the whole process. There's as many different "evolutions"
as reproducing populations. Rabbit genes are becoming more or less frequent in 
rabbit populations. Fox genes are becoming more or less frequent in fox populations.
Fox genes which construct foxes that catch rabbits, insert more copies of themselves
in the next generation. Rabbit genes which construct rabbits that evade foxes are 
naturally more common in the next generation of rabbits. Hence the phrase "natural
selection".

Why is Nature cruel? You, a human, can look at an Ichneumon wasp, and decide that
it's cruel to eat your prey alive. You can decide that if you're going to eat your
prey alive, you can at least have the decency to stop it from hurting. It would 
scarcely cost the wasp anything to anesthetize its prey as well as paralyze it. Or
what about old elephants, who die of starvation when their last set of teeth fall 
out? These elephants aren't going to reproduce anyway. What would it cost evolution—
the evolution of elephants, rather—to ensure that the elephant dies right away, 
instead of slowly and in agony? What would it cost evolution to anesthetize the
elephant, or give it pleasant dreams before it dies? Nothing; that elephant won't 
reproduce more or less either way.

If you were talking to a fellow human, trying to resolve a conflict of interest, 
you would be in a good negotiating position—would have an easy job of persuasion.
It would cost so little to anesthetize the prey, to let the elephant die without 
agony! Oh please, won't you do it, kindly... um...

There's no one to argue with.

Humans, who are often deeply concerned for the well-being of animals, can be very 
persuasive in arguing how various kindnesses wouldn't harm reproductive fitness at
all. Sadly, the evolution of elephants doesn't use a similar algorithm; it doesn't
select nice genes that can plausibly be argued to help reproductive fitness. Simply:
genes that replicate more often become more frequent in the next generation. Like 
water flowing downhill, and equally benevolent.

A human, looking over Nature, starts thinking of all the ways we would design 
organisms. And then we tend to start rationalizing reasons why our design 
improvements would increase reproductive fitness—a political instinct, trying to 
sell your own preferred option as matching the boss's favored justification.

And so, amateur evolutionary biologists end up making all sorts of wonderful and 
completely mistaken predictions. Because the amateur biologists are drawing their
bottom line—and more importantly, locating their prediction in hypothesis-space—
using a different algorithm than evolutions use to draw their bottom lines.

A human engineer would have designed human taste buds to measure how much of each 
nutrient we had, and how much we needed. When fat was scarce, almonds or 
cheeseburgers would taste delicious. But if you started to become obese, or if 
vitamins were lacking, lettuce would taste delicious. But there is no Evolution of
Humans Fairy, which intelligently planned ahead and designed a general system for
every contingency. It was a reliable invariant of humans' ancestral environment
that calories were scarce. So genes whose organisms loved calories, became more 
frequent. Like water flowing downhill.

We are simply the embodied history of which organisms *did in fact* survive and 
reproduce, not which organisms *ought prudentially to have* survived and reproduced.
```

And here's the memorable "alien god" part:

```markdown
Find a watch in a desert, said William Paley, and you can infer the watchmaker.
There were once those who denied this, who thought that life "just happened" without
need of an optimization process, mice being spontaneously generated from straw and 
dirty shirts.

If we ask who was *more* correct—the theologians who argued for a Creator-God, or 
the intellectually unfulfilled atheists who argued that mice spontaneously generated—
then the theologians must be declared the victors: evolution is not God, but it is
closer to God than it is to pure random entropy. Mutation is random, but selection 
is non-random. This doesn't mean an intelligent Fairy is reaching in and selecting.
It means there's a non-zero statistical correlation between the gene and how often
the organism reproduces. Over a few million years, that non-zero statistical
correlation adds up to something very powerful. It's not a god, but it's more closely 
akin to a god than it is to snow on a television screen.

In a lot of ways, evolution *is* like unto theology. "Gods are ontologically distinct
from creatures," said Damien Broderick, "or they're not worth the paper they're written
on." And indeed, the Shaper of Life is not itself a creature. Evolution is bodiless, 
like the Judeo-Christian deity. Omnipresent in Nature, immanent in the fall of every
leaf. Vast as a planet's surface. Billions of years old. Itself unmade, arising 
naturally from the structure of physics. Doesn't that all sound like something that
might have been said about God?

And yet the Maker has no mind, as well as no body. In some ways, its handiwork is 
incredibly poor design by human standards. It is internally divided. Most of all, it
isn't *nice*.

In a way, Darwin *discovered* God—a God that failed to match the preconceptions of 
theology, and so passed unheralded. If Darwin had discovered that life was created 
by an intelligent agent—a bodiless mind that loves us, and will smite us with lightning 
if we dare say otherwise—people would have said "My gosh! That's God!"

But instead Darwin discovered a strange alien God—not comfortably "ineffable", but
*really genuinely different from us*. Evolution is not a God, but if it were, it 
wouldn't be Jehovah. It would be H. P. Lovecraft's Azathoth, the blind idiot God 
burbling chaotically at the center of everything, surrounded by the thin monotonous 
piping of flutes.
```

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

For more on intelligence in LOGI see [here](#Levels-of-Organization-in-General-Intelligence).

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
