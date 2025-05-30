## Python Basics

### 0. Learn Python basics on [Codecademy](https://www.codecademy.com/learn/learn-python) (free version), [w3schools](https://www.w3schools.com/python/), and the [tutorial from the textbook](http://www.cse.msu.edu/~ptan/dmbook/tutorials/tutorial1/tutorial1.html)
 - Skip this step if you already know how to code in Python.
 - If you are seeking for more practices, [https://www.w3resource.com/python-exercises/](https://www.w3resource.com/python-exercises/) has plenty of exercises.

### 1. Install Python on your local machine.

 - Install [conda](https://docs.conda.io/en/latest/miniconda.html) with Python 3.8+.

### 2. Install required packages.
 - Open terminal.
 ```
 conda install scikit-learn
 conda install pandas
 ```

### 3. (Optional) Install an IDE.
 - [Pycharm](https://www.jetbrains.com/pycharm/) community version.


## Github Basics

### 0. Install [Git](https://git-scm.com/downloads) and create your [Github](https://github.com/) account.
 - Skip this step if you already have one.

### 1. Create a new PRIVATE repository called **DSCI-633** under your Github account.
 - (1) Click on the **new** button:
 ![](../img/create_repo.png?raw=yes)

 - (2) Initiate the new private repo:
 ![](../img/init_repo.png?raw=yes)

 - (3) Invite the instructor as collaborators (ezgisiir):
 ![](../img/invite.png?raw=yes)

### 2. Clone the **fds** repo to your local machine.
 ```
 git clone https://github.com/ezgisiir/fds
 ```

### 3. Save username and token in git.
 - Create your personal access token on [this page](https://github.com/settings/tokens)
 - Copy the generated token.
 - In terminal:
 ```
 git config --global credential.helper manager
 ```
 - When running this command, the first time you pull or push from the remote repository, you'll get asked about the username and your token (NOT Password!). Afterwards, for consequent communications with the remote repository you don't have to provide the username and password.

### 4. Working with a github repo.
 - (1) Go to the local directory of the **DSCI-633** repo.
 - (2) Pull from Github so that the content on your local machine is updated with the remote server of Github:
 ```
 DSCI-633> git pull
 ```
 - (3) Work on your local machine (add/remove/edit files under DSCI-633/).
 - (4) Commit to the remote server of Github (upload local changes).
 ```
 DSCI-633> git add .
 DSCI-633> git commit -m "YOUR COMMIT MESSAGE"
 DSCI-633> git push
 ```

 ### 5. Add your information to [[Google sheet][(https://docs.google.com/spreadsheets/d/10jPUZnoEc3B73vq_c727di-N0Vrq2vE7s0r-jp7Ckn0/edit?usp=sharing)]
 - Add your github repo link (along with your RIT username and Github username) to the Google sheet.
