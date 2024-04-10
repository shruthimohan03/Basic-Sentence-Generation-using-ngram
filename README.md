# Sentence Generation using N-grams from Text Data

This code demonstrates the process of generating sentences using an n-gram model based on a dataset of text. Here's a brief description of each part:

1. Reading and Preprocessing Data:
   - The code reads a dataset from a CSV file named 'Context.csv' using pandas.
   - It selects only the 'Text' column from the dataset and takes a subset of the data (first 3000 rows).
   - The text data is converted to lowercase and tokenized using NLTK's word_tokenize function.

2. Creating the N-gram Model:
   - The code defines a function named `generate_ngram` that creates n-grams (bigrams in this case) from a list of words and stores them in a dictionary named `master_ngram`.
   - For each sentence in the preprocessed data, the `generate_ngram` function is called to create and store the n-grams in the `master_ngram` dictionary.

3. Generating Sentences:
   - Another function named `generate_sentence` is defined to generate sentences based on the provided n-gram model.
   - Given an input sentence, the code preprocesses it, creates n-grams, and appends them to the `master_ngram` dictionary.
   - The `generate_sentence` function then uses the input sentence and the n-gram model to generate a new sentence.

4. Example Usage:
   - The code provides three example input sentences: "I want to understand", "I want to know how someone", and "I want to make a statement".
   - Each input sentence undergoes preprocessing, n-gram creation, and sentence generation using the previously defined functions.
   - The generated sentences based on each input are printed out.

Overall, this code demonstrates a basic approach to generating sentences using an n-gram model trained on a dataset of text. It shows how to preprocess the data, create the n-gram model, and use it to generate sentences based on user-provided input.
