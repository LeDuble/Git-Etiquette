<!-- TITLE / HEADER -->
<h1 align="left">
<a id="title" href="#title" aria-hidden="true"></a>
Git Etiquette
</h1>

<p align="center">
   <img height="180" src="https://github.com/LeDuble/Git-Etiquette/blob/main/imgs/logos_tms_orgs/git-etiquette-banner-no-bg.png">
</p>

<p align="center"> 
   <b>Standardized workflow frame for teams and individuals.</b>

</p>

<p align="center">
   <a href="https://creativecommons.org/licenses/by-sa/4.0/">
    <img title="License" src="https://img.shields.io/badge/license-CC%20BY--SA%204.0-blue">
   </a>
   <a href="http://makeapullrequest.com">
    <img title="PRs Welcome" src="https://img.shields.io/badge/PRs-welcome-success">
   </a>
   <a href="https://github.com/LeDuble/Git-Etiquette/graphs/contributors">
    <img title="Contributors" src="https://img.shields.io/github/contributors/LeDuble/Git-Etiquette">
   </a>
   <a href="https://github.com/LeDuble/Git-Etiquette">
    <img title="Star on GitHub" src="https://img.shields.io/github/stars/LeDuble/Git-Etiquette.svg?style=social&label=Star">
   </a>
</p>

<!-- Features -->
<h1>
<a id="feat" href="#feat" aria-hidden="true"></a>
Features
</h1>

- **Git strategy for branching**  
- **Issues, labels and project board automation**    
- **Git command cheat sheet**

<!-- TABLE OF CONTENTS -->
<h2>
<a id="table-of-contents" href="#table-of-contents" aria-hidden="true"></a>
Table of Contents
</h2>
<ol>
<li><a href="#intro">Introduction</a></li>
<!-- <li><a href="#feat">Features</a></li> -->
<li><a href="#start">Getting Started</a></li>
<ul><a href="#proj">- Project board</a></ul>
<ul><a href="#labe">- The labels for issues </a></ul>
<ul><a href="#issu">- Issues forms and pull request template </a></ul>
<ul><a href="#wfile">- Workflow file setup </a></ul>
<ul><a href="#base">- Base tree for repository </a></ul>
<li><a href="#gtst">Git strategy and usage</a></li>
<ul><a href="#bed">- Bedrock Rules</a></ul>
<ul><a href="#bran">- Branch Strategy</a></ul>
<ul><a href="#form">- Formatting Rules</a></ul>
<li><a href="#usfgit">Useful Git Commands</a></li>
<ul><a href="#creabr">- How to Create a Branch (via Git)</a></ul>
<ul><a href="#dltbr">- Deleting Branches Locally & Remotely</a></ul>
<ul><a href="#gitig">- .gitignore</a></ul>
<ul><a href="#addig">- Adding .gitignore into already existing repository</a></ul>
<ul><a href="#mergbr">- Merging Branches</a></ul>
<li><a href="#chtsht">Cheat Sheet</a></li>
<li><a href="#orgs">Featured organizations, teams, and projects that utilize the Git Etiquette</a></li>
<li><a href="#ten">How to Contribute</a></li>
<li><a href="#nine">Authors</a></li>
<li><a href="#eleven">License</a></li>
</ol>

---

<!-- INTRODUCTION -->
<h1>
<a id="intro" href="#intro" aria-hidden="true"></a>
Introduction
</h1>

The main focus of Git Etiquette is to provide a standard way of using Git and project management tools that is shared among developers, which helps to ensure that everyone is on the same page and following the same standardized workflow frame. 

By following the Etiquette, the team can ensure that their workflow will be more consistent, work will be properly documented and their use of the git will be more efficient.
Additionally, it provides clear instructions for using Git, which helps to minimize the risk of errors and improves the quality of the work being done.

The background story for Git Etiquette is that it was started as a personal project to create a unified and coherent workflow for personal use. The goal was to make it easier for others to understand the work being done and navigate the history of the project more easily.

