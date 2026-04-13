We are building a multilayer perceptron character-level language model.
So what exactly we want our model to do is two things first for the model to learn the representation of each character so that it is not just random nonsense, and on top of that we also want it to be able to generate the next character based on these representaions
this is built off the paper A Neural Probabilistic Language Model
the key idea here is  a sequence of letters that has never been seen before gets high probability if it is made of letters that are similar (in the sense of having a nearby representation) to letters forming an already seen word
How we are going to do it
additional things suggested by the paper mix the probs obtained by this model with trigram