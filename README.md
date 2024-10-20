# Machine-Translation-with-Transformer

A project takes reference from https://www.geeksforgeeks.org/machine-translation-with-transformer-in-python/

Machine translation converts a sequence of text from one language to another. Popular online translation services like Google Translate, Microsoft Translator, and others use machine translation techniques to provide users with quick and accessible translations between a wide range of languages. Transformer models are the most recent and widely adopted approach to machine translation. They are based on Seq2Seq architecture and capture context to learn the mappings between source and target languages. 

In my project, I will be using a model for hugging faces and fine-tuning it to convert our text from Japanese to English.

The transformer architecture can process all the parts of input in parallel through its self-attention mechanism without the need to sequentially process them. The transformer architecture has two parts: an encoder and a decoder. If we want to build an application to convert a sentence from one language to another (Japanese to English), we need to use both the encoder and decoder blocks. This was the original problem (known as a sequence-to-sequence translation) for which the transformer architecture was developed.

However, depending on the type of task, we can either use the encoder block only or the decoder block only of the transformer architecture. The core of the encoder and decoder blocks is multi-head attention. The only difference is the use of masking in the decoder block. These layers tell the model to pay specific attention to certain elements in the input sequence and ignore others when computing the feature representations.

Helsinki-NLP is a Natural Language Processing (NLP) model that can translate different types of content. The University of Helsinki has been actively involved in various NLP projects and research endeavours. One notable project is the Helsinki-NLP GitHub repository, where the University of Helsinki’s NLP researchers and developers contribute to open-source projects related to natural language processing. This repository includes implementations, models, and tools for a variety of NLP tasks. We will use the helsinkis Japanese to English model and fine-tune it on our dataset.
