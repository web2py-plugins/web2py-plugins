# web2py-plugins
Web2py plugins - unofficial repository

## How to install plugins
Web2py plugins are historically published on http://www.web2pyslices.com and this is integrated with Web2py admin interface (application Edit, Download plugins from repository). However there were some problems with maintenance and use of web2pyslices.com and that led to not very useful plugins list on that site.

If you found Web2py plugin on other place, like in this github repository, you can **download it** and **install in Web2py admin interface**: **application Edit, Upload plugin**.

## How is the web2py-plugins account and this repository (web2py-plugins/web2py-plugins) organized
web2py-plugins/web2py-plugins is main repository for packed plugins (.w2p). In addition we create repositories for source code of plugins if author wishes use such repositories for the source code.

In this repo in **root** directory we have plugins with some known maintenance and documentation. In **found/** directory we have everything found on the internet without much knowledge about author, download page, functionality, .. So please google for more info, documentation and newer versions about such plugins.

## Published plugins

- ``plugin_CKEDITOR``, v1.2 (ckeditor 4.5.7 Feb 2016), https://github.com/timrichardson/web2py_ckeditor4
- ``plugin_MANAGE_GROUPS``, v1.0, https://github.com/web2py-plugins/plugin_manage_groups

### found/

- ``plugin_wiki`` is sure OBSOLETE, use controller with: return auth.wiki()

## Help improve this page
Send **pull request** with plugin made by you or with missing found/ plugin. If you are the author and if you add the plugin into root directory, we will create a repository for plugin sources and create access rights for you.

### How to prepare pull requests (this is standard github usage)
If you have access rights to repository (if you have uploaded your own plugin and we have created a plugin repository and have given access rights to you) you can simply clone the repository and commit/push.
However to update web2py-plugins/web2py-plugins repository (to add new plugin) or to improve some published code in other repositories, do following:
- fork the repository - this will create a copy in your github account, where you will have read/write access,
- clone your github fork to your (local) developers machine: git clone ...
- our repository is called **upstream**, your fork is called **origin**
- change local configuration: ``git remote add upstream git://github.com/web2py-plugins/''upstream_repository''.git``
- before you go to change code be sure you are in master branch ``git checkout master`` and update your local repository: ``git pull upstream master``
- see ``git status`` and if you are "ahead" with commits before your ``origin`` fork (i.e. ) then apply ``git push``
- [it could be good but not necessary create a branch: ``git branch mychanges``, ``git checkout novavlastnost``]
- make changes, ``git commit``, ``git push`` (in case of extra branch this will show you the required syntax to push into new branch)
- at ``github.com/youraccount/fork-origin`` create the pull request
