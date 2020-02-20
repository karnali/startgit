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



# You can't push to github

```
$ git remote rm origin
$ git remote add origin git@github.com:karnali/dotfiles.git
$ git push -u origin master
```

# You can't pull to github
```
$ git reset --hard
$ git pull
```

# Local and remote git cleanup

Remove git tracking from a project.
```
$ cd /Users/jsmith/Desktop/github/dotfiles
$ rm -rf .git
```
Recreate the repos from the current content only ex. /Users/jsmith/dotfiles
```
$ git init
$ git add .
$ git commit -m "Initial commit"
```

Push to the github remote repos ensuring you overwrite everything in it
```
$  git remote add origin git@github.com:karnali/dotfiles.git
$  git push -u --force origin master
```

