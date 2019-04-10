## Natural Language Process with Deep Learning

Notes I took from reading the slides

- Will cover basics, like recurrent network, attention etc.
- Present a big picture
- Ability to build systems for major porblems like: 
  - word meaning
  - dependency parsing
  - machine translation
  - question answering
- PyTorch, GPU  

Commonst linguistic way of thinking of meaning:
- sigifier &hArr; sigified idea/thing
- denotational semantics
  
How to have usable meaning? WordNet `nltk.corpus`.  
synonym set, hypernyms ('is a' relationship)
- cons: nuance, hard to up-to-date, hard to get acurate similarity, subjective

Traditional discrete symbol: word --> one-hot representation.  
Vector dimention: (~500000). 
- cons: no natrual similarity   

#### LEARN TO ENCODE SIMILARITY in the vecor themselves

Idea:
- distributional semantics: You shall know a word by the company it keeps
- representing words by their context

word vector (embeddings, representation): dense vector. Similar for words which appear in similar contexts.

`Word2vec` idea:
- large corpus of text
- word &hArr; vector
- use similarity of vectors to calculate of prob of o given c
- adjust vector to maximize

Objective function:
- $Likelihood = L(\theta)\prod^T_{t=1} \prod_{-m \le j \le m}p(w_{t+j}|w_j, \theta)$
- $J(\theta) = -\frac{1}{T}logL(\theta)$

For each word, two vectors. One when it's center, one when it's context.

