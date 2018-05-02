# 001-HTML-learning
## GIT BASH configuration:

1.github

(1) check for existing SSH keys

```
$ cd C:\Users\Herman
$ ls -al ~/.ssh
```

(2) Generating a new SSH key

```
$ ssh-keygen -t rsa -b 4096 -C "useremail"
```
Enter, and type a secure passphrase

(3) Adding a new SSH key to your GitHub account

```
$ clip < ~/.ssh/id_rsa.pub
```
github -> SSH and GPG keys, Completed

2.git-bash

```
$ git config --global user.name "username"
$ git config --global user.email "useremail"
```

add sth else for testing3

3.VS Code push issue:

(1) open folders by using "code ." in git bash
> Q: Can I use SSH Git authentication with VS Code?

> A: Yes, though VS Code works most easily with SSH keys without a passphrase. If you have a SSH key with a passphrase, you'll need to launch VS Code from a Git Bash prompt to inherit its SSH environment.

(2) Avoid git authentication dialog

> Q: I keep getting Git authentication dialogs whenever VS Code is running.

> A: VS Code automatically fetches changes from the server in order to present you with a summary of incoming changes. The Git authentication dialog is independent from VS Code itself and is a part of your current Git credential helper.
One way to avoid these prompts is to set up a credential helper which remembers your credentials. Another option is to disable the auto fetch feature by changing the following setting: "git.autofetch": false.
```
git config --global credential.helper wincred
```