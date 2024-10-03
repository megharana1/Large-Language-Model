# Large-Language-Model-LLM
I trained a neural network on a dataset of 32,000 names, using bigrams to determine the probabilities of one character following another. Built in PyTorch, this model learns P(cᵢ₊₁ | cᵢ) for each character pair, forming a stochastic matrix that captures the morphological structure of the language. This foundational model could be further developed into a more advanced architecture, such as a Transformer-based language model like GPT.

Key steps involved:

Extracting bigrams and mapping their frequencies
Constructing a PyTorch matrix to represent transition probabilities
Training the neural network using cross-entropy loss and backpropagation
Sampling character sequences with torch.multinomial
It encompasses modeling, sampling, training of models and evaluating loss functions such as negative log likelihood for classification.

The neural network was implemented and optimized through gradient descent, successfully reducing the loss function via backpropagation.

Result: The final model generates linguistically plausible names, demonstrating that local character dependencies significantly shape global word structures. This approach is versatile and can be applied to any domain characterized by sequential patterns, including code prediction, melody generation, and DNA sequence modeling.
