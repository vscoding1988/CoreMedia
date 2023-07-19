
## Ubuntu

### Installation

```bash
# First check if git is not already installed
git --version

# If it is not installed execute, else skip
sudo apt update
sudo apt install git

# Check again
git --version

# Set config
git config --global user.name "yourname"
git config --global user.email "your@email.com"
```

## Windows

#TODO 

## Setup credentials

### Setup SSH key

```bash
# Linux
ssh-keygen -C "your@email" -t rsa
cd ~/.ssh
cat id_rsa.pub

# Windows 

```  
#TODO

Go to you Github account -> Settings → SSH and GPG keys → New SSH Key paste the content of the .pub file into in the text box and click on "Add SSH Key".

> If you use the SSH method, make sure to clone SSH urls

### Setup Personal Access Token

To generate a personal access token go to your Github account -> Settings -> Developer Settings (last option) -> Personal Access Token -> Tokens classics -> Generate new token -> select checkbox "repo".

You should get a token looking like this `ghp_yjmXXXXX` and store it somewhere. Whenever you execute pull/push command you will be asked to provide credentials. 

```bash
# There is a way to store the crednetials using the command below, but this will # store the credentials as plain text
git config --global credential.helper store

# There is a way to make it a little bit more secure by using a cache command so
# that the credentials are only persisted for given timeframe in seconds 
# (900s = 15m), but still a better way is to use ssh key

git config credential.helper 'cache --timeout=900'
```

## Clone CoreMedia repository

Now you can clone the CoreMedia repository from companies git server, or download from official CoreMedia [Github Acoount](https://github.com/CoreMedia)(you need to request access to CoreMedia repository through their support portal).


---
#version/2207_1 #CM_11