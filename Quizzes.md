## Quiz 1

Currently, our tokenizer cannot handle acronyms and `'s` when they are followed by another punctuation (e.g., `"U.S."` or `Jinho's,`).  Your task is to improve the tokenizer so it can handle such cases.
* Download [`tokenize_punctuation.py`](../tree/master/src/tokenization/tokenize_punctuation.py).
* Modify `tokenize_punctuation.py` so it can handle the above situation.
* Put `tokenize_punctuation.py ` under the directory `cs329/quiz1`.