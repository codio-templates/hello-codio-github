---------
Each Codio box (Assignment, Book, or Project) can be mapped to a GitHub repo. This connection only needs to be established once per box.

## In GitHub: Make a New Repo 

<details><summary><b>Wait! I have an existing repo I want to clone</b></summary>You can import a project from a GitHub repo [docs page here](https://docs.codio.com/project/projects/#creating-and-importing-a-project) and this connection is made during the importing process. If you are familiar with Git, skip the rest of this guide and just use the terminal as usual  by going to <code>Tools > Terminal</code>. </details>

1. Go to your GitHub organization (or profile) and click the green <b>New</b> repository button
![.guides/img/NewRepo](.guides/img/NewRepo.png)

1. Fill out the requested details. We suggest <b>not</b> initializing a README since one already exists in Codio and will result in an immediate conflict.
![.guides/img/RepoConfig](.guides/img/RepoConfig.png)

1. Copy either the <b>HTTP</b> or <b>SSH</b> URL on the created repo page. (If you do not want to type credentials and you uploaded your public key, use SSH).
![.guides/img/RepoURL](.guides/img/RepoURL.png)


## In Codio: Connect to Repo
<details><summary><b>Just give me a terminal!</b></summary> You can skip the rest of this guide and do your normal Git workflow via command line if you prefer. Open terminal by selecting <b>Tools->Terminal</b></details>



1. On the top tool bar of the Codio Box you want to connect, select from the menu <b>Tools->Git->Remotes...</b>
![.guides/img/RemoteMenu](.guides/img/RemoteMenu.png)
1. When prompted, initialize a local git repository by clicking <b>YES</b>
![.guides/img/gitInit](.guides/img/gitInit.png)
1. When prompted, click <b>Add Remote</b>
![.guides/img/RemoteConfig](.guides/img/RemoteConfig.png)
1. Fill in <code>origin</code> as the name (this is a git standard) and paste the URL you copied into the second box. Press <b>Save</b> and <b>Close</b>
![.guides/img/RemoteConfig2](.guides/img/RemoteConfig2.png)
1. Open the terminal by selecting <b>Tools->Terminal</b>
![.guides/img/terminal](.guides/img/terminal.png)
1. Type <code>git add .</code> and press Enter/Return
1. Type <code>git commit -m "initial commit"</code> and press Enter/Return
1. Type <code>git push --set-upstream origin master</code> and press Enter/Return

If you are new to Git and want to know just enough to save your work, continue to the next page.

### Collaboration in Codio with GitHub
If you share Codio boxes with other members of your GitHub repository (directly through <b>Project->Permissions</b> or a copy through <b>Project->Fork</b>), this connection to GitHub is maintained. They will have to have their GitHub and Codio accounts linked for this to work (as described on the previous page).