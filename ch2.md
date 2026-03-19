# Working with text data
- preparing text for llm training

### Understanding word embeddings
- Deep neural network models, including LLMs cannot process raw text directly, since text is catagorical and not compatible with mathematical operations used to implement and train neural networks.
- Converting data into a vector format is often called embedding.
```
video data => [ video embedding model ] => video embedding vector
audio data => [ audio embedding model ] => audio embedding vector
```
- Sentence or paragraph embeddings are popular choices for retrieval-augmented generation.
- RAG combines generation with retrieval(like searching and external knowledge base) to pull relevant information.
- In Word2Vec embedding techniques, words corresponding to similar concepts often appear close to each other in the embedding space
- embedding size often referred to as the dimensionality of the model

### Tokenizing text
```
Input text:            This is an example.
                              | 
                              V
Tokenized text:   [This] [is] [an] [example] [.]


Token IDs:      [40134] [2025] [133] [389] [12]


Token embeddings: [][][][]   [][][] [][][]  [][][]  [][][]

```

