# Grapheme-to-Phoneme(G2P)
DNN 기반 Grapheme-to-Phoneme 관련자료 모음

## Papers
* [Sequence-to-Sequence Neural Net Models for Grapheme-to-Phoneme Conversion (2015.05)](https://arxiv.org/abs/1506.00196)
  * BLSTM을 사용한 encoder-decoder 모델
  * WER 23.55% (CMUDict)
* [Deep Bidirectional Long Short-Term Memory Recurrent Neural Networks for Grapheme-to-Phoneme Conversion utilizing Complex Many-to-Many Alignments (2016.09. Interspeech2016)](https://www.isca-speech.org/archive/Interspeech_2016/pdfs/1229.PDF)
  * LSTM LM을 이용한 BLSTM 모델
  * WER 23.23% (CMUDict)
* [Grapheme-to-phoneme conversion using Long Short-Term Memory recurrent neural networks (2015.04)](https://static.googleusercontent.com/media/research.google.com/ko//pubs/archive/43264.pdf)
  * LSTM및 n-gram FST를 조합한 모델
  * WER 21.3% (CMUDict)
* [Jointly Learning to Align and Convert Graphemes to Phonemes with Neural Attention Models (2016.10)](https://arxiv.org/abs/1610.06540)
  * LSTM encoder-decoder + global attention 앙상블 모델
  * WER 20.24% (CMUDict)
* [Multitask Sequence-to-Sequence Models for Grapheme-to-Phoneme Conversion (2017.08.  Interspeech2017)](http://www.isca-speech.org/archive/Interspeech_2017/pdfs/1436.PDF)
  * Sequitur G2P + Multitask learning + BLSTM + Attention 모델 
  * WER 24.88% (CMUDict)
* [Massively Multilingual Neural Grapheme-to-Phoneme Conversion (2017.08)](https://arxiv.org/abs/1708.01464)
