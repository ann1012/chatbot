<h1>Chatbot</h1>
A neural chatbot has been created using PyTorch platform.
loss function used is cross-entropy


<h2>Training</h2>
 The input sentence is given to the encoder. The latest hidden state is the first hidden state of the decoder.
  Its first input is the start of the sentence.

In order to train the model the following steps are followed.
A timer is started.
Optimizers and criterion initialized.
A set of training pairs created. 
Train function is  called many times.

<h2>Architecture</h2>
The model consists of  a Seq2Seq Model consisting of an Encoder Decoder network. 
Both encoder and decoder are RNNs. The input is fed into the encoder. The output vector from the encoder is then given to the decoder to produce the output sequence. 

Here instead of the simple decoder an attention decoder is used. This is to give weightage to different part of the encoder output for every decoder output step. 
