UNDER RESEARCH AND ACADEMIA
    [Email](#email)
    [Productivity](#Productivity)
        [Structured procrastination](#Structured-procrastination)
	[Tactical procrastination](#Tactical-procrastination)
        [Batch low-intensity tasks](#Batch-low-intensity-tasks)
[Physics](#Physics)
	[Common misconceptions](#Common-misconceptions)
		[Misconceptions about relativity](#Misconceptions-about-relativity)
UNDER SOFTWARE
[Performance optimization](#Performance-optimization), pretty much all Carlos Bueno  	CHANGE FROM PREMATURE 
	
REMOVE
[Readability]

--------------------------------------
(UNDER Erisology and thinking less wrongly)
I'd be remiss not to mention that Carlos Bueno's [advice on optimizing software performance](#Performance-optimization) ("in 8-figure compute environments", as he says on Twitter) has a *ton* of good stuff on thinking less wrongly.

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


----------------------------------------	
<a name="#Physics"></a>
## Physics
([overview](#overview))	

<a name="#Common-misconceptions"></a>
### Common misconceptions
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
    
<a name="#Productivity"></a>
### Productivity
([overview](#overview))  

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


(UNDER BIO/EVOLUTION)
[Evolution as alien god](#evolution-as-alien-god), where I first learned that there are many evolutions, as many as reproducing populations

(UNDER BIO/EVOLUTION)
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

(UNDER PHILO)
<a name="#Ra"></a>
### Ra
([overview](#overview))	

Every time someone mentions Harvard, or McKinsey, or even Google, I think of Sarah Constantin's [Ra](https://srconstantin.wordpress.com/2016/10/20/ra/). 

A quick sketch:

```markdown
The Egyptian god Ra was a symbol of divine kingship, all-powerful and all-seeing.  
He’s a good metaphor for a certain kind of psychological phenomenon that involves 
thought distortions around authority and legitimacy.

The Establishment is primarily an upper-class phenomenon, that it is more about 
social and moral legitimacy than mere wealth or raw power, and that it is *boringly
evil* — it produces respectable, normal, right-thinking, mild-mannered people who 
do things with very bad consequences.

It’s like a dissipating, entropic motion, a process that corrupts institutions.

Ra is something like a psychological mindset, that causes people to actually 
*seek* corruption and confusion, and to *prefer corruption for its own sake* — 
though, of course, it doesn’t feel quite like that from the inside.

Ra is a specific kind of glitch in intuition, which can roughly be summarized as 
*the drive to idealize vagueness and despise clarity*.  

As forces in the human psyche go, Ra is a pretty mild one. It’s not a powerful 
biological drive like aggression, or a difficult-to-treat problem like depression,
or a highly optimized energy-saving structure like the standard cognitive biases.

Ra is hard to pin down, but vulnerable to open communication and introspection.  
If you can talk and think about what you want, or how you feel, or why you believe
what you do, and you don’t dodge the question, Ra will dissolve like mist. 

Ra is hard to see, but easy to overcome once you see it.
```

What is Ra *not*?

```markdown
The usual pitfall when using poetic language to define egregores is making them too broad.
There is not one root of all evil that causes all the ills of the world.

Ra is not simply conformity, simply authoritarianism, or simply power-seeking.  Ra is not
the same as “bureaucracy” or “capitalism” or “fallen human nature” or all the myriad reasons
why your idealistic goal might fail.  Ra is not “everything that is wrong with people who
disagree with me.”

As a social phenomenon, Ra is responsible for some dysfunctions in the democratic modern 
West; it is not, for instance, what was going on with the Nazis, or with terrorists, or 
with communist revolutionaries, or with the Confederates in the American Civil War.  Ra 
is not driving people who want to take over the world for some fanatic goal. 

But it’s not *merely* the most commonly claimed drivers of institutional decay, like 
“knowledge problems” or “coordination problems”.  People who participate in those problems
*are* following rational self-interest, but wind up contributing individually to collectively
harmful outcomes.
```

Sarah goes on to define Ra extensionally. To summarize:

- Ra is about generic superlativity
- Ra is about legitimacy
- Ra defends itself with vagueness, confusion, incoherence — and then ange
- Ra hates communication and introspection
- Ra is fake Horus
- Ra corresponds to a stage in the corruption of organizations
- Ra is easy to overcome

I'll quote from the parts I liked:







<a name="#Legibility"></a>
### Legibility
([overview](#overview))	
	
The community forum *The Scholar's Stage* has a great post, [Tradition is Smarter Than You Are](http://scholars-stage.blogspot.com/2018/08/tradition-is-smarter-than-you-are.html), that gives a couple examples of tradition-as-Chesterton's-fence. It begins like so:

```markdown
Brain-power alone is not enough to explain why humans are such a successful species. Humans, he 
(evolutionary anthropologist-cum-cross cultural psychologist Joseph Henrich) argues, are not nearly
as intelligent as we think they are. Remove them from the culture and environment they have learned 
to operate in and they fail quickly. His favorite example of this are European explorers who die in
the middle of deserts, jungles, or arctic wastes even though thousands of generations of hunter-
gatherers were able to survive and thrive in these same environments. If human success was due to our
ability to problem solve, analyze, and rationally develop novel solutions to novel challenges, the 
explorers should have been fine. Their ghastly fates suggest that rationality may not be the key to
human survival.
```
 
The key is cultural evolution. An example via the cassava plant, or manioc, from Heinrich's book [*The Secret of Our Success*](https://amzn.to/2LuDcEh):

```markdown
In the Americas, where manioc was first domesticated, societies who have relied on bitter varieties
for thousands of years show no evidence of chronic cyanide poisoning. In the Colombian Amazon, for
example, indigenous Tukanoans use a multistep, multiday processing technique that involves scraping,
grating, and finally washing the roots in order to separate the fiber, starch, and liquid. Once
separated, the liquid is boiled into a beverage, but the fiber and starch must then sit for two more
days, when they can then be baked and eaten. Figure 7.1 shows the percentage of cyanogenic content in
the liquid, fiber, and starch remaining through each major step in this processing. 

Such processing techniques are crucial for living in many parts of Amazonia, where other crops are 
difficult to cultivate and often unproductive. However, despite their utility, one person would have
a difficult time figuring out the detoxification technique. Consider the situation from the point of
view of the children and adolescents who are learning the techniques. They would have rarely, if ever,
seen anyone get cyanide poisoning, because the techniques work. And even if the processing was
ineffective, such that cases of goiter (swollen necks) or neurological problems were common, it would
still be hard to recognize the link between these chronic health issues and eating manioc. Most people
would have eaten manioc for years with no apparent effects. Low cyanogenic varieties are typically 
boiled, but boiling alone is insufficient to prevent the chronic conditions for bitter varieties. 
Boiling does, however, remove or reduce the bitter taste and prevent the acute symptoms (e.g., diarrhea,
stomach troubles, and vomiting). 

So, if one did the common-sense thing and just boiled the high-cyanogenic manioc, everything would seem
fine. Since the multistep task of processing manioc is long, arduous, and boring, sticking with it is
certainly non-intuitive. Tukanoan women spend about a quarter of their day detoxifying manioc, so this
is a costly technique in the short term. Now consider what might result if a self-reliant Tukanoan
mother decided to drop any seemingly unnecessary steps from the processing of her bitter manioc. She 
might critically examine the procedure handed down to her from earlier generations and conclude that 
the goal of the procedure is to remove the bitter taste. She might then experiment with alternative 
procedures by dropping some of the more labor-intensive or time-consuming steps. She’d find that with
a shorter and much less labor-intensive process, she could remove the bitter taste. Adopting this easier
protocol, she would have more time for other activities, like caring for her children. Of course, years
or decades later her family would begin to develop the symptoms of chronic cyanide poisoning. 

Thus, the unwillingness of this mother to take on faith the practices handed down to her from earlier 
generations would result in sickness and early death for members of her family. Individual learning does
not pay here, and intuitions are misleading. The problem is that the steps in this procedure are causally
opaque—an individual cannot readily infer their functions, interrelationships, or importance. The causal
opacity of many cultural adaptations had a big impact on our psychology. 

Wait. Maybe I’m wrong about manioc processing. Perhaps it’s actually rather easy to individually figure
out the detoxification steps for manioc? Fortunately, history has provided a test case. At the beginning
of the seventeenth century, the Portuguese transported manioc from South America to West Africa for the 
first time. They did not, however, transport the age-old indigenous processing protocols or the underlying
commitment to using those techniques. Because it is easy to plant and provides high yields in infertile 
or drought-prone areas, manioc spread rapidly across Africa and became a staple food for many populations.
The processing techniques, however, were not readily or consistently regenerated. Even after hundreds of
years, chronic cyanide poisoning remains a serious health problem in Africa. Detailed studies of local 
preparation techniques show that high levels of cyanide often remain and that many individuals carry low
levels of cyanide in their blood or urine, which haven’t yet manifested in symptoms. In some places,
there’s no processing at all, or sometimes the processing actually increases the cyanogenic content. On 
the positive side, some African groups have in fact culturally evolved effective processing techniques, 
but these techniques are spreading only slowly.

The point here is that cultural evolution is often much smarter than we are. Operating over generations 
as individuals unconsciously attend to and learn from more successful, prestigious, and healthier members
of their communities, this evolutionary process generates cultural adaptations. Though these complex 
repertoires appear well designed to meet local challenges, they are not primarily the products of 
individuals applying causal models, rational thinking, or cost-benefit analyses. Often, most or all of
the people skilled in deploying such adaptive practices do not understand how or why they work, or even 
that they “do” anything at all. Such complex adaptations can emerge precisely because natural selection
has favored individuals who often place their faith in cultural inheritance—in the accumulated wisdom 
implicit in the practices and beliefs derived from their forbearers—over their own intuitions and 
personal experiences.
```

Another example from northern Canada, where Naskapi foragers hunt caribou:

```markdown
When hunting caribou, Naskapi foragers in Labrador, Canada, had to decide where to go. Common sense might
lead one to go where one had success before or to where friends or neighbors recently spotted caribou. 
However, this situation is like Matching Pennies in chapter 2. The caribou are mismatchers and the 
hunters are matchers. That is, hunters want to match the locations of caribou while caribou want to 
mismatch the hunters, to avoid being shot and eaten. If a hunter shows any bias to return to previous 
spots, where he or others have seen caribou, then the caribou can benefit (survive better) by avoiding
those locations (where they have previously seen humans). 

Thus, the best hunting strategy requires randomizing. Can cultural evolution compensate for our 
cognitive inadequacies? Traditionally, Naskapi hunters decided where to go to hunt using divination and 
believed that the shoulder bones of caribou could point the way to success. To start the ritual, the shoulder
blade was heated over hot coals in a way that caused patterns of cracks and burnt spots to form. This 
patterning was then read as a kind of map, which was held in a pre-specified orientation. The cracking 
patterns were (probably) essentially random from the point of view of hunting locations, since the outcomes 
depended on myriad details about the bone, fire, ambient temperature, and heating process. Thus, these 
divination rituals may have provided a crude randomizing device that helped hunters avoid their own
decision-making biases. The undergraduates in the Matching Pennies game could have used a randomizing 
device like divination, though the chimps seem fine without it.
```

There's a similar practice in Indonesia employed by the Kantus of Kalimantan, who use bird augury to select locations for their agricultural plots:

```markdown
The anthropologist Michael Dove argues that two factors will cause farmers to make plot placements
that are too risky. First, Kantu ecological models contain the Gambler’s Fallacy and lead them to 
expect that floods will be less likely to occur in a specific location after a big flood in that 
location (which is not true). 

Second, as with the MBAs’ investment allocations in chapter 4, Kantus pay attention to others’ 
success and copy the choices of successful households, meaning that if one of their neighbors has
a good yield in an area one year, many other people will want to plant there in the next year. 
Reducing the risks posed by these cognitive and decision-making biases, the Kantu rely on a system
of bird augury that effectively randomizes their choices for locating garden plots, which helps them
avoid catastrophic crop failures. The results of divination depend not only on seeing a particular
bird species in a particular location, but also on what type of call the bird makes (one type of call 
may be favorable, and another unfavorable). 

The patterning of bird augury supports the view that this is a cultural adaptation. The system seems 
to have evolved and spread throughout this region since the seventeenth century when rice cultivation
was introduced. This makes sense, since it is rice cultivation that is most positively influenced by
randomizing garden locations. It’s possible that, with the introduction of rice, a few farmers began
to use bird sightings as an indication of favorable garden sites. On average, over a lifetime, these
farmers would do better—be more successful—than farmers who relied on the Gambler’s Fallacy or on 
copying others’ immediate behavior. 

Whatever the process, within 400 years, the bird augury system had spread throughout the agricultural
populations of this Borneo region. Yet it remains conspicuously missing or underdeveloped among local
foraging groups and recent adopters of rice agriculture, as well as among populations in northern 
Borneo who rely on irrigation. So, bird augury has been systematically spreading in those regions
where it is most adaptive. This example makes a key point: not only do people often not understand
what their cultural practices are doing, but sometimes it may even be important that they don’t
understand what their practices are doing or how they work. If people came to understand that bird 
augury or bone divination didn’t actually predict the future, the practice would probably be dropped
or people would increasingly ignore ritual findings in favor of their own intuitions.
```

There are two arguments Heinrich is making here:

```markdown
The first is that customs, traditions, and the like are subject to Darwinian selection. Henrich is not
always clear on exactly what is being selected for—is it individuals who follow a tradition, groups 
whose members all follow the tradition, or the tradition itself?—but the general gist is that traditions
stick around longest when they are adaptive. 

This process is "blind." Those who follow the traditions do not know how they work, and in some cases
(like religious rituals that build social solidarity) knowing the details of how they work might actually
reduce the efficacy of the tradition. That is the second argument of note: we do not (and often cannot)
understand just how the traditions we inherit help our survival, and because of that, it is difficult to
artificially create replacements. 
```

This, of course, jives perfectly with the work of James C. Scott. Here's *The Scholar's* summary intro:

```markdown
Scott has spent a large amount of his career studying the way states shape the societies they rule over, 
and the way societies try to resist the advance of the state. The central problem of ruler-ship, as Scott
sees it, is what he calls *legibility*. To extract resources from a population the state must be able to
understand that population. The state needs to make the people and things it rules legible to agents of
the government. Legibility means uniformity. States dream up uniform weights and measures, impress national
languages and ID numbers on their people, and divvy the country up into land plots and administrative 
districts, all to make the realm legible to the powers that be. 

The problem is that not all important things can be made legible. Much of what makes a society successful
is knowledge of the tacit sort: rarely articulated, messy, and from the outside looking in, purposeless. 
These are the first things lost in the quest for legibility. Traditions, small cultural differences, odd 
and distinctive lifeways—in other words, the products of cultural evolution that Henrich fills his book 
with—are all swept aside by a rationalizing state that preserves (or in many cases, imposes) only what it 
can be understood and manipulated from the 2,000 foot view. The result, as Scott chronicles with example
after example, are many of the greatest catastrophes of human history. 
```

That's a pretty good summary, but I prefer Scott Alexander's more verbose treatment in his [book review](https://slatestarcodex.com/2017/03/16/book-review-seeing-like-a-state/) of James' book, because microhumor and just *likable* storytelling. 

Scott (SA, not JCS) begins with a suspicious observation:

```markdown
Scott starts with the story of “scientific forestry” in 18th century Prussia. Enlightenment
rationalists noticed that peasants were just cutting down whatever trees happened to grow in the
forests, *like a chump*. They came up with a better idea: clear all the forests and replace them 
by planting identical copies of Norway spruce (the highest-lumber-yield-per-unit-time tree) in 
an evenly-spaced rectangular grid. Then you could just walk in with an axe one day and chop down 
like a zillion trees an hour and have more timber than you could possibly ever want.

This went poorly. The impoverished ecosystem couldn’t support the game animals and medicinal 
herbs that sustained the surrounding peasant villages, and they suffered an economic collapse. 
The endless rows of identical trees were a perfect breeding ground for plant diseases and forest
fires. And the complex ecological processes that sustained the soil stopped working, so after a
generation the Norway spruces grew stunted and malnourished. Yet for some reason, everyone
involved got promoted, and “scientific forestry” spread across Europe and the world.
```

"Evenly-spaced rectangular grids" will become a suspiciously repeating theme, "not just in biological systems but also in social ones":

```markdown
Natural organically-evolved cities tend to be densely-packed mixtures of dark alleys, tiny 
shops, and overcrowded streets. Modern scientific rationalists came up with a better idea: 
an evenly-spaced rectangular grid of identical giant Brutalist apartment buildings separated 
by wide boulevards, with everything separated into carefully-zoned districts. Yet for some 
reason, whenever these new rational cities were built, people hated them and did everything 
they could to move out into more organic suburbs. And again, for some reason the urban
planners got promoted, became famous, and spread their destructive techniques around the world.

Ye olde organically-evolved peasant villages tended to be complicated confusions of everybody
trying to raise fifty different crops at the same time on awkwardly shaped cramped parcels of 
land. Modern scientific rationalists came up with a better idea: giant collective mechanized 
farms growing purpose-bred high-yield crops and arranged in (say it with me) evenly-spaced
rectangular grids. Yet for some reason, these giant collective farms had lower yields per acre
than the old traditional methods, and wherever they arose famine and mass starvation followed.
And again, for some reason governments continued to push the more “modern” methods, whether it
was socialist collectives in the USSR, big agricultural corporations in the US, or sprawling 
banana plantations in the Third World.

Traditional lifestyles of many East African natives were nomadic, involving slash-and-burn 
agriculture in complicated jungle terrain according to a bewildering variety of ad-hoc rules. 
Modern scientific rationalists in African governments (both colonial and independent) came up
with a better idea – resettlement of the natives into villages, where they could have modern 
amenities like schools, wells, electricity, and evenly-spaced rectangular grids. Yet for some
reason, these villages kept failing: their crops died, their economies collapsed, and their 
native inhabitants disappeared back into the jungle. And again, for some reason the African 
governments kept trying to bring the natives back and make them stay, even if they had to blur
the lines between villages and concentration camps to make it work.
```

This raises the question: why did these schemes fail, and why were they still continued despite that? James' two-part answer is High Modernism in service of (this is the key insight) *legibilization of the world by centralized governing bodies to aid monitoring and control*, mostly for efficient taxation:

```markdown
The first part of the story is High Modernism, an aesthetic taste masquerading as a scientific
philosophy. The High Modernists claimed to be about figuring out the most efficient and high-
tech way of doing things, but most of them knew little relevant math or science and were 
basically just LARPing being rational by placing things in evenly-spaced rectangular grids.

But the High Modernists were pawns in service of a deeper motive: the centralized state wanted
the world to be “legible”, ie arranged in a way that made it easy to monitor and control. An 
intact forest might be more productive than an evenly-spaced rectangular grid of Norway spruce,
but it was harder to legislate rules for, or assess taxes on.

The state promoted the High Modernists’ platitudes about The Greater Good as cover, in order to
implement the totalitarian schemes they wanted to implement anyway. The resulting experiments 
were usually failures by the humanitarian goals of the Modernists, but resounding successes by 
the command-and-control goals of the state. And so we gradually transitioned from systems that
were messy but full of fine-tuned hidden order, to ones that were barely-functional but really
easy to tax.
```

The problem that legibilization solves is best illustrated by a parable:

```markdown
Suppose you’re a premodern king, maybe one of the Louises who ruled France in the Middle Ages.
You want to tax people to raise money for a Crusade or something. Practically everyone in your 
kingdom is a peasant, and all the peasants produce is grain, so you’ll tax them in grain.
Shouldn’t be too hard, right? You’ll just measure how many pints of grain everyone produces, and…

	The pint in eighteenth-century Paris was equivalent to 0.93 liters, whereas in Seine-en-
	Montane it was 1.99 liters and in Precy-sous-Thil, an astounding 3.33 liters. The aune, 
	a measure of length used for cloth, varied depending on the material(the unit for silk, 
	for instance, was smaller than that for linen) and across France there were at least 
	seventeen different aunes.
	
Okay, this is stupid. Just give everybody evenly-sized baskets, and tell them that baskets are
the new unit of measurement.

	Virtually everywhere in early modern Europe were endless micropolitics about how baskets 
	might be adjusted through wear, bulging, tricks of weaving, moisture, the thickness of the
	rim, and so on. In some areas the local standards for the bushel and other units of
	measurement were kept in metallic form and placed in the care of a trusted official or else
	literally carved into the stone of a church or the town hall. Nor did it end there. How the
	grain was to be poured (from shoulder height, which packed it somewhat, or from waist height?),
	how damp it could be, whether the container could be shaken down, and finally, if and how it
	was to be leveled off when full were subjects of long and bitter controversy.
	
Huh, this medieval king business is harder than you thought. Maybe you can just leave this problem to 
the feudal lords?

	Thus far, this account of local measurement practices risks giving the impression that, 
	although local conceptions of distance, area, volume, and so on were different from and
	more varied than the unitary abstract standards a state might favor, they were nevertheless
	aiming at objective accuracy. This impression would be false. […]

	A good part of the politics of measurement sprang from what a contemporary economist might 
	call the “stickiness” of feudal rents. Noble and clerical claimants often found it difficult
	to 	increase feudal dues directly; the levels set for various charges were the result of
	long struggle, and even a small increase above the customary level was viewed as a threatening
	breach of tradition. Adjusting the measure, however, represented a roundabout way of achieving
	the same end.

	The local lord might, for example, lend grain to peasants in smaller baskets and insist on 
	repayment in larger baskets. He might surreptitiously or even boldly enlarge the size of the
	grain sacks accepted for milling (a monopoly of the domain lord) and reduce the size of the
	sacks used for measuring out flour; he might also collect feudal dues in larger baskets and
	pay wages in kind in smaller baskets. While the formal custom governing feudal dues and wages 
	would thus remain intact (requiring, for example, the same number of sacks of wheat from the
	harvest of a given holding), the actual transaction might increasingly favor the lord. The
	results of such fiddling were far from trivial. Kula estimates that the size of the bushel
	(boisseau) used to collect the main feudal rent (taille) increased by one-third between 1674
	and 1716 as part of what was called the reaction feodale.
	
Okay, but nobody’s going to make too big a deal about this, right?

	This sense of victimization [over changing units of measure] was evident in the cahiers of 
	grievances prepared for the meeting of the Estates General just before the Revolution. […]
	In an unprecedented revolutionary context where an entirely new political system was being
	created from first principles, it was surely no great matter to legislate uniform weights 
	and measures. As the revolutionary decree read “The centuries old dream of the masses of
	only one just measure has come true! The Revolution has given the people the meter!”	
	
Maybe you should tax land. After all, it’s the land that grows the grain. Just figure out how much
land everybody owns, and you can calculate some kind of appropriate tax from there.

So, uh, peasant villagers, how much land does each of you own?

	A hypothetical case of customary land tenure practices may help demonstrate how difficult
	it is to assimilate such practices to the barebones scheme of a modern cadastral map 
	[land survey suitable for tax assessment][…]

	Let us imagine a community in which families have usufruct rights to parcels of cropland
	during the main growing season. Only certain crops, however, may be planted, and every 
	seven years the usufruct land is distributed among resident families according to each 
	family’s size and its number of able-bodied adults. After the harvest of the main-season
	crop, all cropland reverts to common land where any family may glean, graze their fowl and
	livestock, and even plant quickly maturing, dry-season crops. Rights to graze fowl and
	livestock on pasture-land held in common by the village is extended to all local families, 
	but the number of animals that can be grazed is restricted according to family size, 
	especially in dry years when forage is scarce. Families not using their grazing rights can
	give them to other villagers but not to outsiders. Everyone has the right to gather 
	firewood for normal family needs, and the village blacksmith and baker are given larger
	allotments. No commercial sale from village woodlands is permitted.

	Trees that have been planted and any fruit they may bear are the property of the family 
	who planted them, no matter where they are now growing. Fruit fallen from such tree, however,
	is the property of anyone who gathers it. When a family fells one of its trees or a tree is
	felled by a storm, the trunk belongs to the family, the branches to the immediate neighbors, 
	and the “tops” (leaves and twigs) to any poorer villager who carries them off. Land is set
	aside for use or leasing out by widows with children and dependents of conscripted males.
	Usufruct rights to land and trees may be let to anyone in the village; the only time they
	may be let to someone outside the village is if no one in the community wishes to claim 
	them. After a crop failure leading to a food shortage, many of these arrangements are
	readjusted.

You know what? I’m just going to put you all down as owning ten. Ten land. Everyone okay with that?
Cool. Let’s say ten land for everyone and just move on to the next village.

	Novoselok village had a varied economy of cultivation, grazing, and forestry…the complex
	welter of strips was designed to ensure that each village household received a strip of 
	land in every ecological zone. An individual household might have as many as ten to 
	fifteen different plots constituting something of a representative sample of the village’s
	ecological zones and microclimates. The distribution spread a family’s risks prudently, 
	and from time to time the land was reshuffled as families grew or shrunk…The strips of
	land were generally straight and parallel so that a readjustment could be made by moving
	small stakes along just one side of a field, without having to think of areal dimensions.
	Where the other side of the field was not parallel, the stakes could be shifted to 
	compensate for the fact that the strip lay toward the narrower or wider end of the field.
	Irregular fields were divided, not according to area, but according to yield.

…huh. Maybe this isn’t going to work. Let’s try it the other way around. Instead of mapping land,
we can just get a list with the name of everyone in the village, and go from there.

	Only wealthy aristocrats tended to have fixed surnames…Imagine the dilemma of a tithe or
	capitation-tax collector [in England] faced with a male population, 90% of whom bore just
	six Christian names (John, William, Thomas, Robert, Richard, and Henry).

Okay, fine. That won’t work either. Surely there’s something else we can do to assess a tax burden
on each estate. Think outside the box, scrape the bottom of the barrel!

	The door-and-window tax established in France [in the 18th century] is a striking case in 
	point. Its originator must have reasoned that the number of windows and doors in a dwelling
	was proportional to the dwelling’s size. Thus a tax assessor need not enter the house or 
	measure it, but merely count the doors and windows.

	As a simple, workable formula, it was a brilliant stroke, but it was not without consequences.
	Peasant dwellings were subsequently designed or renovated with the formula in mind so as to
	have as few openings as possible. While the fiscal losses could be recouped by raising the tax
	per opening, the long-term effects on the health of the population lasted for more than a century.	
```

Notice that this is totally in keeping with [reality having a surprising amount of detail](#Reality-has-a-surprising-amount-of-detail), but on top of that there's all this adversarial stuff going on -- feudal rent-seeking and its avoidance, fairness, politicization of measurement, etc.  

Another issue is that the relative illegibility of early cities to outsides granted locals a vital margin of political safety from outside control, as can be illustrated by the simple heuristic of asking if an outsider needed a local guide to navigate; centralized states didn't like this:

```markdown
Historically, the relative illegibility to outsiders of some urban neighborhoods has provided a 
vital margin of political safety from control by outside elites. A simple way of determining whether
this margin exists is to ask if an outsider would have needed a local guide in order to find her way 
successfully. If the answer is yes, then the community or terrain in question enjoys at least a small
measure of insulation from outside intrusion. Coupled with patterns of local solidarity, this 
insulation has proven politically valuable in such disparate contexts as eighteenth-and early 
nineteenth-century urban riots over bread prices in Europe, the Front de Liberation Nationale’s 
tenacious resistance to the French in the Casbah of Algiers, and the politics of the bazaar that 
helped to bring down the Shah of Iran. Illegibility, then, has been and remains a reliable resource
for political autonomy.
```

Anyway, *that's* what legibilization solves:

```markdown
The moral of the story is: premodern states had very limited ability to tax their citizens 
effectively. Along with the problems mentioned above – nonstandardized measurement, 
nonstandardized property rights, nonstandardized personal names – we can add a few others. 
At this point national languages were a cruel fiction; local “dialects” could be as different
from one another as eg Spanish is from Portuguese, so villagers might not even be able to
understand the tax collectors. Worst of all, there was no such thing as a census in France
until the 17th century, so there wasn’t even a good idea of how many people or villages there
were.

Kings usually solved this problem by leaving the tax collection up to local lords, who 
presumably knew the idiosyncracies of their own domains. But one step wasn’t always enough. 
If the King only knew Dukes, and the Dukes only knew Barons, and the Barons only knew village
headmen, and it was only the village headmen who actually knew anything about the peasants, 
then you needed a four-step chain to get any taxes. Each link in the chain had an incentive to
collect as much as they could and give up as little as they could get away with. So on the one
end, the peasants were paying backbreaking punitive taxes. And on the other, the Royal Treasurer
was handing the King half a loaf of moldy bread and saying “Here you go, Sire, apparently this 
is all the grain in France.”

So from the beginning, kings had an incentive to make the country “legible” – that is, so
organized and well-indexed that it was easy to know everything about everyone and collect/double-
check taxes. Also from the beginning, nobles had an incentive to frustrate the kings so that they
wouldn’t be out of a job. And commoners, who figured that anything which made it easier for the 
State to tax them and interfere in their affairs was bad news, usually resisted too.
```

Resistance against legibilization was intense, but centralized states gradually pushed outwards from their capitals iteratively, honing their techniques as they went. Here's what happened in the context of surnames:

```markdown
Peasants didn’t like permanent surnames. Their own system was quite reasonable for them: John the
baker was John Baker, John the blacksmith was John Smith, John who lived under the hill was John 
Underhill, John who was really short was John Short. The same person might be John Smith and John
Underhill in different contexts, where his status as a blacksmith or place of origin was more 
important.

But the government insisted on giving everyone a single permanent name, unique for the village, and 
tracking who was in the same family as whom. Resistance was intense:

	What evidence we have suggests that second names of any kind became rare as distance from the state’s
	fiscal reach increased. Whereas one-third of the households in Florence declared a second name, the
	proportion dropped to one-fifth for secondary towns and to one-tenth in the countryside. It was not
	until the seventeenth century that family names crystallized in the most remote and poorest areas of
	Tuscany – the areas that would have had the least contact with officialdom. […]

	State naming practices, like state mapping practices, were inevitably associated with taxes (labor,
	military service, grain, revenue) and hence aroused popular resistance. The great English peasant 
	rising of 1381 (often called the Wat Tyler Rebellion) is attributed to an unprecedented decade of
	registration and assessments of poll taxes. For English as well as for Tuscan peasants, a census of
	all adult males could not but appear ominous, if not ruinous.

The same issues repeated themselves a few hundred years later when Europe started colonizing other
continents. Again they encountered a population with naming systems they found unclear and unsuitable 
to taxation. But since colonial states had more control over their subjects than the relatively weak
feudal monarchies of the Middle Ages, they were able to deal with it in one fell swoop, sometimes
comically so:

Nowhere is this better illustrated than in the Philippines under the Spanish. Filipinos were instructed
by the decree of November 21, 1849 to take on permanent Hispanic surnames. […]

	Each local official was to be given a supply of surnames sufficient for his jurisdiction, “taking
	care that the distribution be made by letters of the alphabet.” In practice, each town was given
	a number of pages from the alphabetized [catalog], producing whole towns with surnames beginning
	with the same letter. In situations where there has been little in-migration in the past 150 years,
	the traces of this administrative exercise are still perfectly visible across the landscape. “For
	example, in the Bikol region, the entire alphabet is laid out like a garland over the provinces of
	Albay, Sorsogon, and Catanduanes which in 1849 belonged to the single jurisdiction of Albay. 
	Beginning with A at the provincial capital, the letters B and C mark the towns along the cost 
	beyond Tabaco to Wiki. We return and trace along the coast of Sorosgon the letters E to L, then 
	starting down the Iraya Valley at Daraga with M, we stop with S to Polangui and Libon, and finish
	the alphabet with a quick tour around the island of Catanduas.

	The confusion for which the decree is the antidote is largely that of the administrator and the tax
	collector. Universal last names, they believe, will facilitate the administration of justice, finance,
	and public order as well as make it simpler for prospective marriage partners to calculate their 
	degree of consanguinity. For a utilitarian state builder of [Governor] Claveria’s temper, however, the 
	ultimate goal was a complete and legible list of subjects and taxpayers.

This was actually a lot less cute and funny than the alphabetization makes it sound:

	What if the Filipinos chose to ignore their new last names? This possibility had already crossed 
	Claveria’s mind, and he took steps to make sure that the names would stick. Schoolteachers were
	ordered to forbid their students to address or even know one another by any name except the officially
	inscribed family name. Those teachers who did not apply the rule with enthusiasm were to be punished.
	More efficacious perhaps, given the minuscule school enrollment, was the proviso that forbade priests 
	and military and civil officials from accepting any document, application, petition, or deed that did 
	not use the official surnames. All documents using other names would be null and void.

Similar provisions ensured the replacement of local dialects with the approved national language. Students
were only allowed to learn the national language in school and were punished for speaking in vernacular. 
All formal documents had to be in the national language, which meant that peasants who had formally been 
able to manage their own legal affairs had to rely on national-language-speaking intermediaries. Scott
talks about the effect in France:

	One can hardly imagine a more effective formula for immediately devaluing local knowledge and 
	privileging all those who had mastered the official linguistic code. It was a gigantic shift in power.
	Those at the periphery who lacked competence in French were rendered mute and marginal. They were now 
	in need of a local guide to the new state culture, which appeared in the form of lawyers, notaries, 
	schoolteachers, clerks, and soldiers.
```

High Modernism, extensionally defined:

```markdown
- standardization, 
- Henry Ford, 
- the factory as metaphor for the best way to run everything, 
- conquest of nature, 
- New Soviet Man, 
- people with college degrees knowing better than you, 
- wiping away the foolish irrational traditions of the past, 
- Brave New World, 
- everyone living in dormitories and eating exactly 2000 calories of Standardized Food
  Product (TM) per day, 
- anything that is For Your Own Good, 
- gleaming modernist skyscrapers, 
- The X Of The Future, 
- complaints that the unenlightened masses are resisting The X Of The Future, 
- demands that if the unenlightened masses reject The X Of The Future they must be re-
  educated For Their Own Good, and (of course) 
- evenly-spaced rectangular grids.
```

James' description of why Brasilia was abandoned reminds me of Putrajaya, except for the latter they perhaps tried to do a hybrid of sorts to learn from the mistakes of the "Corbusierites":

```markdown
Most of those who have moved to Brasilia from other cities are amazed to discover “that it is a 
city without crowds.” People complain that Brasilia lacks the bustle of street life, that it has 
none of the busy street corners and long stretches of storefront facades that animate a sidewalk
for pedestrians. For them, it is almost as if the founders of Brasilia, rather than having planned
a city, have actually planned to prevent a city. The most common way they put it is to say that
Brasilia “lacks street corners,”by which they mean that it lacks the complex intersections of dense
neighborhoods comprising residences and public cafes and restaurants with places for leisure, work,
and shopping.

While Brasilia provides well for some human needs, the functional separation of work from residence
and of both from commerce and entertainment, the great voids between superquadra, and a road system
devoted exclusively to motorized traffic make the disappearance of the street corner a foregone
conclusion. The plan did eliminate traffic jams; it also eliminated the welcome and familiar 
pedestrian jams that one of Holston’s informants called "the point of social conviviality".

The term brasilite, meaning roughly Brasilia-itis,which was coined by the first-generation residents,
nicely captures the trauma they experienced. As a mock clinical condition, it connotes a rejection of
the standardization and anonymity of life in Brasilia. “They use the term brasilite to refer to their
feelings about a daily life without the pleasures-the distractions, conversations, flirtations, and
little rituals of outdoor life in other Brazilian cities.” Meeting someone normally requires seeing
them either at their apartment or at work. Even if we allow for the initial simplifying premise of 
Brasilia’s being an administrative city, there is nonetheless a bland anonymity built into the very 
structure of the capital. The population simply lacks the small accessible spaces that they could
colonize and stamp with the character of their activity, as they have done historically in Rio and
Sao Paulo. To be sure, the inhabitants of Brasilia haven’t had much time to modify the city through 
their practices, but the city is designed to be fairly recalcitrant to their efforts.

“Brasilite,” as a term, also underscores how the built environment affects those who dwell in it. 
Compared to life in Rio and Sao Paulo, with their color and variety, the daily round in bland,
repetitive, austere Brasilia must have resembled life in a sensory deprivation tank. The recipe for 
high-modernist urban planning, while it may have created formal order and functional segregation, did
so at the cost of a sensorily impoverished and monotonous environment-an environment that inevitably
took its toll on the spirits of its residents.

The anonymity induced by Brasilia is evident from the scale and exterior of the apartments that 
typically make up each residential superquadra. For superquadra residents, the two most frequent 
complaints are the sameness of the apartment blocks and the isolation of the residences (“In Brasilia,
there is only house and work”). The facade of each block is strictly geometric and egalitarian.
Nothing distinguishes the exterior of one apartment from another; there are not even balconies that 
would allow residents to add distinctive touches and create semipublic spaces.
```

It's useful to contrast High Modernist principles (as epitomized by the French architech Le Corbusier) with Jane Jacobs' critique of them. 

High Modernism:

```markdown
First, there can be no compromise with the existing infrastructure. It was designed by superstitious
people who didn’t have architecture degrees, or at the very least got their architecture degrees in
the past and so were insufficiently Modern. The more completely it is bulldozed to make way for the
Glorious Future, the better.

Second, human needs can be abstracted and calculated. A human needs X amount of food. A human needs 
X amount of water. A human needs X amount of light, and prefers to travel at X speed, and wants to 
live within X miles of the workplace. These needs are easily calculable by experiment, and a good 
city is the one built to satisfy these needs and ignore any competing frivolities.

Third, the solution is the solution. It is universal. The rational design for Moscow is the same as
the rational design for Paris is the same as the rational design for Chandigarh, India. As a 
corollary, all of these cities ought to look exactly the same. It is maybe permissible to adjust for
obstacles like mountains or lakes. But only if you are on too short a budget to follow the rationally
correct solution of leveling the mountain and draining the lake to make your city truly optimal.

Fourth, all of the relevant rules should be explicitly determined by technocrats, then followed to the
letter by their subordinates. Following these rules is better than trying to use your intuition, in 
the same way that using the laws of physics to calculate the heat from burning something is better than
just trying to guess, or following an evidence-based clinical algorithm is better than just prescribing
whatever you feel like.

Fifth, there is nothing whatsoever to be gained or learned from the people involved (eg the city’s 
future citizens). You are a rational modern scientist with an architecture degree who has already 
calculated out the precise value for all relevant urban parameters. They are yokels who probably cannot
even spell the word architecture, let alone usefully contribute to it. They probably make all of their
decisions based on superstition or tradition or something, and their input should be ignored For Their
Own Good.
```

Jane Jacobs' critique of them, as summarized twice over by James and Scott:

```markdown
First, existing structures are evolved organisms built by people trying to satisfy their social
goals. They contain far more wisdom about people’s needs and desires than anybody could formally
enumerate. Any attempt at urban planning should try to build on this encoded knowledge, not 
detract from it.

Second, man does not live by bread alone. People don’t want the right amount of Standardized Food
Product, they want social interaction, culture, art, coziness, and a host of other things nobody 
will ever be able to calculate. Existing structures have already been optimized for these things,
and unless you’re really sure you understand all of them, you should be reluctant to disturb them.

Third, solutions are local. Americans want different things than Africans or Indians. One proof of
this is that New York looks different from Lagos and from Delhi. Even if you are the world’s best 
American city planner, you should be very concerned that you have no idea what people in Africa 
need, and you should be very reluctant to design an African city without extensive consultation of
people who understand the local environment.

Fourth, even a very smart and well-intentioned person who is on board with points 1-3 will never be
able to produce a set of rules. Most of people’s knowledge is implicit, and most rule codes are 
quickly replaced by informal systems of things that work which are much more effective (the classic 
example of this is work-to-rule strikes).

Fifth, although well-educated technocrats may understand principles which give them some advantages
in their domain, they are hopeless without the on-the-ground experience of the people they are trying
to serve, whose years of living in their environment and dealing with it every day have given them a
deep practical knowledge which is difficult to codify.
```

To the Tukanoans' multistep manioc/cassava processing, the Naskapi foragers' randomized caribou-hunting and Kantus' bird augury for agricultural plot location selection at the beginning of this section James adds the example of Tanzanian farming:

```markdown
(In Tanzania), small farmers grew dozens of different crops together in seeming chaos. Western 
colonists tried to convince them – often by force – to switch to just growing one thing at a time 
to reap advantages of efficiency, standardization, and specialization of labor. Only growing one 
crop in the same field was Agricultural Science 101. But this turned out to be a bad idea in the 
difficult Tanzanian environment:

	The multistoried effect of polyculture has some distinct advantages for yields and soil 
	conservation. “Upper-story” crops shade “lowerstory” crops, which are selected for their
	ability to thrive in the cooler soil temperature and increased humidity at ground level.
	Rainfall reaches the ground not directly but as a fine spray that is absorbed with less
	damage to soil structure and less erosion. The taller crops often serve as a useful 
	windbreak for the lower crops. Finally, in mixed or relay cropping, a crop is in the field
	at all times, holding the soil together and reducing the leaching effects that sun, wind,
	and rain exert, particularly on fragile land. Even if polyculture is not to be preferred
	on the grounds of immediate yield, there is much to recommend it in terms of sustainability
	and thus long-term production.

	Our discussion of mixed cropping has thus far dealt only with the narrow issues of yield 
	and soil conservation. It has overlooked the cultivators themselves and the various other
	ends that they seek by using such techniques. The most significant advantage of 
	intercropping, Paul Richards claims, is its great flexibility, “the scope [it] offers for
	a range of combinations to match individual needs and preferences, local conditions, and 
	changing circumstances within each season and from season to season.” Farmers may polycrop 
	in order to avoid labor bottlenecks at planting and at harvest.44Growing many different 
	crops is also an obvious way to spread risks and improve food security. Cultivators can
	reduce the danger of going hungry if they sow, instead of only one or two cultivars, crops
	of long and short maturity, crops that are drought resistant and those that do well under
	wetter conditions, crops with different patterns of resistance to pests and diseases, crops
	that can be stored in the ground with little loss (such as cassava), and crops that mature 
	in the “hungry time” before other crops are gathered. Finally, and perhaps most important, 
	each of these crops is embedded in a distinctive set of social relations. Different members
	of the household are likely to have different rights and responsibilities with respect to
	each crop. The planting regimen, in other words, is a reflection of social relations, ritual
	needs, and culinary tastes; it is not just a production strategy that a profit-maximizing 
	entrepreneur took straight out of the pages of a text in neoclassical economics.
```

Okay. After all this talk negatively portraying legibility, is it *bad* somehow? James says that's not what he was getting at:

```markdown
...he’s not against legibility and modernism per se, but he wants to present them as ingredients
in a cocktail of state failure. You need a combination of four things to get a disaster like Soviet
collective farming (or his other favorite example, compulsory village settlement in Tanzania). 
First, a government incentivized to seek greater legibility for its population and territory. 
Second, a High Modernist ideology. Third, authoritarianism. And fourth, a “prostrate civil society”,
like in Russia after the Revolution, or in colonies after the Europeans took over.

I think his theory is that the back-and-forth between centralized government and civil society allows
scientific advances to be implemented smoothly instead of just plowing over everyone in a way that 
leads to disaster. I also think that maybe a big part of it is incremental versus sudden: western 
farming did well because it got to incrementally add advances and see how they worked, but when you
threw the entire edifice at Tanzania it crashed and burned.
```
