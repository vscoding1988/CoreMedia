
There are multiple ways of creating templates for CoreMedia. The most proffered way is to create a new theme below `/frontend/themes`. CoreMedia has a `pnpm` task for creating a new theme.

```bash
# Executed in project folder
cd frontend

# First install all dependencies
pnpm install

# Create new empty theme `tutorial`, the command will ask some questions 
# - we don't want to derive the theme from other themes -> N
# - we don't need any plugins -> click ENTER
# - we don't want to have them as dependencies -> N
pnpm create-theme tutorial
pnpm install
```

> It is up to you, if you want to include CoreMedia bricks for the tutorial we don't need them

Below `/frontend/themes` a new folder was created `tutorial-theme` most of the folders are self explanatory and others will be explained in the following tutorials. For now let's deploy the new theme into CoreMedia. 

```bash
cd themes\tutorial-theme

pnpm run deploy
```

>The first time you will be asked to log in, you can let Proxy Url empty and use the user that was created in #TODO

In studio the folder `/All Content/Themes/tutorial` was created the theme can now be attached to the homepage that was created in #TODO 

---
#version/2207_1 #CM_11