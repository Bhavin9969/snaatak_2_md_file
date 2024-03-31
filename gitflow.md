
![git](https://github.com/Bhavin9969/snaatak_2_md_file/assets/164474264/67aa546c-4643-43ef-8f13-73f8581e1883)

| Author | Created on | Version | Last updated by | Last edited on |
| ------ | ---------- | ------- | --------------- | -------------- |
| Bhavin    | 28-03-24   | version 1 | Bhavin         | 31-03-24       |

| Table of content|
| --------------- |
| 1. [Introduction](#intoduction)
| 2. [Purpose](#purpose)
| 3. [Enhancement of GitFlow](#enhancement-of-gitflow)
| 4. [Advantages](#advantages)
| 5. [Disadvantages](#disadvantages)
| 6. [Conclusion](#conclusion)
| 7. [Contact Information](#contact-information)
| 8. [Reference](#reference)

# Intoduction

- Gitflow is a popular Git branching strategy aimed at simplifying release management. And Gitflow is an alternative Git branching model that involves the use of supporting branches and multiple primary branches. It was first published and made popular by **Vincent Driessen**. Git flow involves isolating your work into different types of Git branches.

# Purpose

- Fundamentally, It is provide a structured approach to managing code branches, particularly in projects with longer development cycles and multiple contributors. In this article, we’ll cover the different branches in the Git flow workflow.

# Git Flow

![all](https://github.com/Bhavin9969/snaatak_2_md_file/assets/164474264/1c265178-1789-469f-8007-c65136478c5f)

## Enhancement of GitFlow Branches
    
![main](https://github.com/Bhavin9969/snaatak_2_md_file/assets/164474264/78beda67-d68c-47dc-b5ed-0e9f35641ddb)


- The central repo holds two main branches with an infinite lifeline, first one is "main" and another is "develop". First, let's talk about "main" branch, so The main branch should be familiar to every Git user. The **main** branch stores the official release history/production ready code. The main branch is created at the start of a project and is maintained throughout the development process and we consider **main** to be the main branch where the source code of head always reflects a production-ready state.
<br>
<br>

![develop](https://github.com/Bhavin9969/snaatak_2_md_file/assets/164474264/c4317f64-9b64-4fd8-8826-1f64ed535328)


- And another main branch is "develop", and the **develop** branch serves as an integration branch for festures. The develop branch is created at the start of a project and is maintained throughout the development process, and contains pre-production code with newly developed features that are in the process of being tested. And we consider "develop" to be the main branch where the source code of head always reflects a state with the latest delivered development changes for the next release. And when the source code in the **develop** branch reaches a stable point and is ready to be released, all of the changes should be merged back into **master** and then tagged with a release number.
<br>
<br>

![feature](https://github.com/Bhavin9969/snaatak_2_md_file/assets/164474264/81a10d79-6e1f-4c87-a034-cf90915361a4)


- The "feature" branch is the most common type of branch in the Git flow. It is used when working on a new feature or change, developers create a new branch ( feature ) off the **develop** branch. They make their changes in this feature branch and test them locally. **Feature** branch will merge to their parent 'develop' branch, instead of merging to 'main' branch. Means when a feature is complete, it gets merged back into **develop**, feature should never interact directly with **main**.
<br>
<br>

![release](https://github.com/Bhavin9969/snaatak_2_md_file/assets/164474264/271f6c6e-eee5-44ec-b904-454320d7d096)

- To understand "Release" branch, we can say - when it's time to prepare a new release, a release branch is created from the " develop " branch. and The branch is typically named 'release/a.b.c', where 'a.b.c' is the version number of the release. The code in the **release** branch is tested thoroughly to ensure that it meets the quality standards for release. This may include running automated tests, performing manual testing, and checking for compatibility with different environments. And once the code in the release branch is deemed ready for release, ( any final adjustments or documentation updates are made here. ) the release is then prepared for deployment to production, and once it's ready to ship, the **release** branch gets merged into **main** and tagged with a version number. In addition, it should be merged back into **develop**, which may have progressed since the release was initiated.

- It helps to separate the release process from ongoing development work, making it easier to manage the release process and track changes in the codebase.
<br>

![hotfix](https://github.com/Bhavin9969/snaatak_2_md_file/assets/164474264/9084b97d-724f-4fc6-b992-f53013a5a2a9)

- "Hotfix" branches are used to quickly patch production releases. **Hotfix** branches are a lot like **release** and **feature** branches except they're based on **main** instead of **develop**. Having a dedicated line of development for bug fixes from **main** lets your team address issues without interrupting. Means the **hotfix** branch is used to quickly address necessary changes in your main branch. Inshort, the **hotfix** branch provides a quick and controlled way to address critical issues in the production code (**main**), ensuring that urgent problems can be fixed and deployed without disrupting ongoing development work. ( If a bug is found in the **main** branch, we create a new branch to fix that bug to avoid interrupting other branches. )



# Advantages
| No.                   | Advantages                                                                                                     |
|---------------------------|-----------------------------------------------------------------------------------------------------------------|
| **1** | Using multiple separate branches in Git will provide flexibility. |
| **2** | Gitflow makes developer speed up the process with familiar branch structure. |
| **3** | It keep repository & process clean and tidy. |
| **4** | Easy bug tracking because each feature or bugfix is developed in its own branch, it's easier to track changes and identify the source of bugs. |

# Disadvantages
| No.                   | Disadvantages                                                                                                     |
|---------------------------|-----------------------------------------------------------------------------------------------------------------|
| **1** | Using multiple separate branches in Git will gets complex at sometimes. |
| **2** | With multiple branches being worked on simulraneously, there is a higher risk of merge conflivts, which can slow down development. |

# Conclusion


- GitFlow is a powerful branching model and workflow for Git that helps teams manage their codebase more effectively. It provides a clear and organinzed structure for branching, allowing for parallel development, stable releases, and easy bug tracking. While **git flow** may not be suitable for all projects or teams, especially those with simpler development processes or smaller team sizes but its flexibility and adaptability make it a valuable tool for managing complex development workflows and collaborating on software projects.

## Contact Information
|Name	|Email address |
| --------------- | -------------- |
|Bhavin|	[bhavin.panchal.snaatak@mygurukulam.co](https://www.gmail.com/)|

## Reference
|Description	|link|
| :---------------: | :--------------: |
| Gitflow workflow | https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow |
| What is Gitflow | https://www.gitkraken.com/learn/git/git-flow |