My team leader was excited about my personal project I was working on and assigned me to write it up so that the rest of the team could benefit from it.

(<a href="#table-of-contents">back to top</a>)

---

<!-- Getting started -->
<h1>
<a id="start" href="#start" aria-hidden="true"></a>
Getting started 
</h1>

<ol>
<li><a href="#proj">Project board</a></li>
<li><a href="#labe">The labels for issues </a></li>
<li><a href="#issu">Issues forms and pull request template </a></li>
<li><a href="#wfile">Workflow file setup </a></li>
<li><a href="#base">Base tree for repository </a></li>
</ol>

(<a href="#table-of-contents">back to top</a>)


<!-- Project board -->
<h2>
<a id="proj" href="#proj" aria-hidden="true"></a>
Project Board
</h2>
Here's how you setup your project board, which is a crucial part of automation and project management.

<img align=left width="163" height="287" alt="" src="https://github.com/LeDuble/Git-Etiquette/blob/main/imgs/logos_tms_orgs/savechanges.png"></img>
#### Views
Project views allow you to view the project from different layouts and are located at the top as tabs.

Set up for each view:
Name | Layout | Group | Fields
--- | --- | --- | ---
*List view by status* | Table | Status | All, except Milestones
*Board view* | Board | Default | All, except Milestones, Tracks, Tracked by
*List all* | Table | Default | All, except Milestones

Remember to save changes!

#### Status
In projects, click the three dots in the top right corner, select Settings, then under Custom Fields, click on Status and add the following statuses (including the emojis):
<!-- * Unassigned ❕
* Unlabeled ❗ -->
* **Backlog 📜**
* **In Progress 🚧**
* **Ready for Review 🔍**
* **Done ✔️**

Also don't forget to remove any default statuses.

#### Example
You can view the project board of this repository to get an example of what the project board should look like and how the automation is handled.

<a href="https://github.com/users/LeDuble/projects/5/views/1">A project board</a>

(<a href="#start">back to Getting Started</a>)

(<a href="#table-of-contents">back to top</a>)

<!-- The labels for issues -->
<h2>
<a id="labe" href="#labe" aria-hidden="true"></a>
The labels for issues
</h2>

#### Featured labels
* Labels can either be assigned automatically by the automation or manually by the user. It is best to let the automation handle the assignment of labels marked as "automatically" and not add them manually to an issue.
* when a new issue is opened, it will be automatically assigned the "Backlog 📜" label. If an issue is already labeled as "In Progress 🚧", you can change the label back to "Backlog 📜" if needed.

#### Adding labels to the repository
You can add labels by going to the repository, clicking on the <i>Issues</i> tab, and then clicking on the <i>Labels</i> button, which is located next to the milestones option, and now you can start copying these labels by clicking on the <i>New Labels</i> button.

<img width="386" height="64" alt="" src="https://github.com/LeDuble/Git-Etiquette/blob/main/imgs/logos_tms_orgs/labelsteps.jpg">


#### Organization default repository labels
If you plan to use these labels across all of your organization's future repositories, then you can go to your organization's <i>settings</i>, navigate to the <i>repository</i> section under <i>"code, planning, and automation"</i>, and click on <i>repository defaults</i>. Then, you can click on the <i>new label</i> button and add the labels. These labels will featured in all of organization's future repositories, but will not be added to already existing repositories, so you will need to add them manually to those. 

