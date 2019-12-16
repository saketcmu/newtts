# A new Algorithm for Text to Speech
A Text to Speech synthesis system typically consists of multiple stages with encoder, decoder and waveform synthesis stages.  Designing each of these  modules  is  a  challenging  task.   Each  of these components needs to be designed carefully and several design choices are available for these components. Tacotron is an End-to-End generative Text to Speech (TTS) model that synthesizes speech directly from characters.  

The backboneof Tacotron is a seq2seq model with attention. The building block of Tacotron is called a CBHGmodule. CBHG module transforms prenet’s output into encoder’s hidden representation, which is later decoded by the decoder.  More recently,LSTM has been shown to simplify the task of extracting interesting features from segments of data.   These properties of LSTM make it very attractive to use in TTS models to easily store the dependency.  In this work, we have focused on building an alternate architecture for Text toSpeech engine which makes use of the numerous advantages of LSTM. A custom block consisting of 3 layer bidirectional LSTM with residual connections are designed.  The performance of our architecture was compared against the performance of regular Tacotron.

https://colab.research.google.com/drive/1FgwJp6-dSw7nYjnXSP3HJYXXrodj_5a8

