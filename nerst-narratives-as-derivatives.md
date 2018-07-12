I liked this essay by John Nerst: [Partial Derivatives and Partial Narratives](https://everythingstudies.com/2016/06/02/partial-derivatives-and-partial-narratives/).
But it's a bit too long for me to "see all at once", so here's a quick working summary in "tweetstorm" format (following Venkat Rao). 

I still don't know how to use LaTeX in Markdown yet. The solution below is a temporary stopgap, to be replaced as soon as I find something better.

---

### Narratives as partial derivatives of a complicated function representing "ground truth"

1. A function is usually defined in terms of ordered pairs: one variable depends on another "like so", e.g. <a href="https://www.codecogs.com/eqnedit.php?latex=\inline&space;f(x)&space;=&space;3x" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\inline&space;f(x)&space;=&space;3x" title="f(x) = 3x" /></a> 
describes the ordered pairs (1,3), (2,6), (3,9), ... 
2. A function's derivative "summarizes" the variable dependence in a certain way. x affects y *this way*, e.g. <a href="https://www.codecogs.com/eqnedit.php?latex=\inline&space;f'(x)&space;=&space;3" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\inline&space;f'(x)&space;=&space;3" title="f'(x) = 3" /></a>.
3. Derivatives are a useful way of understanding the behavior of a function, because of the way they summarize the variable dependence. Instead of holding all the distinct ordered pairs (1,3), (2,6), (3,9), ... in your head, all you need to remember is that "when x increases by 1, y increases by 3". It's a convenient summary. 
3. Derivatives destroy information. <a href="https://www.codecogs.com/eqnedit.php?latex=\inline&space;f'(x)&space;=&space;3&space;\Rightarrow&space;f(x)&space;=&space;3x&space;&plus;&space;C" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\inline&space;f'(x)&space;=&space;3&space;\Rightarrow&space;f(x)&space;=&space;3x&space;&plus;&space;C" title="f'(x) = 3 \Rightarrow f(x) = 3x + C" /></a>,
where C might assume any value, even a function (of other variables). There is an infinite family of functions who share the same derivative. It's easy to lose sight of this. 
4. A function can have many different partial derivatives that look nothing alike, e.g. <a href="https://www.codecogs.com/eqnedit.php?latex=\inline&space;f(x,y,z)&space;=&space;2x&plus;100y-3z^2&space;\Rightarrow&space;f_x&space;=&space;2,&space;f_y&space;=&space;100,&space;f_z&space;=&space;-6z" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\inline&space;f(x,y,z)&space;=&space;2x&plus;100y-3z^2&space;\Rightarrow&space;f_x&space;=&space;2,&space;f_y&space;=&space;100,&space;f_z&space;=&space;-6z" title="f(x,y,z) = 2x+100y-3z^2 \Rightarrow f_x = 2, f_y = 100, f_z = -6z" /></a>.
1. Think of reality as a function---a complicated one, with many variables---and our narratives of reality as partial derivatives of that function. 

### A fleshed-out example
This one comes from Scott Alexander's [book review](http://slatestarcodex.com/2016/11/10/book-review-house-of-god/)
of Samuel Shem's novel *House of God*. 

Scott actually gives two examples of what he calls the "weird form of figure-ground iversion" where the signal gets reinterpreted as the noise and vice versa (what in Nerst's metaphor would be flipping from one partial derivative to another). Here's one on politics:

```markdown
Some people think of government as another name for the things we do together, like providing food 
to the hungry, or ensuring that old people have the health care they need. These people know that 
some politicians are corrupt, and sometimes the money actually goes to whoever’s best at demanding 
pork, and the regulations sometimes favor whichever giant corporation has the best lobbyists. But 
this is viewed as a weird disease of the body politic, something that can be abstracted away as 
noise in the system.

And then there are other people who think of government as a giant pork-distribution system, where 
obviously representatives and bureaucrats, incentivized in every way to support the forces that 
provide them with campaign funding and personal prestige, will take those incentives. Obviously 
they’ll use the government to crush their enemies. Sometimes this system also involves the hungry 
getting food and the elderly getting medical care, as an epiphenomenon of its pork-distribution 
role, but this isn’t particularly important and can be abstracted away as noise.

I think I can go back and forth between these two models when I need to, but it’s a weird switch 
of perspective, where the parts you view as noise in one model resolve into the essence of the other 
and vice versa.
```

And here's the one relevant to Shem's novel:

```markdown
Doctors use certain assumptions, like:

1. The patient wants to get better, but there are scientific limits that usually make this impossible
2. Medical treatment makes people healthier
3. Treatment is determined by medical need and expertise

But in House of God, the assumptions get inverted:

1. The patient wants to just die peacefully, but there are bureaucratic limits that usually make this 
impossible
2. Medical treatment makes people sicker
3. Treatment is determined by what will make doctors look good without having to do much work

Everybody knows that those first three assumptions aren’t always true. Yes, sometimes we prolong life 
in contravention of patients’ wishes. Sometimes people mistakenly receive unnecessary treatment that 
causes complications. And sometimes care suffers because of doctors’ scheduling issues. But it’s easy 
to abstract away to an ideal medicine based on benevolence and reason, and then view everything else 
as rare and unfortunate deviations from the norm.

House of God goes the whole way and does a full figure-ground inversion. The outliers become the norm; 
good care becomes the rare deviation. What’s horrifying is how convincing it is.
... 


```