Label Name | Description | Manually or Automatically | Label / Status Field
--- | --- | --- | :---:
Docs 📝 | Changes to documentation only | Manually | Label
Feat 🆕 | A new feature | Manually | Label
Style 🖌️ | Changes to formatting (e.g. the code is missing semicolons) | Manually | Label
Test ☑️ | Adding/correcting existing tests | Manually | Label
Refactor 🔁 | A code change which isn't bug fix or adds a feature. It's restructure of the code without changing the functionality | Manually | Label
BugFix 🐛 | A bug fix | Manually | Label
Chore 👷‍♂️ | Maintenance or change to auxiliary tools | Manually | Label
Add ➕ | Adding essentials to the repository (e.g. .gitignore or example files) | Manually | Label
Backend ⚙️ | When a backend issue is opened, it is automatically given to the issue | Automatically | Label
Frontend 🖥️ | When a fronted issue is opened, it is automatically given to the issue | Automatically | Label
Design 🎨 | When a design issue is opened, it is automatically given to the issue | Automatically | Label
Unassigned ❕ | Currently nobody has been assigned to it | Automatically | Label
Unlabeled ❗ | No labels have been added | Automatically | Label
Backlog 📜 | Tasks that have not yet been started or left unfinished | Both | Both
In Progress 🚧 | Currently in the process of being worked on | Manually | Both
Ready for Review 🔍 | A pull request has been created and it is ready for review | Manually | Both
Done ✔️ | Task has been completed or closed | Manually | Both

* When copying and pasting labels, make sure to include any associated emojis.

(<a href="#start">back to Getting Started</a>)

(<a href="#table-of-contents">back to top</a>)

<!-- Issues forms and pull request template -->
<h2>
<a id="issu" href="#issu" aria-hidden="true"></a>
Issues forms and pull request template
</h2>

Make sure to add the issue form files to the `.github/ISSUE_TEMPLATE` folder in your repository, and the pull request template goes to the `.github` folder.

Pick them from here:
Issue forms | Pull request template
---|---
<a href="https://github.com/LeDuble/Git-Etiquette/blob/main/.github/ISSUE_TEMPLATE/backend-card.yml">backend-card.yml</a> | <a href="https://github.com/LeDuble/Git-Etiquette/blob/main/pull_request_template.md">pull_request_template.md</a>
<a href="https://github.com/LeDuble/Git-Etiquette/blob/main/.github/ISSUE_TEMPLATE/design-card.yml">design-card.yml</a> |
<a href="https://github.com/LeDuble/Git-Etiquette/blob/main/.github/ISSUE_TEMPLATE/frontend-card.yml">frontend-card.yml</a> |
<!-- <a href="">config.yml</a> | -->

When creating an issue, depending on which one you pick, the form will automatically add one of the three labels (Backend ⚙️, Design 🎨, or Frontend 🖥️). For example, if you select a card related to backend development, it will add the "Backend ⚙️" label.

   <ol>
   <li>Open a new issue inside the repository.</li>
   <li>Choose one of the cards or templates (Backend, Frontend, or Design).</li>
   <ul>- For example if you choose the backend card, then the Backend ⚙️ label will be added.</ul>
   <ul>- Backlog 📜 label is always added when opening an issue.</ul>
   <li>Pick one descriptive label from this list: Docs 📝, Feat 🆕, Style 🖌️, Test ☑️, Refactor 🔁, BugFix 🐛, Chore 👷‍♂️, Add ➕ </li>
   <li>you can add another label from this list: In Progress 🚧, Done ✔️</li>
   <ul>The label "In Progress 🚧" means that someone is currently working on the issue.</ul>
   <ul>The label "Done ✔️" indicates that the issue has been completed or closed.</ul>
   </ol>

   ```mermaid

   %%{init: {'themeVariables': { 'fontSize': '20px'}}}%%
    graph LR;
        classDef infoboxcolors fill:#fff2cc, color:#000000;
        classDef firstboxcolors fill:#dae8fc, color:#000000;
        classDef secondboxcolors fill:#e1d5e7, color:#000000;
        classDef thirdboxcolors fill:#d5e8d4, color:#000000;

    subgraph Main
    style Main color:#00000000, fill:#00000000, stroke:#f66, stroke-width:2px, stroke-dasharray:5 5
    
    subgraph .
    style . color:#00000000, fill:#00000000, stroke-width:3px, stroke:#f66
        subgraph 1.
        style 1. color:#272B30, stroke:#f66, fill:#f8cecc
    end

        X([Open an issue])-->A[Project];
        class X infoboxcolors;
        class A firstboxcolors;
        end
    
    subgraph ..
    style .. color:#00000000, fill:#00000000, stroke-width:3px, stroke:#f66
        subgraph 2.
        style 2. color:#272B30, stroke:#f66, fill:#f8cecc
    end

        A-.->XX([Choose</br> a template]);
        class XX infoboxcolors;

        XX-->B((Backend)) & C((Frontend)) & D((Design));
        class B,C,D secondboxcolors;
        end

    subgraph ...
    style ... color:#00000000, fill:#00000000, stroke-width:3px, stroke:#f66
        subgraph 3.
        style 3. color:#272B30, stroke:#f66, fill:#f8cecc
    end

        .... -.->XXX([A more descriptive</br>label</br>is added</br>manually]);
        class XXX infoboxcolors;
        XXX-->E(Docs);
        XXX-->F(Feat);
        XXX-->G(Style);
        XXX-->H(Test);
        XXX-->I(Refactor);
        XXX-->J(Bugfix);
        XXX-->K(Chore);
        XXX-->L(Add);
        XXX-->R(In Progress);
        XXX-->S(Done);
        class E,F,G,H,I,J,K,L,M,N,O,P,Q,R,S,T,U thirdboxcolors;
        end
    
    subgraph ....
    style .... color:#00000000, fill:#00000000, stroke-width:3px, stroke:#f66
        subgraph 3.
        style 3. color:#272B30, stroke:#f66, fill:#f8cecc
    end

        Frontend & Backend & Design & Backlog -.- XXXX([These labels</br>will be automatically</br>added accordingly]);
        class XXXX infoboxcolors;
        C-->Frontend(Frontend);
        B-->Backend(Backend);
        D-->Design(Design);
        C & B & D-->Backlog(Backlog);
        class E,F,G,H,I,J,K,L,M thirdboxcolors;
        end
    end

   ```
   Schema for labeling.

