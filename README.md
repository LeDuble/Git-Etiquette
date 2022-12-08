<!-- TITLE -->
<h1 align="center">
<a id="title" href="#title" aria-hidden="true"></a>
Git Etiquette and Cheat Sheet
</h1>

<p align="center">This Git Etiquette and Cheat Sheet is made for The Software Developer Team of DigiTalents Helsinki.</p>

<!-- TABLE OF CONTENTS -->
<h2>
<a href="table-of-contents" aria-hidden="true"></a>
Table of Contents
</h2>
<ol>
<li><a href="#descr">Introduction</a></li>
<li><a href="#one">Bedrock Rules</a></li>
<li><a href="#two">Formatting Rules</a></li>
<li><a href="#three">How to Create a Branch (via Git)</a></li>
<li><a href="#four">Merging Branches</a></li>
<li><a href="#five">Deleting Branches Locally & Remotely</a></li>
<li><a href="#six">.gitignore</a></li>
<li><a href="#seven">Adding .gitignore into already existing repository</a></li>
<li><a href="#eight">Cheat Sheet</a></li>
<li><a href="#nine">Authors</a></li>
<li><a href="#ten">How to Contribute</a></li>
<li><a href="#eleven">License</a></li>
<li><a href="#twelve">Future Updates</a></li>
</ol>

---

