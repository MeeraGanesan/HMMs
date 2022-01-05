# HMMs
Note: Code is kept private, can show on a need-to-know basis.

This project implements a named entity recognition system using Hidden Markov Models. It uses the forward backward algorithm.

Named entity recognition (NER) is the task of classifying named entities, typically proper nouns, into pre-defined categories, such as person, location, organization. This is an incredibly important task for a machine to begin to analyze and interpret a body of natural language text.

The first part of the project implements an algorithm to learn the hidden Markov model parameters needed to apply the forward backward algorithm. There are 3 sets of parameters that are estimated: the initialization probabilities, the transition probabilities, and the emission probabilities. Each of these probabilities are modeled using a multinomial distribution whose parameters are estimated using maximum likelihood.

The next part of the project implements the forward-backward algorithm. This finds the probability of a label given all the evidence variables. The algorithm then assigns a tag using the minimum Bayes risk predictor, which is the tag corresponding to the maximum probability.
