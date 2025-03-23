# LLM-fro-scratch
Modern language models (like GPT-4) use transformers, a deep learning architecture that learns word relationships through self-attention. We’ll build a basic transformer-based model to understand how to build a large language model from scratch. 
"The goal of our language model will be to predict the next word".

The six main components we’ll cover:
1)Tokenization:Computers can’t understand words directly, so we map each word to a unique number (ID). This process is called tokenization. 

2)Embedding Layer:Numbers alone (like 0 and 1) don’t carry meaning. An embedding layer transforms these numbers into vectors (lists of numbers), allowing words with similar meanings to have similar representations

3)Positional Encoding:Transformers process all words at once, so they don’t naturally understand order (e.g., “I love you” ≠ “You love I”). Positional encoding fixes this by adding a unique “position signal” to each word.

4)Self-Attention:Self-attention helps the model focus on important words. For example, in “The cat sat on the mat”, “sat” relates more to “cat” than “mat”

5)Transformer Block:A single attention layer isn’t enough. Transformer blocks combine attention with deeper processing

6)Full Language Model:Combine all the components into one model that predicts next word
REFER THE CODE FILE(LLM from scratch.ipynb) ATTACHED FOR BETTER UNDERSTANDING

To scale up this model into a practical LLM, several key changes are needed. First, the vocabulary size must expand from just 6 words to 50,000+ words or subwords using techniques like Byte-Pair Encoding (BPE) and tokenizers from libraries like Hugging Face. Instead of two sentences, real-world training requires millions of sentences sourced from books, Wikipedia, or large datasets. 
