<!-- TITLE -->
<h1 align="center">
<a id="title" href="#title" aria-hidden="true"></a>
Git Etiquette and Cheat Sheet
</h1>

<p align="center">This Git Etiquette and Cheat Sheet is made for The Software Developer Team of Virittämö Helsinki.</p>

<!-- TABLE OF CONTENTS -->
<h2>
<a href="table-of-contents" aria-hidden="true"></a>
Table of Contents
</h2>
<ol>
<li><a href="#descr">Introduction</a></li>
<li><a href="#one">When starting a new project - follow these steps</a></li>
<li><a href="#two">Structure of projects beta board</a></li>
<li><a href="#three">Labels</a></li>
<li><a href="#four">To-do list and issues</a></li>
<!-- <li><a href="#four">Merging Branches</a></li>
<li><a href="#five">Deleting Branches Locally & Remotely</a></li>
<li><a href="#six">.gitignore</a></li>
<li><a href="#seven">Adding .gitignore into already existing repository</a></li>
<li><a href="#eight">Cheat Sheet</a></li>
<li><a href="#nine">Authors</a></li>
<li><a href="#ten">How to Contribute</a></li>
<li><a href="#eleven">License</a></li>
<li><a href="#twelve">Future Updates</a></li>
</ol> -->

---

<!-- Introduction -->
<h2>
<a id="descr" href="#descr" aria-hidden="true"></a>
Introduction
</h2>

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-success)](http://makeapullrequest.com)
[![License](https://img.shields.io/badge/license-CC%20BY--SA%204.0-blue)](https://creativecommons.org/licenses/by-sa/4.0/)

<div>This part focuses on the project management and how to setup the environment for it.</div></br>

<div>What you need:</div>

- Projects beta board
- Projects beta automatization files (can be found here)
- Creation of the team (project specific, inside the organization)
- Issues page
- Issues & Pull request templates (can be found here)

</br><div>This helps creating exceptional base for tracking the issues and documentation. Your team leader & co-workers will thank you later for doing the base work. </div>

<div>Noteworthy is that having everything organized right a way at the beginning of a project will help your team leader, co-workers and potential new developers to keep on track what's happening with the project. Proper documentation is basis to everything to help your team to succeed with the project.
<!-- When starting a new project in an organization then follow these steps to improve work flow within the team and organization!
This helps creating exceptional base for tracking the issues and documentation. Your team leader & co-workers will thank you later for doing the base work.
Having everything organized right at the beginning of a project will help your team leader, co-workers and potential new developers to keep on track what's happening with the project. Proper documentation is basis to everything to help your team to succeed with the project. -->

(<a href="#table-of-contents">back to top</a>)

---

<!-- Starting a projects beta board -->
<h2>
<a id="descr" href="#one" aria-hidden="true"></a>
Starting a Project - Necessary First Steps
</h2>
<div>These are the primary steps that should be followed when starting a new project</div>

1. **Make a new repository**
2. **Start a projects beta board**
3. **Create a team**
   1. Add people who will be working on the project
   2. Add the project related repositories via 'repository' tab
   <!-- 3. Start a discussion inside the team page 
      1. Include direct link to-do issues page (for easy and quick access)
      2. Pin it -->
4. **Create a to-do list in issues page**
   1. Add following titles: **Major**, **Minor** and **Other** (an example can be found <a href="https://github.com/LeDuble/Git-Etiquette/issues/1">here</a>)
   2. Start creating issues/task cards
      * You can either **start issues** from the to-do list like this:
         * <img src="https://cdn.discordapp.com/attachments/907908132884320316/933374215195852820/unknown.png" width="500">
      * or **if an issue already exist**, then type hashtag (#) followed by specified number (e.g. `#2`)
      <!-- 1. Edit to-do list
         * template (note it's important to include `- [ ]` to make it work):
         * _```- [] <write issue here>```_
      2. Save it
      3. On the right side of the text appears "convert to issue" button. Click it.  -->
5. **Add the following .github files in to the repository**
   * Here will be the templates for the issues & pull request. Keeping them clean and organized. 
   * Also it includes a file that automates that issues are automatically added to the projects beta board.

</br><div> Some of these steps can still be used for an already started project. So, no worries, if you have already started a project and want to use these with it, you still can!</div>
   <!-- These files gives you templates for issue & pull request creation. But also a file that gives you access to  Simply said, keeps them clean and organized.
   * Also they inclu -->


(<a href="#table-of-contents">back to top</a>)

---

<!-- Structure of projects beta board -->
<h2>
<a id="descr" href="#one" aria-hidden="true"></a>
The Structure of The Projects Beta Board
</h2>
<div>
Titles, views, statuses and labels needed for the projects beta board and their order.
</div></br>

<div><b>Views:</b></div>
<img src="https://cdn.discordapp.com/attachments/907908132884320316/1001387911335379065/unknown.png" width="500">

<div><b>Titles:</b></div>
<img src="https://cdn.discordapp.com/attachments/907908132884320316/1001386289981046815/unknown.png" width="500">
<div><b>Labels:</b></div>
<img src="https://cdn.discordapp.com/attachments/907908132884320316/1001386289981046815/unknown.png" width="500">
read more about labels <a href="">here</a>
<div><b>Statuses:</b></div>
<img src="https://cdn.discordapp.com/attachments/907908132884320316/1001386289981046815/unknown.png" width="500">



<div>Follow the structure for the views, labels and titles to keep project standardized within the organization.</div></br>

<div>It's also important to maintain the structure for the workflow file that automatizes the "pipeline" between issues and projects beta board (For an example if title or view names are incorrect it may cause instability or errors when the automatization file is run with github actions).</div>



(<a href="#table-of-contents">back to top</a>)

---


<!-- Starting a projects beta board -->
<h2>
<a id="descr" href="#three" aria-hidden="true"></a>
Labels
</h2>
<div>Labels are pretty much same than in the git etiquette main page.</div>

   * **Docs** - Changes to documentation only
   * **Feat** - A new feature
   * **Style** - Changes to formatting (e.g. the code is missing semicolons).
   * **Test** - Adding/correcting existing tests.
   * **Refactor** - A code change which isn't bug fix or adds a feature. It's restructure of the code without changing the functionality.
   * **BugFix** - A bug fix.
   * **Chore** - Maintenance or change to auxiliary tools.
   * **Add** - Adding essentials to the repository (e.g. .gitignore or example files).

 # ----------------- labels ----------------- #
   * unassigned: Unassigned ❕
   * unlabeled: Unlabeled ❗
   * docs: Docs 📝
   * feat: Feat 🆕
   * style: Style 🖌️
   * test: Test ☑️
   * refactor: Refactor 🔁
   * bugfix: BugFix 🐛
   * chore: Chore 👷‍♂️
   * add: Add ➕
   * backend: Backend ⚙️e
   * frontend: Frontend 🖥️
   * design: Design 🎨

# ----------------- projects fields ----------------- #
   * un_assigned: Unassigned ❕
   * un_labeled: Unlabeled ❗
   * backlog: Backlog 📜
   * in_progress: In Progress 🚧
   * ready_for_review: Ready for Review 🔍
   * done: Done ✔️


(<a href="#table-of-contents">back to top</a>)

---


<!-- Starting a projects beta board -->
<h2>
<a id="descr" href="#four" aria-hidden="true"></a>
To-do list and issues
</h2>

1. **Make a new repository**
2. **Start a projects beta board**
3. **Create a team**
   1. Add people who will be working on the project
   2. Add the project related repositories via 'repository' tab
   3. Start a discussion in the team page 
      1. Include link to it (for easy and quick access)
      2. Pin it
4. **Create a to-do list in issues page**
   1. Add following headers: **Major**, **Minor** and **Other**
   * You can either **start issues** from to-do list
      1. Edit to-do list
         * template (note it's important to include `- [ ]` to make it work):
         * _```- [] <write issue here>```_
      2. Save it
      3. On the right side of the text appears "convert to issue" button. Click it. 
      * <img src="https://cdn.discordapp.com/attachments/907908132884320316/933374215195852820/unknown.png" width="500">
      
   * or **if an issue already exist**, then type hashtag (#) followed by specified number (e.g. `#2`)


(<a href="#table-of-contents">back to top</a>)

---