(<a href="#start">back to Getting Started</a>)

(<a href="#table-of-contents">back to top</a>)

<!-- Workflow file setup -->
<h2>
<a id="wfile" href="#wfile" aria-hidden="true"></a>
Workflow file setup
</h2>

Variable | Description | Example Organisation / User specific setting |
--- | --- | ---
`username` | | User
`gh_project_token` | | User
`organization_name` | | Organisation
`gh_app_key` | | Organisation
`gh_app_id` | | Organisation
`gh_app_installation_id` | | Organisation
`project_number` | | Both
`project_portfolio_number` | | Both

### Authentication for user
Create a Personal Access Token (PAT)
1. Let's begin with creating a PAT by going to the <i>personal settings</i>. From there, go to <i>the developer settings</i> and then click on the <i>personal access tokens</i> on the left menu, which opens a menu of two items. Pick the <i>tokens (classic)</i> from the dropdown menu, and then press the button that says <i>"Generate new token"</i> to generate a new token (classic)

For additional details on creating a PAT, refer to the <a href="https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token#keeping-your-personal-access-tokens-secure">documents</a>

2. Select the following scopes (permissions)
   * <b>repo</b> - <i>all</i>
   * <b>admin:org</b> - <i>write:org</i>
   * <b>admin:org</b> - <i>read:org</i>
   * <b>project</b> - <i>read:project</i>

3. Save the given token in to your repository secrets and name it as `SECRET_TOKEN` so that the workflow file knows what to look for.
   
### Authentication for organisation (via app)
* Start by creating a Github App under your organization. Follow the instructions in the <a href="https://docs.github.com/en/apps/creating-github-apps/creating-github-apps/creating-a-github-app">documents</a>.

#### App settings
*  For the newly created Github App, set the following requirements: 
   * Repository permissions (8 in total) 
      * <b>Actions</b> - <i>Read and write</i>
      * <b>Checks</b> - <i>Read and write</i>
      * <b>Commit statuses</b> - <i>Read only</i>
      * <b>Contents</b> - <i>Read and write</i>
      * <b>Environments</b> - <i>Read only</i>
      * <b>Issues</b> - <i>Read only</i>
      * <b>Metadata</b> - <i>Read only</i>
      * <b>Pull requests</b> - <i>Read only</i>
   * Organization permissions (2 in total)
      * <b>Members</b> - <i>Read only</i>
      * <b>Projects</b> - <i>Read and write</i>
   
   * Check the <a href="https://docs.github.com/en/apps/maintaining-github-apps/editing-a-github-apps-permissions">documents</a> to see how to edit the permissions of the Github App.

