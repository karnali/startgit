# GitHub Instructions!

Create a new repository on GitHub.com. To avoid errors, do not initialize the new repository with README, license, or gitignore files. You can add these files after your project has been pushed to GitHub.

Open Terminal Change the current working directory to your local project. config-globals. Set the username and email address for your Git commits. Replace [EMAIL_ADDRESS] with your Git email address. Replace [USERNAME] with your Git username.

#  git config --global
```
$ git config --global user.name "First Last"
$ git config --global user.email "email@domain.com"
```

# Generate rsa key locally.
```
$ ssh-keygen -t rsa
$ cat ~/.ssh/id_rsa.pub 
```
Copy .pub key and go to github and create SSH keys under settings.


# cd to your local git project folder.
```
$ git init
$ git add .
$ git commit -m ". means include all files inside dotfiles folder"
$ git status

$ Push an existing repository from the command line
$ git remote add origin git@github.com:karnali/dotfiles.git
$ git push -u origin master
```



# You can't push to git://github.com/karnali/dotfiles.git

```
$ git remote rm origin
$ git remote add origin git@github.com:karnali/dotfiles.git
$ git push -u origin master
```

# If git pull from github fails
```
$ git reset --hard
$ git pull
```
