<a id="update-quantum"></a>**UPDATE 8/6/2016**: I belatedly rewrote the section below due to reader feedback. Thanks guys! (Here's the [original version](https://github.com/ad510/firstest-principle/blob/daa34b2e94f8d508b8a4141b58217c8f5445d798/_posts/2016-07-10-learning.md#what-our-physics-theories-cant-predict).)

Well, then, how about we do this the proper way, and use the fundamental laws of physics to derive what's going to happen? Well, the most fundamental physics theories we know of today are [general relativity](http://www.feynmanlectures.caltech.edu/II_42.html) and the [standard model of particle physics](http://www.quantumdiaries.org/2010/12/08/known-knowns-of-the-standard-model/). General relativity won't be of much use here because it doesn't have a concept of who "you" are. But the standard model has a concept called a [quantum state](http://scottaaronson.com/democritus/lec9.html) that can be used as a representation of "you."

The way measurement works in quantum mechanics is that when you measure something, the quantum state of "you" becomes *entangled*, or correlated with, the quantum state of the thing you measured. For example, if the quantum state of "your thoughts about a kitten" is entangled with the quantum state of an actual kitten standing in front of you, the plain English translation is that what you *think* the kitten is doing probably has something to do with what the kitten is *actually* doing.

{obvious approach would involve defining quantum states of "you", effects of evil prankster pressing 0, effects of evil prankster pressing 1, calculating how they entangle with each other}
So if you want to use the standard model to predict what you'll see in the simulation, you'd need to calculate how "you" will become entangled with the 2 versions of the simulation. And to do this, you'd have to partition the quantum state of the universe into the subsystem that is "you" and the subsystem that is "not you." But even if you are a godlike being who knows the quantum state of the universe, partitioning the quantum state of "you" from the rest of the universe is *extremely* hard. What's more, the standard model will *not* give you any guidance on how to do it!

Defining the quantum state of "you" is a famous unsolved problem in physics called the [measurement problem](https://en.wikipedia.org/wiki/Measurement_problem). And solving it isn't as simple as defining "you" as the quantum state of every particle in your brain, or as the quantum state being simulated in a quantum mechanics simulation. (If you want to understand why, go to Scott Aaronson's [lecture on free will](http://scottaaronson.com/democritus/lec18.html) and search "Mars Express." In that section, he lists several unsolved questions about its feasibility and says, "These are not metaphysical questions. They are, in principle, empirically answerable ones." You can think of this blog post as proposing one way to empirically answer some of these questions.)

So if predicting what you will measure is an unsolved problem in physics, why have we gotten away with it for so long? Thanks to something called [decoherence](https://en.wikipedia.org/wiki/Quantum_decoherence), in every experiment we've done in practice, the quantum state of the universe quickly reached a state where everyone agreed on what the outcome of the experiment was. In other words, even if everyone measured different things, at least what each person measured was *consistent* with what every other person measured. {to account for decoherence into unknown environment in these situations, you can use techniques in quora link}

But once we create sufficiently good brain-computer interfaces, we may create situations where different people will *not* agree on the outcome. For example, in the "0 or 1" experiment, you would either die, see a 0, or see a 1, but everyone watching the computers from outside will see all 3 outcomes simultaneously, like in the drawing below. {math of those techniques is way too complicated for me to understand, but they seem to be workarounds to not knowing quantum state of "you" rather than solving the underlying problem, and I'd be really surprised if they can model "you" accurately enough to model the case where you can only see 1 of these outcomes instead of all 3 simultaneously. If I'm right about that,} In that case, decoherence would no longer be a valid excuse for not knowing what the quantum state of "you" is.

<img src="/learning/outcome_25.png" width="652"/>

{to the best of my understanding,} What this means is that in order to correctly predict the probabilities of you seeing a 0 or a 1, you have to take a wild guess at how to partition the quantum state of the universe into the subsystem that is "you" and the subsystem that is "not you," and it has to be accurate enough to correctly predict:

1. How "you" move over a brain-computer interface from a brain into a simulation
2. What happens to "you" when the classical bits of the simulation are copied into 2 other computers {copy classical bits != copy quantum state of computers. Cannot copy quantum state of subatomic particles in computer. Even if simulating quantum mechanics (which may not necessarily be the case), no cloning theorem predicts that simulated quantum state cannot be the quantum state of you, only a quantum state that may or may not be entangled with you}
3. How strongly "you" entangle with the simulation when it displays either a 0 or a 1

If your wild guess isn't *that* accurate, then even if you have unlimited computational resources, the standard model will likely make a *very* wrong prediction. {if I'm misunderstanding something and you know of a way to predict this with standard model, please email me. Since my current understanding is} In other words, *it's possible to do an experiment in which the most fundamental physics theories we know of today cannot predict the probabilities of you seeing a 0 or a 1!* {I think it is very likely current understanding is wrong}

{digital physics is TOE that's much less sensitive to who you are}
In that case, we'd need a new physics theory to fill the gap.

```
current best guess of defining events: after converting pure state of you now to mixed state of you when displaying 0/1, what is probability that entropy of entanglement between computer & pure state of "real you" is greater than cutoff
some subjectivity on how to approximate as mixed state so probably more rigorous procedure to do this

intuitive understanding of von neumann entropy
- discrete shannon entropy = sum(p[i] * log2(1 / p[i]) for i = 1 to n)
  - min # yes or no questions you'd expect to ask to learn outcome (https://www.youtube.com/watch?v=2s3aJfRr9gE)

one specific situation where you'd use partial trace/cptp map (to understand assumptions they make)
- https://en.wikipedia.org/wiki/Quantum_decoherence#Density_matrix_approach

- https://en.wikipedia.org/wiki/Quantum_decoherence
  - "Decoherence shows how a macroscopic system interacting with a lot of microscopic systems (e.g. collisions with air molecules or photons) moves from being in a pure quantum state—which in general will be a coherent superposition (see Schrödinger's cat)—to being in an incoherent mixture of these states. The weighting of each outcome in the mixture in case of measurement is exactly that which gives the probabilities of the different results of such a measurement."
  - "Moreover, our observation tells us that this mixture looks like a proper quantum ensemble in a measurement situation, as we observe that measurements lead to the "realization" of precisely one state in the "ensemble"."
- quantum ensemble = mixed state (https://en.wikipedia.org/wiki/Density_matrix), so this basically says decoherence describes how pure state turns into mixed state, where mixed state probabilities are probabilities of alternative events happening
  - so maybe what I want is probability of all events in mixed state of "you" whose entropy with version of sim is greater than cutoff value

https://www.quora.com/How-is-quantum-entanglement-related-to-decoherence
http://www.academia.edu/7100280/Partial_traces_in_decoherence_and_in_interpretation_What_do_reduced_states_refer_to

delete footnote 2?
check update date
```
