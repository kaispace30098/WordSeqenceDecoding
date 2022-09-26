# WordSeqenceDecoding
This notebook trains a seq2seq decoder model with teacher forcing. The model contains a Embedding layer with pretrained weights by GloVe and a GRU layer with hidden-state for next-word generation. After training the model we create a sampling model with previous layers with trained weights from the decoder and (let machine choose from word distribution from the softmax outcome) to generate a sentence.
The dataset is a bunch of Sonnets,a fourteen-line poem written in iambic pentameter. So 14 lines of sentence will be our output at a time.