* Go to Optional features (in the app) and opt-out from the following setting:
   * User-to-server token expiration
* Generate a private key, treat the file like the password and keep it safe.

#### Installing
* Install the Github App in the organization
   * To install the GitHub App in your organization, go to your <i>organization's settings</i>, navigate to <i>Developer settings</i>, select <i>GitHub Apps</i>, click <i>edit</i> next to the app, select <i>Install App</i>, and then click <i>Install</i>.

#### Secrets
* To make the <i><b>private key</b></i>, <i><b>the GitHub App's installation id</b></i>, and <i><b>the App's id</b></i> accessible to all the repositories in the organization for the workflow file, store the private key as `PRIVATE_KEY`, the GitHub App's installation id as `APP_INSTALLATION_ID`, and the app's id as `APP_ID` as secrets in the organization's settings and actions.
   * <i><b>The private key</b></i> can be generated within the app itself, by navigating to the app's settings and selecting the Generate Private Key option.
   * <i><b>App id</b></i> can be found from configuration general page as <i>App ID</i>
   * To find <i><b>the app installation id</b></i>, navigate to your organization's settings, select Github Apps, and then select Configure next to the app. The `app installation id` can be found now in the address bar, like this: `https://github.com/organizations/<organization>/settings/installations/<id>`

#### Finding number of project board
* Go to the project board and then look in the address bar, it should appear like this: `https://github.com/users/<username>/projects/<number>` and for the organization it should appear like this: `https://github.com/orgs/<organizationname>/projects/<number>`
* Project id is necessary for the automation.

(<a href="#start">back to Getting Started</a>)

(<a href="#table-of-contents">back to top</a>)

#### Editing the parameters in WFprojects.yml file
Only the parameters should be changed that are inside the angle brackets (`<>`). For example, ```username: octocat``` or ```project_number: 1``` (remember to remove anglebrackets).

These parameters can be found org/user related settings in the WFprojects.yml file and are almost at the beginning of the file. 

* User related settings (only edit these).
```  # ----------------- user related settings (only edit these) ----------------- #
username: <username>
gh_project_token: ${{ secrets.SECRET_TOKEN }}
project_number: <projectid>
```
* Organization related settings.
``` # ----------------- org related settings (only edit these) ----------------- #
organization_name: <organization>
gh_app_key: ${{ secrets.APP_SECRET_KEY }}
gh_app_id: ${{ secrets.APP_ID }}
gh_app_installation_id: ${{ secrets.APP_INSTALLATION_ID }}
project_number: <projectid>
```

<!-- Base tree for repository -->
<h2>
<a id="base" href="#base" aria-hidden="true"></a>


Base tree for repository
</h2>
In the end the base of the repository should look like this:

```text
.
├── .github
│   ├── CODE_OF_CONDUCT.md
│   ├── CONTRIBUTING.md
│   ├── ISSUE_TEMPLATE
│   │   ├── backend-card.yml
│   │   ├── design-card.yml
│   │   ├── frontend-card.yml
│   │   └── config.yml
│   ├── workflows
│   │   └── WFprojects.yaml
│   └── pull_request_template.md
├── .gitignore
└── README.md

3 directories, 10 files
```
Excluding .gitignore file. There's topic about .gitignore later in this guide, which I recommend to check out.
<!-- which you can
read more about <a href=six>here</a> and how to add it. -->

(<a href="#start">back to Getting Started</a>)

(<a href="#table-of-contents">back to top</a>)

---

<!-- Git strategy and usage -->
<h1>
<a id="gtst" href="#gtst" aria-hidden="true"></a>
Git strategy and usage
</h1>

