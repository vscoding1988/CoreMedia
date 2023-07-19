
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
```



## Windows

#TODO 

## Setup credentials

To generate a personal access token go to your Github account -> Settings -> Developer Settings (last option) -> Personal Access Token -> Tokens classics -> Generate new token -> select checkbox "repo" 

You should get a token looking like this `ghp_yjmXXXXX` and store it somewhere.

```bash
git config --global user.name "yourname"
git config --global user.email "your@email.com"
```

When pulling for the first time, you will asked to log in, use your user and the generated token instead of password.

## Clone CoreMedia repository

Now you can clone the CoreMedia repository from companies git server, or download from official CoreMedia [Github Acoount](https://github.com/CoreMedia)(you need to request access to CoreMedia repository through their support portal).


---
#version/2207_1 #CM_11