## Information Extraction

Your task is to summarize Wikipedia articles with respect to certain entities.


## Preparation

* Copy texts from Wikipedia articles for the last 10 U.S. presidents (e.g., [Barack Obama](https://en.wikipedia.org/wiki/Barack_Obama), [George W. Bush](https://en.wikipedia.org/wiki/George_W._Bush), [Bill Clinton](https://en.wikipedia.org/wiki/Bill_Clinton)), and save them into a single text file `hw2.txt`. Strip out the followings from your text file:
 * References and reference numbers (e.g., `[1]`, `[421]`).
 * Titles, main article info, and any line that does not end with proper punctuation (e.g., `.`).
* Login to your Azure account on a terminal and download the followings:

   ```
   wget http://www.mathcs.emory.edu/~choi/courses/cs329/dat/nlp4j-1.0.1.jar
   wget -O nlp4j-english-1.0.0.jar http://search.maven.org/remotecontent?filepath=edu/emory/mathcs/nlp/nlp4j-english/1.0.0/nlp4j-english-1.0.0.jar
   wget https://raw.githubusercontent.com/emorynlp/nlp4j/master/src/main/resources/edu/emory/mathcs/nlp/configuration/config-decode-en.xml
   wget https://raw.githubusercontent.com/emorynlp/nlp4j/master/src/main/resources/edu/emory/mathcs/nlp/configuration/log4j.properties
   ```

* Parse the text file:

   ```
   java -Xmx8g -XX:+UseConcMarkSweepGC -cp nlp4j-1.0.1.jar:nlp4j-english-1.0.0.jar -Dlog4j.configuration=edu/emory/mathcs/nlp/configuration/log4j.properties edu.emory.mathcs.nlp.bin.NLPDecode -c config-decode-en.xml -i hw2.txt
   ```
* You should see `hw2.txt.nlp` generated.  Download `hw2.txt.nlp` to your local machine.

## Program

* Save [`dependency.py`](https://github.com/emory-courses/cs329/blob/master/src/dependency/dependency.py) as `hw2.py` to your local machine.
* Run `hw2.py` with `hw2.txt.nlp` on a terminal:

   ```
   python hw2.py hw2.txt.nlp
   ```

* Modify `hw2.py` such that it accepts another argument and prints information about the argument. For instance, if the following command is given, only information relevant to `Obama` should be printed on the screen:

   ```
   python hw2.py hw2.txt.nlp Obama
   ```

* Your program can be as simple as printing out all sentences including the keyword or as complicated as making a summarization of the article. Extra credits will be given to the top _k_ programs.

## Report

You should write a report (1-3 pages) including the followings:
* Instruction of how to run your program.
* Description of how you generated `hw2.txt` (e.g., manually stripped out noise, wrote a script, ran an existing tool).
* Description of how you improved your program from the baseline (single word matching). You should explicitly describe what kind of new features you integrated and which examples work for your features.
* Analysis of your program including weakness and strength.

## Submission

Create a directory `cs329/hw2` under your `mathcs` account and put the followings:
* `hw2.py`, `hw2.txt`, `hw2.txt.nlp`, your report in `pdf`.