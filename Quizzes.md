## Quiz 1

Currently, our tokenizer cannot handle acronyms and `'s` when they are followed by another punctuation (e.g., `"U.S."` or `Jinho's,`).  Your task is to improve the tokenizer so it can handle such cases.
* Download [`tokenize_punctuation.py`](../tree/master/src/tokenization/tokenize_punctuation.py) or [`tokenize_regex.py`](../tree/master/src/tokenization/tokenize_regex.py).
* Modify `tokenize_*.py` so it can handle the above situation.
* Put `tokenize_*.py ` under the directory `cs329/quiz1`.

## Quiz 2

Write phrase structure trees for the following sentence in the Penn Treebank format.
```
Emory University is a private research university in metropolitan Atlanta, located in the Druid Hills.
```
* Examples of phrase structure trees in the Penn Treebank can be found [here](../tree/master/src/phrase_structures/wsj_00.parse).
* The Penn Treebank guidelines can be found [here](http://www.sfs.uni-tuebingen.de/~dm/07/autumn/795.10/ptb-annotation-guide/root.html).
* Create a text file `quiz2.txt` containing two trees in the parenthetical notation and put it under the directory `cs329/quiz2`.
* Stanford parser: [demo](http://nlp.stanford.edu:8080/parser).

## Quiz 3

* Create a virtual machine at Azure: [guidelines](Microsoft-Azure).
* Login to your Azure account by typing the following command on a terminal. If you don't have a terminal, try [putty](http://www.chiark.greenend.org.uk/~sgtatham/putty/download.html). Replace `yourID` with your Emory ID and `104.209.xxx.xx` with your public IP address.

  ```
  ssh yourID@104.209.xxx.xx
  ```

* Install Java 8 by running the following commands:

   ```
   sudo apt-add-repository ppa:webupd8team/java
   sudo apt-get update
   sudo apt-get install oracle-java8-installer
   sudo apt-get install oracle-java8-set-default
   ```

* Enter the following commands:

   ```
   cat /etc/*-release > info.txt
   java -version 2>> info.txt
   ```

* Login to your `mathcs` account:

   ```
   ssh yourID@lab0z.mathcs.emory.edu
   ```

* Create a directory `cs329/quiz3` by entering the following command:

   ```
   mkdir -p cs329/quiz3
   ```

* Copy `info.txt` from your Azure account to your `mathcs` account:

   ```
   scp yourID@104.209.212.48:~yourID/info.txt cs329/quiz3/
   ```   

* Check if `info.txt` is copied to your `mathcs` account by running the following command:

   ```
   cat cs329/quiz3/info.txt
   ```