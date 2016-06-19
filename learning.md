# What learning algorithms can predict that our physics theories might not

A [hot topic](http://fqxi.org/community/essay/winners/2013.1) in physics right now is applying techniques from information theory and theoretical machine learning to better understand physics. There are even hopes that these techniques might develop into a so-called "theory of everything" that unifies and explains all aspects of the universe. But for all the attention this subject has gotten, I'm a bit disappointed that I've never seen an introduction that explains

1. where *exactly* might you be able to use learning algorithms where you can't just use [existing](https://en.wikipedia.org/wiki/Standard_Model) [physics](https://en.wikipedia.org/wiki/General_relativity) theories instead, and
2. a hands on guide to applying learning algorithms in these situations, for people who don't know information theory jargon

So I'm going to write one!

People often describe information physics or digital physics by saying it is something about the [entropy of black holes](http://www.pbs.org/wgbh/nova/blogs/physics/2014/04/is-information-fundamental/), or worse (in my opinion), the idea that [we might be living in a computer simulation](http://www.amnh.org/2016-asimov-debate). While there's a lot of research along those lines, I think it's more important to understand why those ideas are worth studying in the first place. So instead, I'm going to start with the following idea:

> *If* it is possible to put ourselves inside computer simulations, it *might* be possible to put ourselves in a situation where we cannot use existing physics theories to predict what we'll perceive happening to us, but where we can use machine learning algorithms to do so.

But before we get into it, I need to make a couple disclaimers. First, I'm not one of the people doing research in this area, and it's possible that my understanding of what these researchers are doing is completely and utterly wrong. I'm writing this anyway because I think this area is fascinating, and I want other people to be able to appreciate why it is so fascinating. So if you have any questions, comments, or corrections, please email me at [email].

Second, I want to make it very clear that information physics is currently just a *hypothesis* about how the universe works. Unlike more established theories such as the [standard model](http://www.quantumdiaries.org/2010/12/08/known-knowns-of-the-standard-model/) and [general relativity](http://www.feynmanlectures.caltech.edu/II_42.html), we do not know if this is *actually representative* of how the universe works, or even if a new physics theory is needed to explain the situation hinted at above (where I emphasized "if" and "might"). Answering those questions would require serious experimental evidence that is way beyond our capabilities today. But given how quickly our technology is improving, I wouldn't be completely shocked if it is possible in my lifetime.

So first question: how might we be able to put ourselves in a computer simulation?

## Putting ourselves in a computer simulation

If you haven't been living under a rock, you've probably noticed that computers and software have gotten *way* better over the last several decades, and this trend shows no signs of stopping. So [one study](http://hplusmagazine.com/2010/02/05/how-long-till-human-level-ai/) asked a bunch of AI experts when they think computers will become as smart as humans, and more than half predicted that this will happen before 2050.

![](learning/agi.gif)

If the optimists are right, we might see super-smart computers in my lifetime! But even if the pessimists are right, it's fun to speculate about what really powerful computers would be capable of anyway.

Virtual reality simulations are already pretty good these days. If computers in 2050 might be smarter than humans, then virtual reality simulations in 2050 might be so good that to a simulated person living in one, it would look pretty convincingly like a real universe.

Instead of speculating about it, could we see for ourselves if that is the case? Perhaps it could be done like this. People have used [brain-to-brain interfaces](https://www.washington.edu/news/2015/09/23/uw-team-links-two-human-brains-for-question-and-answer-experiment/) to think to each other over the internet, and the technology to do things like this is improving quickly. It wouldn't be too much of a stretch to imagine that several decades from now, these brain-to-brain connections might have so much bandwidth that people hooked up this way would feel like a single person. After all, our brains are really just [2 half-brains](https://www.youtube.com/watch?v=wfYbgdo8e-8) that communicate with each other, but we still each feel like a single person. So how would it feel if we hooked up two people's brains together in year 2050?

![](learning/im_him_sml.png)

Better yet, what if we hooked up your brain to a simulated brain in a virtual reality world? Would you feel like you are also the person in the simulation?

![](learning/im_him2_sml.png)

We won't know until we actually try it. If the answer is no then the rest of this blog post is completely irrelevant, but if the answer is yes then that would be really cool!

So let's say you do that and you're now a single person that lives in both the real world and a virtual reality world. Then the real world part of you gets into a tragic accident and your brain is blasted into a million pieces. How sad.

![](learning/im_virtual_sml.png)

But are you really dead? Because, you know, people have done surgeries where they [removed half of someone's brain](https://en.wikipedia.org/wiki/Hemispherectomy) and they still lived on OK. So if half of your brain is in the real world and half of your brain is in a computer simulation and you lose the part of your brain in the real world, shouldn't you still live on in the simulation?

If you try it out and the answer is no, then the rest of this blog post is completely irrelevant. But if the answer is yes, then it means that it's possible to put ourselves completely inside a computer simulation! Isn't that like the coolest thing ever? (If you like this sort of thing, here's a Wait But Why post describing [more situations like these](https://waitbutwhy.com/2014/12/what-makes-you-you.html).)

So what does this have to do with information physics? Oh right:

> *If it is possible to put ourselves inside computer simulations*, it might be possible to put ourselves in a situation where we cannot use existing physics theories to predict what we'll perceive happening to us, but where we can use machine learning algorithms to do so.

So now I've explained the first part. But even if you can live completely inside a simulation (and this is already a huge if), the computers running the simulation must still follow the laws of physics. So if you know how the simulation is programmed to behave, you don't need machine learning algorithms to predict what will happen to you. And if you could somehow know [general relativity](https://en.wikipedia.org/wiki/General_relativity), the [standard model](https://en.wikipedia.org/wiki/Standard_Model), and the state of every particle in the universe at the time your real world brain is blasted into a million pieces, then even if someone later decides to change the computer code of the simulation, then in theory you could predict that too. So what do you need learning algorithms for?

## What our physics theories can't predict

One really cool property of computer simulations is that you can make exact copies of them on different computers. If the simulation uses what's called a "deterministic algorithm," then it means that all copies of the simulation will output the same thing.

Now let's suppose that after disconnecting your real world brain, the simulation you're living in becomes deterministic, and that 30 seconds from now, it's programmed to display a message to you saying "You're still alive!" But those of us controlling the simulation are evil pranksters, and we decide to play a trick on you. Once the simulation becomes deterministic, we copy it onto a second computer, and right before it displays the "You're still alive!" message, we blast the original computer into a million pieces. Now here's the question: do you get to see the message?

[drawing]

Well, it depends on how we define "you," doesn't it? If we define "you" based on which physical body you're in, or which physical computer you're in, then you "die" in the original computer and don't get to see the message. (Arguably, by that definition, you die even earlier, when your physical human brain is blasted into a million pieces.) But if we instead define "you" in a different way where it doesn't matter which physical body or computer you're in, then maybe you do get to see the message.

But here's the thing. The way science works is that you're supposed to do experiments to figure out what's right and what's wrong. And what we just described here is a way for you to *experimentally determine* which of these definitions of "you" is wrong! How? By using the procedure above to attempt to put yourself in a computer simulation, then having some friends do that trick so that only a copy of the simulated "you" gets to see the "You're still alive!" message. If you die before you see the message, then the definitions of "you" predicting that you see the message are wrong. If you *do* get to see the message, then you know for a fact that the definitions of "you" predicting that you do *not* see the message are most definitely wrong! (One weird thing about this experiment is that people watching the computers from outside don't find out which definitions of "you" are wrong, but they can still reproduce the outcome for themselves by putting themselves inside a simulation.)

I'm going to use the terminology of the [Wait But Why post](https://waitbutwhy.com/2014/12/what-makes-you-you.html) I linked to earlier, and I'm going to call the hypothesis that you *do not* see the message the "brain theory." And I'm going to call the hypothesis that you *do* see the message the "data theory."

As of today, we don't know which hypothesis is right. But think about what it would mean if the data theory is right.

Well, that would mean we get to do an even crazier experiment! Suppose we do the same experiment as above, except for the following:

1. The evil pranksters copy the simulation onto 2 other computers, instead of just 1.
2. The simulation is deterministic, except for one thing: if someone presses a key on the keyboard, you get to see what they pressed from inside the simulation.
3. After the first computer is destroyed and the "You're still alive!" message appears, someone presses the `0` key on the second computer, and simultaneously presses the `1` key on the third computer.

Will you see a `0` or a `1`?

[drawing]

Easy, right? Isn't there just a 50% chance that you'll see a 0 and a 50% chance that you'll see a 1? Not so fast. Just because there's 2 possibilities doesn't necessarily mean that each one has a 50% chance of occurring. For example, if you consider the possibilities of whether or not you'll be struck by lightning within the next 10 seconds, it is far more likely that you will not be struck by lightning.

Well, then, how about we do this the proper way, and use the fundamental laws of physics to derive what's going to happen? Well, the most fundamental physics theories we know of today are the [standard model of particle physics](http://www.quantumdiaries.org/2010/12/08/known-knowns-of-the-standard-model/) and [general relativity](http://www.feynmanlectures.caltech.edu/II_42.html). And if you do the painstaking calculations, they'll tell you that the outcome of this experiment looks something like this:

[dead person]
[dead person in computer]
[person that sees 0]
[person that sees 1]

Here's the thing. While these theories can give you a probability distribution over what every atom in those computers is going to do, neither of them has a concept of who "you" are. So if you happen to know that "you" are a person being simulated in 2 computers (but you don't know which computer you're in because both copies of you have identical memories), and one version of "you" is going to see a 0 and the other version of "you" is going to see a 1, these theories cannot tell you the probabilities that the "real you" will see a 0 or a 1!

Of course, if the brain theory is right and you die before you would see either the 0 or the 1, then this doesn't matter. But if the data theory is right and you *do* get to see either the 0 or the 1, then that would mean *it's possible to do an experiment in which the most fundamental physics theories we know of today cannot predict the probabilities of you seeing a 0 or a 1*! (Take a moment to appreciate how crazy that would be.) In that case, we'd need a new physics theory to fill the gap.

## Enter the learning algorithms

Remember that at the beginning of this post, I promised to tell you about how people are "applying techniques from information theory and theoretical machine learning to better understand physics?" Well, now I get to tell you about that. But before we get into how you might figure out the probability of seeing a 0 or a 1 in the situation above, let's start with a slightly different question.

Suppose we do the experiment above, and you end up seeing either a 0 or a 1. (I'm going to assume from now on that the data theory is right, though this is still an open question.) But since those of us controlling the simulation are evil pranksters, we play the same trick again on both copies of "you" so that there are now 4 versions of "you:" a version that sees `00`, a version that sees `01`, a version that sees `10`, and a version that sees `11`.

[picture]

Then we play the same trick again, so that there's a version of "you" that sees every 3-digit sequence of 0's and 1's. Then we play the same trick again, and again, and so on, until we run out of money to buy more computers. (I'd imagine computers will be pretty cheap in year 2050.)

Now you can start to see a pattern. Inside the simulation, you see a sequence of 0's and 1's that keeps getting longer and longer. So considering the sequence that you've seen so far, how can you guess whether the next digit will be a 0 or a 1? Great question, and this sounds like a great time to talk about learning algorithms!

## The most badass learning algorithm ever invented

Machine learning is a really big field, and there are way too many learning algorithms to cover them all here. Most of these algorithms exist either to address practical, real-life problems such as performance or perceived theoretical problems such as runtime complexity. But if you are a godlike being who is not concerned with either of these worldly problems (and let's face it, we all wish we were), there is really only one learning algorithm you need to know, and it is called Solomonoff induction. Mathematicians have more or less proven that it is the best general purpose learning algorithm theoretically possible that we can approximately compute using known physics, and I think it is the most badass learning algorithm ever invented. [delete last sentence?]

Here's the problem that Solomonoff induction is designed to solve: suppose there is some unknown process generating a sequence of 0's and 1's (also known as a "bitstring") and you want to guess the next digit (or "bit") in the sequence. (Sounds familiar?)

So how might you do that? Intuitively you'd think that the next bit will probably continue the same pattern as the previous bits, rather than being something "random." But how can you tell how "random" a bitstring is? A subjective but really effective way of doing that is by figuring out what are the lengths of the shortest computer programs that output that bitstring. [link?] So let's use this idea to assign a probability to every bitstring.

First we need a way to randomly generate computer programs that produces shorter programs more often than longer programs. Easy! Flip a coin. If it lands heads, you're done. But if it lands tails, flip it again, and this time, if it lands heads then write a 0, and if it lands tails then write a 1. Keep repeating this process until you get to the part where "if it lands heads, you're done." The resulting bitstring is our *computer program*. (We normally read computer code as text, but it is stored on computers as a bitstring.)

Now we need this computer program to output a bitstring. Simple! Save the computer program as a binary file and run it using a deterministic interpreter for your favorite programming language, perhaps Python or JavaScript. (It doesn't matter which language, as long as it's Turing complete and has something like print or console.log that prints to the console. Also you should let the program use unlimited time and memory.) Of course, almost all randomly generated computer programs will have a syntax error, but that's OK because there is still a chance that the program will run and print something. As for the text that the program prints to console (which can also be represented as a bitstring), how about we call it the *console output*.

Finally we can assign a probability to every bitstring. If you generate and run random computer programs, over and over again for the rest of your life and a long time beyond, we can define the *algorithmic probability* of a bitstring to be the number of *console outputs* so far (counting duplicates) that *begin* with the bitstring in question, divided by *total* number of console outputs so far (both of which approach infinity). You can use this formula to calculate the probability that you will see any sequence of 0's and 1's when you put yourself in a 2050-era virtual reality simulation!

[are there any issues caused by finite console outputs?]

Now that's cool, but what we really want to do is predict the value of the bit you'll see *next*. To do that, first write down the bits you've seen so far, followed by an extra 0 at the end. I'll call that bitstring 0. Also write down the bits you've seen so far, followed by an extra 1 at the end, which I'll call bitstring 1. Then according to *Solomonoff induction*, the probability of seeing a 0 next is just the algorithmic probability of bitstring 0, divided by the sum of the algorithmic probability of bitstring 0 and the algorithmic probability of bitstring 1. The probability of seeing a 1 next is just one minus the probability of seeing a 0 next.

Phew, that was a mouthful! If you like, here's a flowchart:

```
the
extremely patient [1] person's
guide to
THE MOST BADASS LEARNING ALGORITHM
EVER INVENTED

  Start
    |
    v
*Flip* 2 coins <---  <-------------------------
    |              |                           |
    v              |                           |
If first coin is:  |                           |
[heads] -> write 0 |                           |
[tails] -> write 1 |                           |
    |           ---                            |
    |    Second coin is [heads]                |
    | Second coin is [tails]                   |
    v                                          |
Save bits as a *binary file*                   |
100101 -> random_program.bin                   |
    |                                          |
    v                                          |
*Execute* it as a computer program [2]         |
python random_program.bin > console_output.bin |
    |                                          |
    v                                          |
When it starts executing,                      |
get a new sheet of paper and...                |
    |                        ------------------
    |                   Do until the end of time
    | When time ends
    v
Given a bitstring *B*:
                                 # of console outputs (counting duplicates) that begin with *B*
algorithmic probability of *B* = --------------------------------------------------------------
                                 total # of console outputs (counting duplicates)
    |
    v
Given a bitstring *C*:
                                  algorithmic probability of *C* followed by 0
probability that next bit is 0 = -----------------------------------------------
                                 (algorithmic probability of *C* followed by 0 +
                                  algorithmic probability of *C* followed by 1)

probability that next bit is 1 = 1 - probability that next bit is 0
```

[1] "Extremely patient" is like the biggest understatement ever.
[2] Use the same deterministic Turing complete interpreter for every program, and let it use unlimited time and memory. In this example, I assume Python is running in a completely deterministic virtual machine.

Isn't that completely ridiculous? But that, folks, has been mathematically proven to be the best general purpose learning algorithm theoretically possible, assuming you have unlimited computing power and patience.

If you want to learn more about Solomonoff induction and why it is so badass, see [here](http://lesswrong.com/lw/dhg/an_intuitive_explanation_of_solomonoff_induction/), [here](http://scholarpedia.org/article/Algorithmic_probability), and [here](http://twistedoakstudios.com/blog/Post5623_solomonoffs-mad-scientist).

## Can we do better? [probably want to rewrite this]

Even though the procedure I just described uses the most badass learning algorithm ever invented, it still has an important limitation. If you follow it precisely, you will only make predictions using knowledge of past 0's and 1's you saw, ignoring knowledge of other stuff. Suppose that for some really weird reason, whenever you wave your arms and shout "I will see a 0," it increases your chances of seeing a 0 next. (You never know when the bits are chosen by an unknown process.) That would be a good thing to know, but the procedure above would not learn to take that into account. Could we modify it to take into account information like that?

Yes we can! Instead of directly writing down the bitstring displayed in the simulation and using Solomonoff induction to predict the next bit, you can record a video of everything you see and hear (and smell and touch and taste) and use Solomonoff induction to predict how the video will continue, which will include the 0's and 1's displayed in the future. This is possible because videos are ultimately stored on your computer as 1's and 0's. In fact, there's an added bonus of doing it this way (if you can ignore the even worse performance issues). When the bitstring only contains the 0's and 1's displayed, Solomonoff induction would not predict other things you will perceive in the simulation and you would need a separate way of doing that, such as knowing how the simulation is programmed. But if you use Solomonoff induction to predict *everything* you will sense in the future, you would no longer need to rely on someone telling you how the simulation behaves before you put yourself in the simulation.

Heck, in theory you could do that to predict what will happen to you right now in the real world, even if you do not put yourself in a simulation. Which raises the question of whether learning algorithms should be considered physics theories in their own right. (More on that in future blog posts, if I get the time to write them.)

[email, CC0]
