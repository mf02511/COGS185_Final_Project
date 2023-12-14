# Comparing Standard Recurrent Neural Network and Long Short-Term Memory Neural Network on Char-RNN

**Author:** Mizuho Fukuda

**Course:** COGS 185 - Advanced Machine Learning Methods, UCSD

## Abstract
This experiment intends to test the effectiveness of standard recurrent neural networks and long short-term memory networks through the Char-RNN model [2]. Using a complete set of Sherlock Holmes text dataset, two sets of Char-RNN models were trained using either a standard recurrent neural network or a long short-term memory model and the results were compared. The results were compared on the average loss of 3 trials over 20,000 iterations of training for each model. In addition, the performance of models were assessed based on the quality of generated text. The training loss for the two models indicated that the long short-term memory network significantly improves the model’s learning efficiency and the text generated by the long short-term memory network also indicated a more effective model.

1. Introduction
   Char-RNN is a very  simple yet practical character level language model presented by Karpathy in his blog “The Unreasonable Effectiveness of Recurrent Neural Networks” [2], which generates text by processing and learning from the input text on a character sequence level. Char-RNN is implemented using a recurrent neural network, a powerful artificial neural network that processes inputs and generates outputs in a sequential manner. One significant advantage of recurrent neural networks is its ability to “model data with temporal or sequential structure and varying length inputs and outputs” as opposed to standard neural networks that assumes each data point as an independent, randomly generated element [3]. While a standard neural network assumes a fixed length of input and output, recurrent neural networks deal with sequences of elements of varying lengths, each element dependent on the previous element in the sequence. Figure 1 below illustrates the structure of a recurrent neural network. The right side of the figure illustrates the unrolled network. At each step, the hidden state is computed using the input at that step as well as the previous hidden state.

   ![simple RNN](assets/simple_rnn.png)

   Figure 1: A standard recurrent neural network [5].

   On the forward pass, the hidden state at each step is calculated using the following equation: $$h^{(t)} = \sigma(W^{hx}x^{(t)} + W^{hh}h^{(t-1)} + b_{h)}$$



3.  
