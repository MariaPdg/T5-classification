# **Fine-Tuning the  Multilingual Text-To-Text Transfer Transformer (mT5) for Language Classification**

## _Or: What's the language of a given sentence?_

_We demonstrate how to fine-tune a pre-trained T5 model and its multimodal extension mT5, evaluating its accuracy, and using it for the language prediction task on GPU with TensorFlow._

Here you find how to to do the following:
* Preprosess [XNLI](https://www.tensorflow.org/datasets/catalog/xnli) dataset
* Create new [seqIO](https://github.com/google/seqio) `Task` with `tf.data.Dataset` 
* Fine-tune [mT5](https://github.com/google-research/multilingual-t5) model as well as [T5](https://arxiv.org/pdf/1910.10683.pdf)  for the new `Task` 
* Log with `TensorBoard`
* Make some predictions with the trained model

## Background

T5 was introduced by C. Raffel et al. in the paper [_Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer_](https://arxiv.org/abs/1910.10683). T5 is the Text-To-Text Transfer Transformer, which allows converting text-based language problems into a text-to-text format. The authors achieved state-of-the-art performance with [_Colossal Clean Crawled Corpus (C4)_](https://www.tensorflow.org/datasets/catalog/c4) in covering summarization, question answering, text classification, and other English-based NLP problems.

In this notebook, I aim to give a brief overview of T5, explain some of its implications for NLP, and demonstrate how it can be used for language classification task. 

The full version of the project is available under the [Link](https://colab.research.google.com/drive/1-ZYNdqJ5O5b818FTGAipxogeohTcA47l?usp=sharing)
