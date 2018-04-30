# **What is Git-workflow**?

## Firstly, consider two functionalities of git.
- tracking changes in computer files
- coordinating work

## A Git-workflow is necessary in the coordinating work.
One project may have several contributers. When they work together remotely, they need a tool to simplify the process. The workflow make this process more efficient and well-organized.

Flow in workflow means that the work goes on fluently and smoothly like waterflow well arranged and in order.

# **Why people like Git-workflow**? 

## Coordinating work aspect

Git-workflow makes the cooperating more efficient and easier. Consider your team are dealing with a big project without git-workflow, and each of you do one part alone. After finished, these seperated parts need to be combined together. This may spend a lot of time, and many problems may occur at once. With git-workflow, the project is combined steps by steps when the project is developing. And it is much easier to solve single problem occured. Also the combination will be more organized with workflow.

## Individual work aspect

Git-workflow enables individuals to work on a project in a more flexiable way. For example, One can realize his/her several different ideas at the same time, and switch to see which is better. 

# ** How does Git-workflow work **?
## Git-workflow provides project branches with different function:
- Master: the main branch
- Develop
- feature branch
- hotfix branch
- release branch

The last three branches will be merge into master or develop branch after finished.

## The merge process
You create a new branch and work on it. After finishing it you send a pull request to the master branch. If your pull request is accepted, the new branch will be merge into the master branch.

## Several kinds of git-workflow
### **Centralized workflow**
Linear workflow. One purpose. Team menbers clone the repository to their local file. And each time they finish a part they deal with the conflicts and merge the branch into master branch. So in most time, there is just one branch.

### **Feature branches workflow**
This kind of workflow is ramose. Each feature has its independent branch, and is updated on this branch. So that the feature developing is isolated. 

Once a feature is finished, programmer will not merge it into master branch immediately. Instead, he/she will send a pull request, which will remind other programmer that this feature is completed. You can also use pull request as a "SOS" to ask your teammate to help you solve some problems in this feature.

That is to say, before branches are merged, the pull request inform your teammate to do the final examination. If there is something wrong or something need more imporvement, they will write a comment to tell you. Then you make some changes. When the feature is good enough, the pull request will be passed. And this feature branch is merged into master branch.

### **Gitflow**
This kind of workflow is much more complicated. It provides independent branches for **feature developing**, **release preparing** and **maintaining**. It provides a framwork to manage a rubust big project.

The "master" branch is used to release product. Add a "develop" branch to do the job that "master" branch does in the feature branches workflow. Then two more branches are add. One is "Release" branch, which is used to do release preparation. Once the preparation is over, the product will be tagged and merged to "master" branch as new version. Another is "hotfix" branch, whose functionality is to put a patch to production releases. After fixing bugs, this branch will be merged into "master" branch and "develop" branch.

### **Forking workflow**
Compared to those above, this kind of workflow is essential different. In this workflow, one project has two repository. One is public on the sever, and another is private. This enables a huge scale of collaboration in safe environment. Even distrusted third-party can contribute. 

Firstly, developer has a formal repository open on the server. If a programmer want to work on this project and want to clone this repository to his/her local file, he need to establish a copy of the formal repository on the server and it becomes a private repository. Each push works in this private repository. After finishing it, this programmer send a pull request to the developer. Developer will check it and merge it into his "master" branch and push it onto the formal repository.