<ol>
<li><a href="#bed">Bedrock Rules</a></li>
<li><a href="#bran">Branch Strategy</a></li>
<li><a href="#form">Formatting Rules</a></li>
</ol>

(<a href="#table-of-contents">back to top</a>)

<!-- BEDROCK RULES -->
<h2>
<a id="bed" href="#bed" aria-hidden="true"></a>
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

(<a href="#gtst">back to Git Strategy and Usage</a>)

(<a href="#table-of-contents">back to top</a>)

<!-- Branching Strategy -->
<h2>
<a id="bran" href="#bran" aria-hidden="true"></a>
Branching Strategy
</h2>

<img align="right" width="242" height="622" alt="" src="https://github.com/LeDuble/Git-Etiquette/blob/main/imgs/logos_tms_orgs/GitStrategySimplified.png">
The strategy is based on the Git Flow strategy, where each feature (or issue) is represented by a separate branch. Every new branch created is a feature that is being added or worked for the project. The main branch is the production branch, which is the version that is sent to the customer and is always the working one. The dev branch is where all the feature branches are pull requested to aka merged.

The actual Git Flow strategy also includes release and hotfix branches, which are not included in this strategy. Additonally, version numbering is missing, which might be added later.

### Strategy guideline

#### Branches
Name | Description
--- | ---
main | A production branch
dev | A development branch
feature branches | Each issue is one feature branch
#### Merging
* The merge order is from feature branch to development branch, and then from development branch to main branch. This order ensures that changes are tested in the development branch before they are merged in to the main branch. 
   * Simply said: the merge order is: feature > dev > main.
* Always open pull request from feature branch to dev branch (never to main!).
* Each issue equals to one feature which is represented by one feature branch.
* Always open pull request, instead of merging straight to the branch! This ensures that changes are peer reviewed and any potential problems can be identified before the changes are applied to the branch. Even if the problems were accepted via a pull request, it is still easy to revert back if needed.

#### Naming conventions for the branches
* In the two next sections, you can find instructions on how to properly format the branches in order to ensure the team is following a consistent workflow and that the branches are properly documented.

#### 

(<a href="#gtst">back to Git Strategy and Usage</a>)

(<a href="#table-of-contents">back to top</a>)

<!-- FORMATTING RULES -->
<h2>
<a id="form" href="#form" aria-hidden="true"></a>
Formatting Rules for a Branch (Type/Reference ID/Description)
<!-- Formatting Rules for a Branch Creation -->
</h2>

### 1. Type
   * **Docs** - Changes to documentation only
   * **Feat** - A new feature
   * **Style** - Changes to formatting (e.g. the code is missing semicolons)
   * **Test** - Adding/correcting existing tests
   * **Refactor** - A code change which isn't bug fix or adds a feature. It's restructure of the code without changing the functionality
   * **BugFix** - A bug fix
   * **Chore** - Maintenance or change to auxiliary tools
   * **Add** - Adding essentials to the repository (e.g. .gitignore or example files)

