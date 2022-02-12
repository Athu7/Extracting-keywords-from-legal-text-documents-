# Extracting-keywords-from-legal-text-documents-
1st approach(Using LSTM)
1. Data cleaning/ Text preprocessing:

For data cleaning I used regular expressions library, nltk library. A dataframe is created with cleaned documents for the training purpose. 

2. Text embedding:

Fist the text is converted by using onehot encoding then an embedding layer in the network is used to obtain the embedding vectors which are further passed to the LSTM.

3. Model:

1st layer: Embedding layer
2nd layer: LSTM layer conbtaining 100 cells
output layer: Dense output layer with sigmoid activation
Loss function: BinaryCrossEntropy
Optimizer: Adam optimizer

4. Accuracy:
There is some error in my implementation so not getting the required accuracy.
But I tried differnet approaches such as used distilBERT for obtaining the embeddings.
Tried changing the number of cells in LSTM also tried using multiple LSTM layers but all resulted in the same.
Which is why I tried the second approach that is using the pre trained model for feature extraction.



2nd approach(Using pre trained models)

1. I used different pre trained models such as rake, multirake, KeyBert for this approach.
2. I have demonstrated the rake approach in my code.
