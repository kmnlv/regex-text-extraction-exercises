# Regular Expressions for Text Extraction in Python

> Course: Natural Language Processing · Semester 2

## Overview

Two notebooks that move from regex fundamentals to a practical extraction challenge. The first is a guided 53-cell practice using a public-domain novel; the second applies eleven patterns to a Spanish-language sample paragraph containing realistic contact and transaction data.

## Repository structure

- `notebooks/regex-foundations.ipynb` - guided practice on Project Gutenberg's *El idiota* (Dostoievski).
- `notebooks/regex-extraction-challenge.ipynb` - eleven extraction and cleanup tasks.

## Topics covered

`match`, `search`, `findall`, `finditer`, `sub` and `split`; character classes and negated classes; anchors `^` and `$`; quantifiers (`+`, `*`, `?`, `{9,10}`); capturing and named groups `(?P<name>...)`; greedy versus non-greedy matching; and `re.IGNORECASE` / `re.VERBOSE` flags.

## Practical tasks

Extract email addresses, URLs, phone numbers, ISO dates, postal codes, national ID codes, mentions and hashtags, IP addresses and monetary amounts, plus repeated-letter cleanup with `re.sub`.

## Requirements

Python 3 standard library `re`, plus `requests` to download the Gutenberg text in the first notebook, and `jupyter`.

## How to run

```bash
pip install -r requirements.txt
jupyter notebook notebooks/
```

The first notebook fetches `https://www.gutenberg.org/files/2638/2638-0.txt`, so it needs network access. The second is fully self-contained.

---
Author: Karla Maria Monroy Alvarez
