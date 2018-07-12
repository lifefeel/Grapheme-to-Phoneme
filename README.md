# Grapheme-to-Phoneme(G2P)
Grapheme-to-Phoneme 관련자료 모음

## Tutorials
* [Building a phonetic dictionary](https://cmusphinx.github.io/wiki/tutorialdict/)
  * CMUSphinx 툴에서 제공하는 오픈소스 G2P로 발음사전을 구축할 수 있는 튜토리얼 
## Tools
* [Sequitur G2P](http://www-i6.informatik.rwth-aachen.de/web/Software/g2p.html) - A trainable Grapheme-to-Phoneme converter
  * 위 링크에서 오리지널 소스코드를 받을 수 있으나 2016년 5월에 마지막 버전이 출시된 이후 업데이트가 되지 않고 있다. [@jtrmal](https://github.com/jtrmal)이란 사람에 의해 별도로 github 레포지토리가 유지되고 있다. 
  * github 레포지토리 - https://github.com/sequitur-g2p/sequitur-g2p
* [Sequence-to-Sequence G2P toolkit](https://github.com/cmusphinx/g2p-seq2seq) - CMUSphinx에서 공개한 오픈소스 Seq2Seq G2P

## Dataset
* [CMU US English Dictionary](https://github.com/cmusphinx/cmudict)
  * 공식사이트는 [Speech at CMU](http://www.speech.cs.cmu.edu/)에 있는 [CMUdict](http://www.speech.cs.cmu.edu/cgi-bin/cmudict) 페이지 인 것 같으나 최근까지 업데이트 되고 있는 버전은 위의 링크인 github 레포지토리이다.

## Papers
### 통계적 방법을 이용한 G2P
* [Joint-Sequence Models for Grapheme-to-Phoneme Conversion (2008.05)](https://www.sciencedirect.com/science/article/pii/S0167639308000046?via%3Dihub)
  * Sequitur G2P를 개발한 Maximilian Bisani의 논문
* [GRAPHEME-TO-PHONEME CONVERSION SCHEME FOR SENTENCE-BY-SENTENCE LEARNING OF KOREAN MANUSCRIPT USING JOINT SEQUENCE STATISTICAL MODEL(2016)](http://troindia.in/journal/ijcesr/vol3iss7part2/88-91.pdf)
  * 한국어에 대해 문장단위로 학습하는 것을 제안한 논문

### DNN 기반 G2P
* [Sequence-to-Sequence Neural Net Models for Grapheme-to-Phoneme Conversion (2015.05)](https://arxiv.org/abs/1506.00196)
  * BLSTM을 사용한 encoder-decoder 모델
  * PER 5.45%, WER 23.55% (CMUDict)
  * PER 7.38%, WER 30.77% (NetTalk)
  * PER 6.51%, WER 26.69% (Pronlex)
* [Deep Bidirectional Long Short-Term Memory Recurrent Neural Networks for Grapheme-to-Phoneme Conversion utilizing Complex Many-to-Many Alignments (2016.09. Interspeech2016)](https://www.isca-speech.org/archive/Interspeech_2016/pdfs/1229.PDF)
  * LSTM LM을 이용한 BLSTM 모델
  * PER 5.37%, WER 23.23% (CMUDict)
* [Grapheme-to-phoneme conversion using Long Short-Term Memory recurrent neural networks (2015.04)](https://static.googleusercontent.com/media/research.google.com/ko//pubs/archive/43264.pdf)
  * LSTM및 n-gram FST를 조합한 모델
  * WER 21.3% (CMUDict)
* [Jointly Learning to Align and Convert Graphemes to Phonemes with Neural Attention Models (2016.10)](https://arxiv.org/abs/1610.06540)
  * LSTM encoder-decoder + global attention 앙상블 모델
  * PER 4.69%, WER 20.24% (CMUDict)
* [Multitask Sequence-to-Sequence Models for Grapheme-to-Phoneme Conversion (2017.08.  Interspeech2017)](http://www.isca-speech.org/archive/Interspeech_2017/pdfs/1436.PDF)
  * Sequitur G2P + Multitask learning + BLSTM + Attention 모델 
  * PER 5.76%, WER 24.88% (CMUDict)
* [Massively Multilingual Neural Grapheme-to-Phoneme Conversion (2017.08)](https://arxiv.org/abs/1708.01464)

### Korean G2P 관련 논문
* [A linguistically motivated approach to grapheme-to-phoneme conversion for Korean (2006)](https://www.sciencedirect.com/science/article/pii/S0885230805000239) - Kyuchul Yoon, Chris Brew
  * 미국 오하이오 주립대 언어학과에서 발표한 논문
* [Grapheme-to-Phoneme Conversion Using Automatically Extracted Associative Rules for Korean TTS System (2006)](https://www.isca-speech.org/archive/archive_papers/interspeech_2006/i06_1405.pdf) - Jinsik Lee, Seungwon Kim and Gary Geunbae Lee, Interspeech 2006
  * 포항공대 이근배 교수 연구실에서 발표한 논문
* [Rule-based Korean Grapheme to Phoneme Conversion Using Sound Patterns (2009)](http://www.aclweb.org/anthology/Y09-2049) - Yu-Chun Wang, Richard Tzong-Han Tsai
  * 타이완 대학 연구실에서 발표한 논문
* [A data-driven grapheme-to-phoneme conversion method using dynamic contextual converting rules for Korean TTS systems (2009)](https://www.sciencedirect.com/science/article/pii/S0885230809000023) - Jinsik Lee, Gary GeunbaeLee
  * 포항공대 이근배 교수 연구실에서 발표한 논문
* [GRAPHEME-TO-PHONEME CONVERSION SCHEME FOR SENTENCE-BY-SENTENCE LEARNING OF KOREAN MANUSCRIPT USING JOINT SEQUENCE STATISTICAL MODEL(2016)](http://troindia.in/journal/ijcesr/vol3iss7part2/88-91.pdf)
  * 한국어에 대해 문장단위로 학습하는 것을 제안한 논문
  
