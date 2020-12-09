Git allows you to save multiple versions of your work. The basic things you want to do are just a few commands in the terminal. You can open the terminal by selecting <b>Tools->Terminal</b>.
![.guides/img/terminal](.guides/img/terminal.png)

## Saving your work (aka "Committing" and "Pushing")
1. <b>Type <code>git add .</code> and press Enter/Return</b>
    This command tells git to go collect all the changes you have made since your last save (which is called "commit" in Git).
1. <b>Type <code>git commit -m "commit message"</code> and press Enter/Return</b>
    This command bundles all your changes and gives them a useful human-readable name -- so make sure you fill in something useful where is says <code>commit message</code>!
1. <b>Type <code>git push</code> and press Enter/Return</b>
    This command sends this bundle of changes to GitHub so you have a copy in the cloud.
    
## Going back to immediately previous save point (aka Reverting to previous commit)
To get rid of all changes since you last "saved" or "committed", follow these steps. Be careful, you cannot undo this!

1. First, check what your last "commit" or "save" was to make sure you know where you are going back to. You can either look on GitHub or type <code>git log</code>. If you have a lot of commits, you will need to type ctrl+c to exit git log.
1. <code>git add . && git reset --hard HEAD</code>
