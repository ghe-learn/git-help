# git-help

A list of issues encountered when working with git.

# Error: Failed to push some refs to

![](img/integrate-remote-before-pushing-01.png)

## Translation

| type  | text                                                                                        | translate                                                                                                                                     |
|-------|---------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|
| error | failed to push some refs to ‘https://github.com/…’                                          | I could not push the changes that you have committed to GitHub.                                                                               |
| hint  | the remote contains work that you do not have locally                                       | There is work in the repo on GitHub (the remote) that you do not have in the location that you work with R (e.g. your laptop, RStudio Cloud). |
| hint  | this is usually caused by another repository pushing to the same ref                        | Someone else (including you on another computer) is working on this repo and has pushed some changes to it.                                   |
| hint  | you may first want to integate the remote changes (e.g. ’ git pull …’) before pushing again | Pull, then push again.                                                                                                                        |

## Solution

**Pull.** If the work that you pull from GitHub does not overlap with
something you have worked on locally (on your computer or RStudio
Cloud), then this will be the solution. If you have had changes locally
that overlap with the pulled changes on GitHub, you will receive another
error message (to be written up).

![](img/integrate-remote-before-pushing-02.png)

**Push**. And keep on working with the next commit.

![](img/integrate-remote-before-pushing-03.png)
