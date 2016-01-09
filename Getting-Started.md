## Python 2.7

* Download and install the latest version of [Python 2.7.x](https://www.python.org/downloads/release/python-2711/).
* Open a terminal and enter the following command: `python --version`.
* If it prompts `Python 2.7.x`, Python is successfully installed on your machine.

## PyCharm

* Download and install the community version of [PyCharm](https://www.jetbrains.com/pycharm/download/).
* Launch PyCharm.
* Create a project by choosing `File -> New Project`.
 * Create the directory location `cs329`.
 * Make sure to choose an interpreter whose version is 2.7.x.
* Create a file `hello.py` by choosing `File -> New -> Python File`.
* Copy and paste the following code to `hello.py`.
```python
# while loop
s = 0
i = 0
while i < 10:
    s += i
    i += 1
print s,

# for loop using range
s = 0
for i in range(0,10):
    s += i
print s,

# sum using range
print sum(range(10))
```
* Run the code by choosing `Run -> Run 'hello'`.
* If you see `45 45 45` on the console, your program is successfully run.

## Quiz

* Login to `lab0z.mathcs.emory.edu`.
* Create a directory `quiz0` under the `cs329` directory.
* Put `hello.py` under `cs329/quiz0`.
* If you are using a Windows machine with no 3rd-party shell:
 * Use an FTP client (e.g., [FileZilla](https://filezilla-project.org)) to upload your file.
* If you are using a Mac/Linux machine:
 * Run the following command by replacing `yourID` with your `mathcs ID` (e.g., `choi`).
```
rsync -avc hello.py yourID@lab0z.mathcs.emory.edu:~yourID/cs329/quiz0/
```