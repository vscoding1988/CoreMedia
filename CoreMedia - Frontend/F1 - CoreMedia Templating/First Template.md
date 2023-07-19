## Introduction

The folder `/frontend/themes/tutorial-theme/templates` will contain all templates of the theme and although the folder is empty, the channel ( add URL #TODO ) is still rendering a HTML page, this happens because not all templates are part of the themes folder, some are created directly in workspace, in the case of `Page.ftl` you can find the template in `cae-base-lib` module. There is a template priority system, that will be covered later.

## Page.ftl

The theme creation task[^1] has created not only the `templates` folder but also the folder `com.coremedia.blueprint.common.contentbeans` here create a new folder `Page.ftl` with content. 

```html
<!DOCTYPE html>
<html lang="en" dir="ltr">
<head>
    <meta charset="UTF-8">
    <title>Hello world</title>
</head>
<body>
	<h1>Hello World</h1>
</body>
</html>
```

Deploy the theme and have a look on the new start page, now that there is a `Page.ftl` in the themes, it is rendered.


---
[^1]:  [[Setup Workspace for templating]]

#version/2207_1 #CM_11