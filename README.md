
----->Lab 1: Text Preprocessing (No Libraries)<-----
This lab focuses on fundamental text preprocessing by building manual implementations rather than relying on standard libraries.
 * Stopword Removal: You defined a custom, manual list of common stopwords (like "is", "a", "and", "it") to filter out from the text.
 * Punctuation Stripping: The script defines a string of standard punctuation marks and iterates through the input text character by character, keeping only the characters that are not in the punctuation list.
 * Tokenization: Text is broken down into a list of individual tokens using Python's built-in .split() method, which separates the string based on whitespace.
 * Filtering: A loop iterates through the tokenized words, converts them to lowercase to ensure case-insensitivity, and appends them to a new list only if they do not appear in the predefined stop words list.

----->Lab 2 & 3: Word Analysis, Stemming, and POS Tagging<-----
These labs transition into using the Natural Language Toolkit (NLTK) for more complex linguistic tasks.
 * Stemming: The lab uses NLTK's PorterStemmer and word_tokenize to reduce words to their base or root form.
 * Parts of Speech (POS) Tagging: Text is tokenized and then tagged with its corresponding part of speech (like Noun, Verb, Adjective) using NLTK's pos_tag function alongside the averaged_perceptron_tagger.
 * Word Analysis: Using Python's Counter from the collections module, the script calculates the total number of words, extracts unique words using a set, and determines the frequency of each word in a string. It also identifies the longest and shortest words using Python's max() and min() functions with the key=len argument.
 * Random Word Generation: The lab utilizes the NLTK words corpus and Python's random.choice() function to generate a specified number of completely random English words.


----->Lab 4 & 5: Word Sense Disambiguation & Advanced Stemming<-----
This session explores context-dependent meaning and sentence-level stemming operations.
 * Word Sense Disambiguation (WSD): WSD is defined as the process of determining the correct meaning of a word based on its context. The lab implements the Lesk algorithm (from nltk.wsd import lesk) using the wordnet corpus to accurately define a word based on its surrounding sentence (e.g., defining "emotion" as "any strong feeling").
 * Advanced Stemming: The PorterStemmer is applied not just to isolated lists of words, but to fully tokenized sentences using list comprehension to stem every word in a sequence.
 * Custom Task: The lab concludes with a specific assignment: to implement a Porter stemmer entirely without NLTK, specifically to remove common prefixes and suffixes like "ed" and "ing".


----->Lab 6: Dictionary-Based POS Tagging<-----
This lab returns to manual implementation, focusing on a simplified, rule-based approach to linguistic tagging.
 * Dictionary Mapping: A predefined Python dictionary (pos_dict) is created to act as the tagging engine, mapping specific key words directly to their POS values (e.g., "cat" is mapped to "NOUN", "run" to "VERB", "happy" to "ADJECTIVE").
 * Tagging Logic: The script takes a user's word input, converts it to lowercase, and checks if the key exists within the custom dictionary. If a match is found, it prints the designated part of speech; otherwise, it outputs a fallback value of "UNKNOWN".

