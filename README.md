# Massively Multilingual & Multimodal Machine Translation 

### 1. Name of student 

Sheiphan Joseph (PRN: 20220804003) 

Pratik Ghute (PRN: 20220804042) 

### 2. Description 

Researchers have introduced a new tool called SeamlessM4T, which aims to address the limitations in unified speech-to-speech translation systems. These systems typically rely on multiple subsystems for translation, making them less scalable and efficient. To create SeamlessM4T, the researchers used 1 million hours (about 114 years) of open speech audio data to train self-supervised speech representations with a model called w2v-BERT 2.0. They also created a multimodal corpus of aligned speech translations called SeamlessAlign, which included human-labeled and pseudo-labeled data totaling 406,000 hours (about 46 and a half years). 

SeamlessM4T is a single model that supports various translation tasks, including speech-to-speech, speech-to-text, text-to-speech, and text-to-text translation, as well as automatic speech recognition for up to 100 languages. The system achieved significant improvements in translation quality over existing models, including a 20% increase in BLEU score for speech-to-text translation and improvements in speech-to-speech translation quality. It also performed well in human evaluations and demonstrated robustness against background noises and speaker variations. 

### 3. Data set 

- Flores-200 [NLLB Team et al., 2022]: a many-to-many multilingual translation benchmark dataset for 200 languages (we evaluated on devtest).  
facebookresearch/flores: Facebook Low Resource (FLoRes) MT Benchmark (github.com) 

 

- Fleurs [Conneau et al., 2022]: an n-way parallel speech and text dataset in 102 languages built on the text translation Flores-101 benchmark [Goyal et al., 2022]. Fleurs is well suited for several downstream tasks involving speech and text. We evaluated on the test set, except in ablation experiments where we evaluated on the dev set. arxiv.org/pdf/2205.12446.pdf 

 

- CoVoST 2 [Wang et al., 2021c]: a large-scale multilingual S2TT corpus covering translations from 21 languages into English and from English into 15 languages. We evaluated on the test set. 2007.10310.pdf (arxiv.org) 

 

- CVSS [Jia et al., 2022b]: a multilingual-to-English speech-to-speech translation (S2ST) corpus, covering sentence-level parallel S2ST pairs from 21 languages into English. We evaluated text-based semantic accuracy on CVSS-C for the tasks of S2ST and T2ST. We note  that some samples from the evaluation data were missing (in 8 out of 21 languages: Catalan, German, Estonian, French, Italian, Mongolian, Persian, and Portuguese). 2201.03713.pdf (arxiv.org) 

 
