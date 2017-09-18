# 001-HTML-learning
HTML learning notes


GIT BASH configuration:

1.github
    1) check for existing SSH keys
        $ cd C:\Users\Herman
        $ ls -al ~/.ssh
    2) Generating a new SSH key
        $ ssh-keygen -t rsa -b 4096 -C "useremail"
        Enter
        type a secure passphrase
    3) Adding a new SSH key to your GitHub account
        $ clip < ~/.ssh/id_rsa.pub
        github -> SSH and GPG keys
        Completed

2.git-bash
    $ git config --global user.name "username"
    $ git config --global user.email "useremail"