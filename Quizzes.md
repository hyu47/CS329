## Quiz 1

Currently, our tokenizer cannot handle acronyms and `'s` when they are followed by another punctuation (e.g., `"U.S."` or `Jinho's,`).  Your task is to improve the tokenizer so it can handle such cases.
* Download [`tokenize_punctuation.py`](../tree/master/src/tokenization/tokenize_punctuation.py) or [`tokenize_regex.py`](../tree/master/src/tokenization/tokenize_regex.py).
* Modify `tokenize_*.py` so it can handle the above situation.
* Put `tokenize_*.py ` under the directory `cs329/quiz1`.

## Quiz 2

Write phrase structure trees for the following two sentences in the Penn Treebank format.
```
Emory University is a private research university in metropolitan Atlanta, located in the Druid Hills.
```
* Examples of phrase structure trees in the Penn Treebank can be found [here](../tree/master/src/phrase_structures/wsj_00.parse).
* The Penn Treebank guidelines can be found [here](http://www.sfs.uni-tuebingen.de/~dm/07/autumn/795.10/ptb-annotation-guide/root.html).
* Create a text file `quiz2.txt` containing two trees in the parenthetical notation and put it under the directory `cs329/quiz2`.


