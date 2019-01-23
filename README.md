# Roman-to-Devanagari-conversion-for-code-mixed-language

Nowadays people are not very particular about expressing themselves in pure Hindi or pure English. But they tend to mix them up. This project is aimed at understanding code-mixed words written on social media. Mainly we group the words in three categories: English, Hindi and code-mixed We will take the code-mixed words and try to identify whether the word is English or Hindi and then we convert it into Devanagari form. Sufficient parallel transliteration pairs are needed for training state of the art transliteration model. 


Neural Machine Translation is one of the approach to machine translation. Unlike the traditional phrase-based translation system which consists of many small sub-components that are tuned separately, neural machine translation attempts to build and train a single, large neural network that reads a sentence and outputs a correct translation. characters of those languages are hypothesized which encode different features. Thus the character structure is captured for both the languages. The identified words are then translated by using encoders-decoders LSTM network.
![alt text](https://github.com/MShivaG/Roman-to-Devanagari-conversion-for-code-mixed-language/blob/master/NLP.png)

Our flow of work:
  1.Build a token level language identification model
  2.Build a translation model for English words and transliteration model for Hinglish words.
Our contribution towards creating the model:
  1.Char by char method is used for training our model.
  2.The character structure is captured for each language.
  3.Thus model understand the morphological difference between the English and the Hindi words.
  4.Encoder and Decoder are used in our model where encoder encodes the source word and decoder outputs translation from encode vector
Results:
  The Language Identification model works well by char - char method. But the English - Hindi model doesnt work by char by char method. It might work in Hinglish to Hindi model.