### 2. Reference ID
   Reference the issue from GitHub, Trello or some other agile source. 
   For now use one of the two formats shown below.
   * Referencing an issue from Github: **__issue(_insert number here_)__** or just **__hashtag + number__** (e.g. **_/issue12/_** or **_/#12/_**)
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

(<a href="#gtst">back to Git Strategy and Usage</a>)

(<a href="#table-of-contents">back to top</a>)

---

<!-- USEFUL GIT COMMANDS  -->
<h1>
<a id="usfgit" href="#usfgit" aria-hidden="true"></a>
Useful Git Commands
</h1>

<ol>
<li><a href="#creabr">How to Create a Branch (via Git)</a></li>
<li><a href="#dltbr">Deleting Branches Locally & Remotely</a></li>
<li><a href="#gitig">.gitignore</a></li>
<li><a href="#addig">Adding .gitignore into already existing repository</a></li>
<li><a href="#mergbr">Merging Branches</a></li>
</ol>

(<a href="#table-of-contents">back to top</a>)

<!-- CREATE A BRANCH -->
<h2>
<a id="creabr" href="#creabr" aria-hidden="true"></a>
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
      * There are alternative ways (e.g. `git add .`) to add changes to staging area but, they are not preferred unless you are experienced git user. Interactive menu gives easy access to control what changes we want to add to staging phase and push forward.
* **__`git status`__**
   * Shows which files are tracked by Git and which changes have been staged (which have been not).
* **__`git restore --staged <insertFileNameToUnstage>`__**
   * Note: Incase you added something you don't want to push.
* **__`git commit -m "<insertCommentsHere>"`__**
   * Record changes to the repository
* **__`git push --set-upstream origin <insertBranchNameHere>`__** 
   * (You can do alias for this)

(<a href="#usfgit">back to Useful Git Commands</a>)

(<a href="#table-of-contents">back to top</a>)

<!-- MERGING BRANCHES -->
<h2>
<a id="mergbr" href="#mergbr" aria-hidden="true"></a>
Merging Branches
</h2>

Very important: when merging, make sure that you are on the branch that you want to merge to. You will tell Git basically: "see those new stuff? Bring them over here."
1. **__`git add -i`__**
2. **__`git commit -m "<insertCommentsHere>"`__**
3. **__`git checkout master`__**
4. **__`git merge <insertBranchNameHere> --no-ff`__**
   * Additional command "**_--no-ff_**" tells Git that you want to retail all of the comments prior to the merge. Makes tracking easier in the future.

Always consult before merging directly as it can conflict with others. It is recommended to do pull request instead.

(<a href="#usfgit">back to Useful Git Commands</a>)

(<a href="#table-of-contents">back to top</a>)

<!-- DELETING BRANCHES -->
<h2>
<a id="dltbr" href="#dltbr" aria-hidden="true"></a>
Deleting Branches Locally / Remotely
</h2>
<h3 align="left">Locally</h3>

* **__`git branch -d <insertLocalBranchNameHere>`__** - deletes the merged branch locally (it's not needed anymore!).
   - "**_-d_**" only if the branch has been pushed and merged.
   - "**_-D_**" force the local branch to be deleted, even if it hasn't been pushed or merged yet (important! Always communicate with your team before using force!).
<h3 align="left">Remotely</h3>

* Or use this **__`git push origin --delete <insertRemoteBranchNameHere>`__** to remove remote branch.

(<a href="#usfgit">back to Useful Git Commands</a>)

(<a href="#table-of-contents">back to top</a>)

<!-- .GITIGNORE -->
<h2>
<a id="gitig" href="#gitig" aria-hidden="true"></a>
.gitignore
</h2>

Gitignore is essential part of the repository and workflow. It prevents __unnecessary files__ (e.g. large binary files which makes pushing to github very slow) and __secret files__ (e.g. file that includes password or other crucial information) being added to the repository.

* https://gitignore.io - on this page you will find ready-made .gitignore templates that you can use in your projects.

(<a href="#usfgit">back to Useful Git Commands</a>)

(<a href="#table-of-contents">back to top</a>)

<!-- ADDING .GITIGNORE -->
<h2>
<a id="addig" href="#addig" aria-hidden="true"></a>
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

(<a href="#usfgit">back to Useful Git Commands</a>)

(<a href="#table-of-contents">back to top</a>)

---

<!-- CHEAT SHEET -->
<h2>
<a id="chtsht" href="#chtsht" aria-hidden="true"></a>
Cheat Sheet
</h2>

### :large_orange_diamond: <a href="#three">Creating a branch</a>
Command | Description | Frequently used?
------------ | ------------ | :------------:
`git pull` | Before starting a pull command, it is important to make sure that your working copy is clean and free of any uncommitted local changes. To accomplish this, you can use git's Stash feature to save your local changes temporarily so that they are not overwritten when you pull. This will ensure that any changes you make to the repository are safe and secure. |
`git branch -a` | See all available branches | :+1:
`git checkout -b <insert example: chore/#12/gitignore>` | Create a new branch | :wavy_dash:
`git switch <insertBranchNameHere>` | Switch between branches | :+1:

### :large_blue_diamond: <a href="#three">Adding files to a branch (not master)</a>
Command | Description | Frequently used?
------------ | ------------ | :------------:
`git add -i` | Interactive menu | :+1:
`git status` | Files tracked by Git | :+1:
`git restore --staged <insertFileNameToUnstage>` | Unstage unwanted file(s) | :wavy_dash:
`git commit -m "<insertCommentsHere>"` | Record changes to the </br>repository | :+1:
`git push --set-upstream origin <insertBranchNameHere>` | Push staged files in to </br>a branch | :+1:

### :red_square: <a href="#five">Deleting branches</a>
Command | Description | Frequently used?
------------ | ------------ | :------------:
`git branch -d <insertLocalBranchNameHere>` | Delete local branch | :wavy_dash:
`git push origin --delete <insertRemoteBranchNameHere>` | Delete remote branch | :wavy_dash:

### :white_medium_square: <a href="#four">Merging branches</a>
note: merging directly to master or main is not generally recommended, always do a pull request! ! !
Command | Description | Frequently used?
------------ | ------------ | :------------:
`git add -i` | Interactive menu | :+1:
`git commit -m "<insertCommentsHere>"` | Record changes to the repository | :+1:
`git switch master` | Switch to master | :+1:
`git merge <insertBranchNameHere> --no-ff` | Merges a branch into master | :-1:

### Git Flow Strategy Cheat Sheet as in schema
[![GitFlow](https://github.com/LeDuble/Git-Etiquette/blob/main/imgs/logos_tms_orgs/GitStrategyCheatSheet.png)](https://creativecommons.org/licenses/by-sa/4.0/)

(<a href="#table-of-contents">back to top</a>)

---

<!-- EXAMPLES -->
<h2>
<a id="orgs" href="#orgs" aria-hidden="true"></a>
Featured organizations, teams, and projects that utilize the Git Etiquette
</h2>

| <a href=https://github.com/VirittamoHelsinki>Virittämö Helsinki</a> | <a href=https://github.com/VirittamoHelsinki/aava-backend>Aava</a>
:-------------------------:|:-------------------------:|
<img width="200" height="200" alt="" src="https://github.com/LeDuble/Git-Etiquette/blob/main/imgs/logos_tms_orgs/logohkv.jpg"> | <img width="200" height="200" alt="" src="https://github.com/LeDuble/Git-Etiquette/blob/main/imgs/logos_tms_orgs/aava.png">



(<a href="#table-of-contents">back to top</a>)

---

<!-- HOW TO CONTRIBUTE -->
<h2>
<a id="ten" href="#ten" aria-hidden="true"></a>
How to Contribute
</h2>

[![Contributors](https://img.shields.io/github/contributors/LeDuble/Git-Etiquette)](https://github.com/LeDuble/Git-Etiquette/graphs/contributors)

1. Clone repository and create a new branch: **__`git checkout https://github.com/LeDuble/Git-Etiquette.git -b <insertBranchNameHere>`__**
2. Add changes to your branch
3. Create a Pull Request with descriptive text.
4. Leave a star :star_struck:

Feed back and suggestions are welcome! 

(<a href="#table-of-contents">back to top</a>)

---

<!-- AUTHOR -->
<h2>
<a id="nine" href="#nine" aria-hidden="true"></a>
Author
</h2>

* [LeDuble](https://github.com/LeDuble/)

(<a href="#table-of-contents">back to top</a>)

---

<!-- LICENSE -->
<h2>
<a id="eleven" href="#eleven" aria-hidden="true"></a>
License
</h2>

[![License](https://img.shields.io/badge/license-CC%20BY--SA%204.0-blue)](https://creativecommons.org/licenses/by-sa/4.0/)

You can read the full license [here](https://github.com/LeDuble/Git-Etiquette/blob/master/LICENSE.md)

(<a href="#table-of-contents">back to top</a>)