Next-Word Prediction using GPT-2
This project is about training a next-word prediction model using GPT-2. The idea was to take a pre-trained language model and fine-tune it on the WikiText-2 dataset so that it can learn how to predict what word comes next in a sentence. For example, if I give it a prompt like "Deep learning enables", it should be able to suggest a meaningful word to follow.

I used the HuggingFace transformers library to load the GPT-2 model and tokenizer, and trained it using the Trainer API. The dataset used is wikitext-2-raw-v1, but due to memory limitations, I only used 1000 examples for training and 200 for validation. Even though this is much smaller than the full dataset, it was enough to complete the assignment and demonstrate the concept.

The model was trained for just one epoch with a batch size of 1 (because of memory errors). I also defined simple evaluation metrics like perplexity and top-5 accuracy to see how well the model performs.

In the end, I tested the model on a sample prompt and it successfully generated a next word. Everything is done in a clean notebook format with clear sections for installation, tokenization, training, and testing.

This completes the Week 4 NLP project assignment, and all the steps are well-documented. The dataset size was reduced only due to GPU memory limits, which is explained clearly in the notebook and here.