<!-- INTRODUCTION -->
<h2>
<a id="descr" href="#descr" aria-hidden="true"></a>
Introduction
</h2>

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-success)](http://makeapullrequest.com)
[![License](https://img.shields.io/badge/license-CC%20BY--SA%204.0-blue)](https://creativecommons.org/licenses/by-sa/4.0/)

The essence of the Git Etiquette Cheat sheet is to provide standardized workflow frame and foundation for the team. 

By charishing unified workflow means that it is easier to review and track the current history of the project. People will come and go so it's very vital to maintain excellent etiquette. As this allows anyone to join, any time, figure out the process and track the status of the project with ease.

Background story for the Etiquette:
I started Git Etiquette Cheat Sheet as my personal project for personal use to create unified and coherent workflow. The main purpose of this was so that others could interpret easier what I'm working with and navigate history effortlessly.

Team leader (Joonas) heard about it and asked if I could make it for the whole team.

(<a href="#table-of-contents">back to top</a>)

---

<!-- BEDROCK RULES -->
<h2>
<a id="one" href="#one" aria-hidden="true"></a>
Bedrock Rules
</h2>

1. **Pull frequently**
2. **Push infrequently**  
3. **Commit frequently**    
   * Merge "forward frequently"
      * Note: Make sure that your branch doesn’t diverge too much from the original branch 
4. **Create pull requests infrequently**
   * Productivity is not measured by PRs!
   * If your code affects others, then make a pull request. So that others who are working on the same project gets the latest feature. 
      * In other hand if it doesn't affect others, then do not make unecessary pull requests for minor things.
      * Key sentence: Quality Over Quantity 
5. **Always ask if unsure**

(<a href="#table-of-contents">back to top</a>)

---

<!-- FORMATTING RULES -->
<h2>
<a id="two" href="#two" aria-hidden="true"></a>
Formatting Rules for a Branch (Type/Reference ID/Description)
</h2>

### 1. Type
   * **Docs** - Changes to documentation only
   * **Feat** - A new feature
   * **Style** - Changes to formatting (e.g. the code is missing semicolons).
   * **Test** - Adding/correcting existing tests.
   * **Refactor** - A code change which isn't bug fix or adds a feature. It's restructure of the code without changing the functionality.
   * **BugFix** - A bug fix.
   * **Chore** - Maintenance or change to auxiliary tools.
   * **Add** - Adding essentials to the repository (e.g. .gitignore or example files).

### 2. Reference ID
   Reference the issue from GitHub, Trello or some other agile source. 
   For now use one of the two formats shown below.
   * Referencing an issue from Github: **__issue(_insert number here_)__** or just **__number__** (e.g. **_/issue12/_** or **_/12/_**)
   * Referencing from Trello: **__trello(_insert number here_)__** (e.g **_/trello8/_**) 

### 3. Description
   Short Description that is 1-3 words long and separated by hyphens aka " - ". 
   Briefly describes what is done or worked on.

### Examples


Good Examples :+1: | Bad Examples :-1:
------------ | -------------
:heavy_check_mark: `add/issue12/gitignore` | :x: `something/bug12/do_S*ame<`
:heavy_check_mark: `style/8/added-missing-semicolons` | :x: `hi/TeSt/ääliö`
:heavy_check_mark: `fix/trello1/serializer` | :x: `fiX/TreLlo1/SeRiAlIzeR`

**Note:**
Only use allowed special characters which are " / " and " - " when formatting the branch!

(<a href="#table-of-contents">back to top</a>)

---

<!-- CREATE A BRANCH -->
<h2>
<a id="three" href="#three" aria-hidden="true"></a>
How to Create a Branch (via Git)
</h2>

* **__`git branch -a`__**
   * see all available branches in this repository/project.
* **__`git checkout -b <insertBranchNameHere>`__**
   * create a new branch ("__-b__" creates and switches to it).
* **__`git switch <insertBranchNameHere>`__**
   * switch between branches.

### adding it to working branch (not master)
* **__`git add –i`__**
   * Opens interactive menu and it is used to update index using the current content.
* **__`git status`__**
   * Shows which files are tracked by Git and which changes have been staged (which have been not).
* **__`git restore --staged <insertFileNameToUnstage>`__**
   * Note: Incase you added something you don't want to push.
* **__`git commit -m "<insertCommentsHere>"`__**
   * Record changes to the repository
* **__`git push --set-upstream origin <insertBranchNameHere>`__** 
   * (You can do alias for this)

(<a href="#table-of-contents">back to top</a>)

---

<!-- MERGING BRANCHES -->
<h2>
<a id="four" href="#four" aria-hidden="true"></a>
Merging Branches
</h2>

Very important: when merging, make sure that you are on the branch that you want to merge to. You will tell Git basically: "see those new stuff? Bring them over here."
1. **__`git add -i`__**
2. **__`git commit -m "<insertCommentsHere>"`__**
3. **__`git checkout master`__**
4. **__`git merge <insertBranchNameHere> --no-ff`__**
   * Additional command "**_--no-ff_**" tells Git that you want to retail all of the comments prior to the merge. Makes tracking easier in the future.

Always consult before merging directly as it can conflict with others. It is recommended to do pull request instead.

(<a href="#table-of-contents">back to top</a>)

---

<!-- DELETING BRANCHES -->
<h2>
<a id="five" href="#five" aria-hidden="true"></a>
Deleting Branches Locally / Remotely
</h2>
<h3 align="left">Locally</h3>

* **__`git branch -d <insertLocalBranchNameHere>`__** - deletes the merged branch locally (it's not needed anymore!).
   - "**_-d_**" only if the branch has been pushed and merged.
   - "**_-D_**" force the local branch to be deleted, even if it hasn't been pushed or merged yet (important! Always communicate with your team before using force!).
<h3 align="left">Remotely</h3>

* Or use this **__`git push origin --delete <insertRemoteBranchNameHere>`__** to remove remote branch.

(<a href="#table-of-contents">back to top</a>)

---

<!-- .GITIGNORE -->
<h2>
<a id="six" href="#six" aria-hidden="true"></a>
.gitignore
</h2>

Gitignore is essential part of the repository and workflow. It prevents __unnecessary files__ (e.g. large binary files which makes pushing to github very slow) and __secret files__ (e.g. file that includes password or other crucial information) being added to the repository.

* https://gitignore.io - on this page you will find ready-made .gitignore templates that you can use in your projects.

(<a href="#table-of-contents">back to top</a>)

---

<!-- ADDING .GITIGNORE -->
<h2>
<a id="seven" href="#seven" aria-hidden="true"></a>
Adding .gitignore into already existing repository
</h2>

When attempting to ignore a file (or files) that's already tracked in the repository, then do this:

1. Commit all changes
2. Removes any changed files from the index (staging phase).
   * **__`git rm -r --cached .`__**
      - "**_rm_**" - remove command
      - "**_-r_**" - allow recursive removal
      - "**_-cached_**" - only remove files from the index. Your files will still be there.
      - "**_._**" indicates all files will be untracked. Specific file with "git rm -r foo.txt"
   * With this command we untrack all of the files that have already been added to the repository. **Tl:dr** stop tracking but not delete from the system.
3. Add .gitignore file
4. Re-add everything
   * **__`git add .`__**
5. Commit 
   * **__`git commit -m "<insertCommentsHere>"`__**
6. Last step: **__`git push`__**

Becaution here as this will DELETE the file (or files) that is specified in the .gitignore from the github repository.

(<a href="#table-of-contents">back to top</a>)

---

<!-- CHEAT SHEET -->
<h2>
<a id="eight" href="#eight" aria-hidden="true"></a>
Cheat Sheet
</h2>

:large_orange_diamond: <a href="#three">Creating a branch</a> | Description
:------------ | :------------:
<img width=500px/> | <img width=500px/>
:small_orange_diamond: `git branch -a` | See all available branches
:small_orange_diamond: `git checkout -b <insertBranchNameHere>` | Create a new branch
:small_orange_diamond: `git switch <insertBranchNameHere>` | Switch between branches

:large_blue_diamond: <a href="#three">Adding files to a branch (not master)</a> | Description
:------------ | :------------:
<img width=500px/> | <img width=500px/>
:small_blue_diamond: `git add -i` | Interactive menu
:small_blue_diamond: `git status` | Files tracked by Git
:small_blue_diamond: `git restore --staged <insertFileNameToUnstage>` | Unstage unwanted file(s)
:small_blue_diamond: `git commit -m "<insertCommentsHere>"` | Record changes to the repository
:small_blue_diamond: `git push --set-upstream origin <insertBranchNameHere>` | Push staged files in to a branch

:white_medium_square: <a href="#four">Merging branches</a> | Description
:------------ | :------------:
<img width=500px/> | <img width=500px/>
:white_small_square: `git add -i` | Interactive menu
:white_small_square: `git commit -m "<insertCommentsHere>"` | Record changes to the repository
:white_small_square: `git switch master` | Switch to master branch
:white_small_square: `git merge <insertBranchNameHere> --no-ff` | Merges a branch into master

:red_square: <a href="#five">Deleting branches</a> | Description
:------------ | :------------:
<img width=500px/> | <img width=500px/>
:small_red_triangle: `git branch -d <insertLocalBranchNameHere>` | Delete local branch
:small_red_triangle: `git push origin --delete <insertRemoteBranchNameHere>` | Delete remote branch

(<a href="#table-of-contents">back to top</a>)

---

<!-- AUTHOR -->
<h2>
<a id="nine" href="#nine" aria-hidden="true"></a>
Author
</h2>

* [Raja Rana (LeDuble)](https://github.com/LeDuble/)

(<a href="#table-of-contents">back to top</a>)

---

<!-- HOW TO CONTRIBUTE -->
<h2>
<a id="ten" href="#ten" aria-hidden="true"></a>
How to Contribute
</h2>

1. Clone repository and create a new branch: **__`git checkout https://github.com/LeDuble/Git-Etiquette.git -b <insertBranchNameHere>`__**
2. Add changes to your branch
3. Create a Pull Request with descriptive text.
4. Leave a star :star_struck:

Feed back and suggestions are welcome! 

(<a href="#table-of-contents">back to top</a>)

---

<!-- LICENSE -->
<h2>
<a id="eleven" href="#eleven" aria-hidden="true"></a>
License
</h2>

[![License](https://img.shields.io/badge/license-CC%20BY--SA%204.0-blue)](https://creativecommons.org/licenses/by-sa/4.0/)

You can read the full license [here](https://github.com/LeDuble/Git-Etiquette/blob/master/LICENSE.md)


---

<!-- FUTURE UPDATES -->
<h2>
<a id="twelve" href="#twelve" aria-hidden="true"></a>
Future Updates
</h2>
TODO

- [ ] TODO
- [ ] TODO
- [ ] TODO
- [ ] TODO