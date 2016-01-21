## Quiz 1

Currently, our tokenizer cannot handle acronyms and `'s` when they are followed by another punctuation (e.g., `"U.S."` or `Jinho's,`).  Your task is to improve the tokenizer so it can handle such cases.
* Download [`tokenize_regex.py`](../tree/master/src/tokenization/tokenize_regex.py).
* Modify `tokenize_regex.py` so it can handle the above situation.
* Put `quiz1.py` under `cs329/quiz1`.