# Build a GPT-like LLM based on the transformer architecture from scratch 

## Understanding LLMs
- LLMs are deep neural network models 
- LLMs are capable of understanding, generating and interprateting human language
- process and generate text in ways that appear coherent and contexually relevant

### What is an LLM ?
- An LLM is a neural network designed and trained to understand, generate, and respond to human-like text.
- "large" refers to both the model's size in terms of parameters and immense dataset on which it's trained.
- LLMs use an architecture called the "transformers", which allow them to pay selective attention to different parts of the input
- LLMs are also referred as a form of GenAI ( generative AI ) since capable of generaring text

``` 

        system with human like intelligence
    AI +-------------------------------------------------------------------------------------------------------------
       |            algorithms that learn rules automatically from data 
       |      ML +---------------------------------------------------------------------------------------------------
       |         |        ml with neural networks consisting of many layers
       |         |    DL +-------------------------------------------------------------------------------------------
       |         |       |
       |         |       |                   GenAI +-----------------+
       |         |       |                         |                 | use of dl neural networks to create new content 
       |         |       |       LLM +-------------|- - - - - - - - -|----------------------------------------------
       |         |       |            |            |                 |  
       |         |       |            |            |_________________|  
       |         |       |            |
       |         |       |            |-----------------------------------------------------------------------------
       |         |       |            dl neural network for parsing and generationg human text  
       |         |       |__________________________________________________________________________________________
       |         |
       |         |
       |         |__________________________________________________________________________________________________
       |
       |____________________________________________________________________________________________________________

```


### Stages of building and using LLMs
- Most LLMs are implemented using PyTorch deep learning library
- "first step" is to train it on a large corpus of text data or raw data ( unlabelled text )
- "first training stage is called pretraining, pre-trained LLM a base model, then it is further trained called fine-tuning

### Transformer architecture
- The transformer architecture consists of two submodules: an encoder and a decoder connected by "self-attention" mechanism.
```
Input text => [Encoder] => Embeddings
                +--------------|
                |
                V
Input text => [Decoder] => Output

```
- The mmodel is simply trained to predict the next "word". This is a form of self-supervised learning,which is a form of self-labeling.
- In GPT, each new word is chosen based on the sequence that precedes it.
- The GPT architecture employs only the decoder portion of the transformer.


### Building a large language model
- 3 main stages of coding an LLM, 
     -  1) implementing LLM architecture and data process,
     -  2) pretraining LLM to create a foundation model, 
     -  3) fine-tuning the foundation model


