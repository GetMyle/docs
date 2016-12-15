---
title: Development environment
category: Quickstart
order: 12
---

Here is how IDE looks like:

![](https://raw.githubusercontent.com/wiki/GetMyle/Guides/MyletDevGuide/myletprojectstructure.png)

IDE is split into three main parts:
 - main toolbar:
    - `Build & Run` - builds and opens mylet in new window
    - `Run Last Build` - runs last mylet build in new window
    - `Db` - opens up [database tools](#tools)
    - `Publish` - builds and publishes current mylet version to market
    - `Git (on branch)` - shows [source control](#collaboration-and-source-control) options
    - `View Output` - shows last output from hook or controller during mylet execution during development
 - navigation pane on left hand side
 - content pane on right hand side that shows content of an active item in navigation pane and has own toolbar depending on the item:
	- `Edit` - when in document view mode, switch to document editing mode
	- `Rename` - renames current document or folder name
	- `Delete` - deletes current document or folder
	- `Done` - when in editing mode, switches back to view mode
	- `Save` - when in editing mode, saves current document
	- `Install package` - when viewing [`bower.json`](#managing-front-end-dependencies) or [`package.json`](#managing-back-end-dependencies) is used to install a dependency
	- `Add file` - when in folder mode, allows to create empty document or upload another one
	- `Add folder` - when in folder mode, creates sub-folder


### Mylet files

Let's walk through project files of default mylet template:
 - `api/controller.js` - entry point for [mylet controller](#controller) - nodejs code that is executed when specific mylet URL is requested
 - `api/hook.js` - entry point for [mylet hook](#hook)  - nodejs code that is executed when new record appears
 - `views/index.js` - entry point for UI JavaScript
 - `views/index.ejs` - mylet HTML page; currently [EJS](http://www.embeddedjs.com/) templates are used
 - `views/layout.ejs` - layout [EJS](http://www.embeddedjs.com/) template page.
 - `views/index.css` - UI CSS styles
 - `icon.jpg` - mylet icon; see [Mylet configuration](#mylet-configuration) for how to change icon file name
 - `bower.json` - [bower](http://bower.io/) configuration file; see [Managing client side dependencies](#managing-front-end-dependencies)
 - `mylet.dev.json` - development only [mylet configuration file]((#mylet-configuration)
 - `mylet.json` - [mylet configuration file](#mylet-configuration)
 - `package.json` - [npm](https://www.npmjs.com/) configuration file; see [Managing server side dependencies](#managing-back-end-dependencies)
