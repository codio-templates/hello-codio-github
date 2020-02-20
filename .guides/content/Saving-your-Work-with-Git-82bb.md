Git allows you to save multiple versions of your work. The basic things you want to do are just a few commands in the terminal. You can open the terminal by selecting **Tools->Terminal**.
![.guides/img/terminal](.guides/img/terminal.png)

## Saving your work (aka "Committing" and "Pushing")
1. **Type `git add .` and press Enter/Return**
    This command tells git to go collect all the changes you have made since your last save (which is called "commit" in Git).
1. **Type `git commit -m "commit message"` and press Enter/Return**
    This command bundles all your changes and gives them a useful human-readable name -- so make sure you fill in something useful where is says `commit message`!
1. **Type `git push` and press Enter/Return**
    This command sends this bundle of changes to GitHub so you have a copy in the cloud.
    
## Going back to immediately previous save point (aka Reverting to previous commit)
To get rid of all changes since you last "saved" or "committed", follow these steps. Be careful, you cannot undo this!

1. First, check what your last "commit" or "save" was to make sure you know where you are going back to. You can either look on GitHub or type `git log`. If you have a lot of commits, you will need to type ctrl+c to exit git log.
1. `git add . && git reset --hard HEAD`
