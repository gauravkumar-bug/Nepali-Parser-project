# Nepali Parser (Basic NLP Project)

This is a small Python project I made to understand how NLP works for Nepali text.
It takes a Nepali sentence as input and shows:

* tokens (words)
* POS tags (like noun, verb, etc.)
* basic dependency relations

---

## What it does

* Splits sentence into words
* Tags each word using a dictionary + some rules
* Finds a root verb and assigns simple roles (subject, object, etc.)

---

## Files

```
nepali_parser.py
requirements.txt
README.md
```

---

## How to run

Just run the Python file:

```
python nepali_parser.py
```

Then type a sentence like:

```
राम किताब पढ्छ।
```

Type `exit` to stop.

---

## Example output

```
Sentence: राम किताब पढ्छ
Tokens: ['राम', 'किताब', 'पढ्छ']

POS Tags:
  राम -> PROPN
  किताब -> NOUN
  पढ्छ -> VERB

Dependencies:
  राम -> nsubj
  किताब -> obj
  पढ्छ -> ROOT
```

---

## Notes

* This is rule-based, not machine learning
* Accuracy depends on the dictionary
* Unknown words are handled using simple suffix rules

---

## Future ideas

* Add more Nepali words to dictionary
* Improve tagging using context
* Try using libraries like nltk or spacy later

---

## Why I made this

Mostly for practice and to understand:

* how POS tagging works
* how parsing works
* and how NLP systems are built from scratch

---
