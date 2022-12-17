
*Transformer is first introduced in the paper "Attention Is All You Need" by Google at 31st Conference on Neural Information Processing Systems (NIPS 2017), Long Beach, CA, USA [1]. The paper is published on https://arxiv.org/pdf/1706.03762.pdf. This article is based on the original paper.*



Transformer is a type of neural network architecture that was introduced in a paper published in 2017 by researchers at Google. It has since become a popular architecture for natural language processing (NLP) tasks, such as machine translation and text summarization, because of its ability to process long sequences of text effectively.

Before the introduction of the Transformer architecture, most natural language processing (NLP) models were based on recurrent neural networks (RNNs), which use a looping structure to process sequential data such as text. These models were effective for many NLP tasks, but had some limitations.

One of the main limitations of RNNs is their sequential nature, which makes them difficult to parallelize during training. This means that it can be computationally expensive to train large RNN models on large datasets, which can limit their performance.

Another limitation of RNNs is their ability to capture long-term dependencies in language. Because RNNs process input sequentially, they may have difficulty capturing the relationships between words that are far apart in a sentence or paragraph. This can lead to less accurate results for tasks such as language translation.

So how does Transformer revolutionise NLP? 

First of all, the Transformer architecture is its use of self-attention mechanisms, which allow the model to weigh the importance of different words in a given sequence based on their relationships to each other. This allows the model to better capture the meaning of a sentence or paragraph, and perform tasks such as language translation more accurately.

Second, the Transformer architecture is its use of parallelizable computation, which allows it to be trained much more efficiently on large datasets compared to previous architectures. This has made it possible to train much larger and more powerful language models, which has in turn led to significant advances in the field of NLP.

The Transformer architecture has also been successful because it is a general-purpose model that can be used for a wide range of NLP tasks, such as machine translation, text summarization, and sentiment analysis. This has led to its widespread adoption in the NLP community, and has made it a key component of many state-of-the-art NLP systems.

In this article, we will look deeper into what Transformer is and why it is so popular compared to other models like RNN in NLP.





[1] A. Vaswani, N. Shazeer, N. Parmar, J. Uszkoreit, L. Jones, A. N. Gomez, L. Kaiser, and I. Polosukhin, “Attention is all you need,” *arXiv.org*, 06-Dec-2017. [Online]. Available: https://arxiv.org/abs/1706.03762. [Accessed: 15-Dec-2022]. 