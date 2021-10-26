# specialRepo

Assignment Instructions
In pairs, create the following scenarios and explore how to resolve them. Answer any questions in the README.md file of your remote repository (and look up the markdown cheatsheet for formatting to make it nice).
Paste the url for your remote repository in this assignment (both partners must do this).
 
Q1 - What does clone set the variable origin to represent?
Git creates a remote called origin and then it points to it
Q2 - What does the command git push --set-upstream origin master do? What does remote tracking mean in this context?
When you set the “upstream” branches or tracking branches you can pull or push without having to specify the target 
Remote tracking is local references for remote branches.
Research and then execute the following command: git pull origin master
Q3 - Explain and illustrate what's happening in the commit tree when this command executes.
The special branch has features pulled from the main branch then the special branch merges with the main branch after the feature.
Q4 - Are your commits overwritten by the remote master?
You have to merge commit all of your changes the git pull overwrites the commits.
Q5 - Is this a merge or a rebase?
A merge because the special branch is separate from the main branch and is then merged with the main branch after the feature
Q6 - Person B: checkout the local master branch. Is it updated as well, or still behind remote master?
Yes the main branch is up to date 
Q7 - Run git branch. Did your local copy of your branch delete when Person A deleted the remote branch?
No Person B still has the local copy of the branch (WillSpecialBranch)
Q8 - Use git log --graph --all to view the branching structure and copy and paste the result into the README.md formatted as a code segment (see markdown cheatsheet).
Person A
*   commit bffebc1a68f7c3ccb241053bbe12bbf8e698cc19 (HEAD -> main, origin/main, origin/HEAD)
|\  Merge: 74979ef c735335
| | Author: Trent Blair <58864613+tblair22@users.noreply.github.com>
| | Date:   Tue Oct 26 12:27:24 2021 -0600
| | 
| |     Merge pull request #2 from tblair22/Feature2
| |     
| |     I added the edited text file lets gooooooooo
| |   
| *   commit c735335c65147dea285c9721eff48d664bb7e71b (origin/Feature2, Feature2)
| |\  Merge: cb52937 74979ef
| |/  Author: Trent Blair <58864613+tblair22@users.noreply.github.com>
|/|   Date:   Tue Oct 26 12:21:34 2021 -0600
| |   
| |       Merge branch 'main' into Feature2
| | 
* | commit 74979efafe76fa1bc01356e04b6cc177f2dfc5b2
| | Author: William Writer <williamwriter@Williams-MacBook-Pro-2.local>
| | Date:   Tue Oct 26 12:12:06 2021 -0600
| | 
| |     Edited testtext so that there is a merge conflict?
:

Person B

​​*   commit bffebc1a68f7c3ccb241053bbe12bbf8e698cc19 (HEAD -> main, origin/main, origin/HEAD)
|\  Merge: 74979ef c735335
| | Author: Trent Blair <58864613+tblair22@users.noreply.github.com>
| | Date:   Tue Oct 26 12:27:24 2021 -0600
| | 
| |     Merge pull request #2 from tblair22/Feature2
| |     
| |     I added the edited text file lets gooooooooo
| |   
| *   commit c735335c65147dea285c9721eff48d664bb7e71b (origin/Feature2)
| |\  Merge: cb52937 74979ef
| |/  Author: Trent Blair <58864613+tblair22@users.noreply.github.com>
|/|   Date:   Tue Oct 26 12:21:34 2021 -0600
| |   
| |       Merge branch 'main' into Feature2
| | 
* | commit 74979efafe76fa1bc01356e04b6cc177f2dfc5b2
| | Author: William Writer <williamwriter@Williams-MacBook-Pro-2.local>
| | Date:   Tue Oct 26 12:12:06 2021 -0600
| | 
| |     Edited testtext so that there is a merge conflict?
| | 
| * commit cb529378276b281ae7eee5c5ebb04e9e5f3eba66
|/  Author: Trent Blair <tblair22@kentdenver.org>
|   Date:   Tue Oct 26 12:07:32 2021 -0600
|   
|       I added the edited text file
|   
*   commit ba75bdbbfac1562a26513754292dd3e1f2aec65e
|\  Merge: e5a9f2e baa3b56
| | Author: Trent Blair <58864613+tblair22@users.noreply.github.com>
| | Date:   Tue Oct 26 12:00:47 2021 -0600
| | 
| |     Merge pull request #1 from tblair22/WillSpecialBranch
| |     
| |     I updated the Willtext file like a total boss
| | 
| * commit baa3b56a660c3108682ae653ee8ff8940af14fd5 (origin/WillSpecialBranch, WillSpecialBranch)
|/  Author: William Writer <williamwriter@Williams-MacBook-Pro-2.local>
|   Date:   Tue Oct 26 11:56:17 2021 -0600
|   
|       I updated the Willtext file
| 
* commit e5a9f2ec5e05389670795656d2fc0a8f07aa10e7
| Author: William Writer <williamwriter@Williams-MacBook-Pro-2.local>
| Date:   Wed Oct 20 14:17:09 2021 -0600
| 
|     Commit of Will's Special Branch merging into the Main branch
|   
*   commit f5e1d3fa25fb3d5c8354297d3a5855e47ffbd512
|\  Merge: 2e799b3 ce91d2a
| | Author: William Writer <williamwriter@Williams-MacBook-Pro-2.local>
| | Date:   Wed Oct 20 14:13:37 2021 -0600
| | 
| |     commit of Will's Special Branch
:


