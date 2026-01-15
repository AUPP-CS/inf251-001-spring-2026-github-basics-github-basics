[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/6PkNYzZ5)
# Github Basics
This guide will provide a step-by-step instructions to setup your github account on your computer, and the basics on how to clone and commit the code.



### I. Setting up SSH key
#### 1. Generate SSH key
`ssh-keygen -t ed25519 -C "your_email@aupp.edu.kh"`

This creates:
~/.ssh/id_ed25519 (private key)
~/.ssh/id_ed25519.pub (public key)

#### 2. Open and copy your SSH key
Mac: `cat ~/.ssh/id_ed25519.pub | pbcopy`

Windows: `cat ~/.ssh/id_ed25519.pub | clip`


You can also simply open the key and using Ctrl/Cmd+C to copy the key:
`cat ~/.ssh/id_ed25519_new_account.pub`
The cat command will open and display the public key.

#### 3. Copy your SSH key to github
- Open Github
- Login to your github account (using the email from the SSH key creation earlier)
- Go to Settings -> SSH and GPG keys -> New SSH Key
![ssh-key-guide](./ssh_key_guide.png)
*You can use any title you want (to identify your computer). If you change computer, you will have to set this up all over again.*
- Add SSH key

Now you can clone the github repo, commit the code using your github account with the email earlier.



### II. Clone the repository
1. From the github repository, copy the ssh url.
![copy-ssh](./clone_ssh.png)
2. Go to your prefered folder in your computer.
3. Open Terminal from there.
4. Clone the repository using the ssh url: `git clone git@github.com:mbuntoun/github-basics.git`



### III. Make changes to the repository via VS Code
1. Open the folder in VS Code.
2. Add about_me.txt
3. In about_me.txt, write your name, and a few words to describe yourself.
After making the changes, you will see the changes highlight in VS Code. Then, you can commit the code to github.



### IV. Commit to Github
1. Add your changes: In your terminal `git add .`
2. Commit your changes: `git commit -m "your commit message here"`
3. Push to Github: `git push`
Now you can see the changes in the github repository.



### V. Others
For working with a team, you may want to pull the latest changes first before you add and commit any code:
`git pull`

You can also check the status first before you pull using: `git status`
