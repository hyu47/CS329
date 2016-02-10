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

* Go to [microsoftazurepass.com](http://www.microsoftazurepass.com) and enter your promo code to open an Azure account ([instructions](http://www.microsoftazurepass.com/howto)).
* Go to [portal.azure.com](https://portal.azure.com).
* Create a new **virtual machine** (on the left menu):
 * Select **Ubuntu Server 14.04 LTS**.
 * Name the virtual machine **cs329**.
 * Use your Emory ID and password.
 * Create a default resource group.
 * Select the location **East US 2**.
 * Select the machine **DS3 Standard** (you may need to click "view all").
 * Wait for a while until the virtual machine is deployed.
 * If you click "Virtual Machines" on the left menu, you should see `cs329`.
 * Click `cs329` and get the public IP address (e.g, `104.209.xxx.xx`)
* Login to your Azure account by typing the following command on the terminal (replace `yourID` with your Emory ID and `104.209.xxx.xx` with your public IP address).  If you are using a Windows machine, use [putty](http://www.chiark.greenend.org.uk/~sgtatham/putty/download.html) for a terminal.

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

* Check the Java version.

   ```
   java -version
   ```

* Enter the following command on the terminal:

   ```
   cat /proc/cpuinfo > cpuinfo.txt
   ```

* Login to your `mathcs` account:

   ```
   ssh yourID@
   ```

* Logout your Azure account by entering the following command:

   ```
   exit
   ```

