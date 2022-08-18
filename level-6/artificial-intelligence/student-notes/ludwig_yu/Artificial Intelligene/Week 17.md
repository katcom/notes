Week 17


# <section-title>Week 17</section-title>

## <section-title>Transformer</section-title>

A deep neural network model which is able to take account of both the sequence and context of a sequencing of symbols that are coming in.

### What is a transformer

Sequence and context via self-attention. It is basically a model that can predicts words based on the sequence(the order of words) and the context (the co-occurrence of words) of the upcoming data. It outperforms almost all the other models available.

### Before Transformers

**Context with bag of words** ignores the sequence (the order of words) but takes on the context. It tokenizes the words and then analyse which words tends to occur with other words. For example, in the sentence "I love music more than anything in the world", the "music" co-occurs with 'love' and 'more'. Then it uses deep learning network to analyze these patterns. This technique is good at things like analyzing sentiment of a movie review. However, it's not good for generating text as it ignores the order of words.

**Recurrent Neural Network** is all about the order of words (the sequence) but ignores the context of words. To analyze the order of words in a sentence, we could encode the words using ont-hot encoding in which the position of each word is represented by a 1 in a vector with other positions set to 0. For example:

"I love music" would be encoded into

<center>

| Word | Encoding |
| --- | --- |
| I   | 100 |
| Love | 010 |
| Music | 001 |

</center>We use this to model the " space of words". However, there is no connection between how locse the words are. Here is where the \\\*\\\\\\*Embedding Space\\\\\\*\\\* come to play a role. We take each word and use statistical analysis to dimensionally reduce it. We calculate the space between words(how close they are to each other). When placing words into the space, we use the statistical information of the words such that words that have a similar meaning to others sometimes end up in a similar space. In this embedding space, the positions in space are mmuch more meaningful and the relationship between two words are more meaningful than in one-hot encoding. Each of the words is encoded to a vector and we feed the sequence into network (commonly recurrent neural networks, such as LSMN). Basically you teach it to predict the next symbol.

However, this method doesn't understand that certain words are more important when they co-occur.

### Self-attention

What the Transformers differ from the bag of words and recurrent neural network is that it takes account of both the sequence and the context of the text. Basically, it adds the contextual information to the sequential information when we place the words into the embedding space.

It uses a new type of embedding which employs the so-called "self-attention" concept. For instance, when we put the word "love" into the space, we also feeds in information from the other words that are in the sequence(the context). That is the trainable part in the model. In the so-called "self-attention" layers, we train a way of processing the other words in the context in order to apply them. Just like the convolutional neural network, multiples filters are applied to the other words that appeared in the sequence, such that you can then take account in your new model. There could be multiple filters. In the the so-called multi-headed attention, multiple filters process those word embeddings into new embeddings, self attention embeddings, such that you can take account of the balance of words in different way(extract different features). This is the secret of success of the Transformers.

<reading-section-title>Furthur Reading</reading-section-title>

<reading-section>[Chollet,F,Deep Learning with Python second edition, Manning 2021, Chapter 11](D:%5CUol%5CCM3020-AI%5CCase_Study_4/Deep_Learning_with_Python.pdf) [Vaswani, A., Shazeer, N.M., Parmar, N., Uszkoreit, J., Jones, L., Gomez, A.N., Kaiser, L., & Polosukhin, I. (2017). Attention is All you Need. ArXiv, abs/1706.03762.](D:%5CUol%5CCM3020-AI%5CCase_Study_4/2017_ArXiv_abs_Vaswani_Attention_is_All_you_Need.pdf)</reading-section>

* * *

## <section-title>GPT-2</section-title>

"Due to out concerns about malicious applications of the technology we are not releasing the trained model"

### What is GPT-2

### How does it work?

It uses self-attention with multiple "heads"so it generates multiple multiple attention projections.

It can be used in auto-regressive mode: it can generate an endless stream of words.

### Zero-shot concept

GPT-2 out-performed several state of the art systems in zero-shot mode.

You don't have to retrain it or have a specialized dataset for a particular task

### Huggingfacce

> "We are on a mission to democratize good machine learning, one commit at a time"

A group of people doing NLP. A lot of models. We use their models for generating lyrics in this study case.

<reading-section-title>Furthur Reading</reading-section-title>

<reading-section>[The Illustrated GPT-2 (Visualizing Transformer Language Models)](http://jalammar.github.io/illustrated-gpt2) [Radford, Alec et al. “Language Models are Unsupervised Multitask Learners.” (2019).](https://www.semanticscholar.org/paper/Language-Models-are-Unsupervised-Multitask-Learners-Radford-Wu/9405cc0d6169988371b2755e573cc28650d14dfe)</reading-section>

## Fine Tuning

Extra burst of training on a smaller dataset to bias the network slightly

<style>
	section-title{
		color:black;
		text-align:center;
		display: flex;
		justify-content: center;
		background:white;
	}
	section-content {
		display:flex;
		text-indent:1em;
	}
	p {
		text-indent:1em;
	}
	reading-section{
		display:flex;
		flex-direction:column;
		font-size:16px;
		font-style:italic;
		font-family:times;
	}
	reading-section-title{
		display:flex;
		text-align:center;
		justify-content: center;
		font-size:18px;
		font-style:italic;
		font-family:times
	}
	reading-section a{
		margin-top:10px
	}
	a{
		color:black
	}

</style>