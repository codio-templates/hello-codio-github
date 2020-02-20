---------
Each Codio box (Assignment, Book, or Project) can be mapped to a GitHub repo. This connection only needs to be established once per box.

## In GitHub: Make a New Repo 

<details><summary>**Wait! I have an existing repo I want to clone**</summary>You can import a project from a GitHub repo [docs page here](https://codio.com/docs/project/creating/) and this connection is made during the importing process. If you are familiar with Git, skip the rest of this guide and just use the terminal as usual  by going to `Tools > Terminal`. </details>

1. Go to your GitHub organization (or profile) and click the green **New** repository button
![.guides/img/NewRepo](.guides/img/NewRepo.png)

1. Fill out the requested details. We suggest **not** initializing a README since one already exists in Codio and will result in an immediate conflict.
![.guides/img/RepoConfig](.guides/img/RepoConfig.png)

1. Copy either the **HTTP** or **SSH** URL on the created repo page. (If you do not want to type credentials and you uploaded your public key, use SSH).
![.guides/img/RepoURL](.guides/img/RepoURL.png)


## In Codio: Connect to Repo
<details><summary>**Just give me a terminal!**</summary> You can skip the rest of this guide and do your normal Git workflow via command line if you prefer. Open terminal by selecting **Tools->Terminal**</details>



1. On the top tool bar of the Codio Box you want to connect, select from the menu **Tools->Git->Remotes...**
![.guides/img/RemoteMenu](.guides/img/RemoteMenu.png)
1. When prompted, initialize a local git repository by clicking **YES**
![.guides/img/gitInit](.guides/img/gitInit.png)
1. When prompted, click **Add Remote**
![.guides/img/RemoteConfig](.guides/img/RemoteConfig.png)
1. Fill in `origin` as the name (this is a git standard) and paste the URL you copied into the second box. Press **Save** and **Close**
![.guides/img/RemoteConfig2](.guides/img/RemoteConfig2.png)
1. Open the terminal by selecting **Tools->Terminal**
![.guides/img/terminal](.guides/img/terminal.png)
1. Type `git add .` and press Enter/Return
1. Type `git commit -m "initial commit"` and press Enter/Return
1. Type `git push --set-upstream origin master` and press Enter/Return

If you are new to Git and want to know just enough to save your work, continue to the next page.

### Collaboration in Codio with GitHub
If you share Codio boxes with other members of your GitHub repository (directly through **Project->Permissions** or a copy through **Project->Fork**), this connection to GitHub is maintained. They will have to have their GitHub and Codio accounts linked for this to work (as described on the previous page).