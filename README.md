## Version control
* Version control is the process of tracking and managing changes to software code
* Changes made to files/code are recorded, so that specific versions can be recalled later on if needed
* If a new version of a piece of software is causing major issues, version control can be used to roll back to a previously saved iteration.
## Git
* Git is a version control system that allows users to manage and keep track of source code history
* Git is a DVCS (Distributed Version Control System)
* Rather than have one location where the full history of the coed is stored, git allows for copies of code to be made into a full repository which contains the full history of changes.
### Benefits of git- Performance
* Committing new changes, branching, merging and comparing past versions are all optimized for performance
* Git isn't fooled by file names when determining storage and version history of the file tree. It focuses on content 
* This is useful as files are often renamed, split and rearranged 
* Git is `distributed`, meaning each iteration/version can be stored and worked on separately without internet access, and changes can be `pushed` when deemed appropriate.
### Benefits of git- Security
* Intergrity of managed source code is a priority
* The content of the files as well as the true relationships between files and directories, versions, tags and commits, all of these objects in the Git repository are secured with a cryptographically secure hashing algorithm called SHA1
* This protects the code and the change history against both accidental and malicious change and ensures that the history is fully traceable.
### Benefits of git- Flexibility
* `Git` supports various kinds of non linear work flows 
* `Git` is efficient in small and large projects
* `Git` is compatible with many existing systems and protocols
### Benefits of git- Branch workflow
* Branches provide an isolated environment for every change to the codebase -> new branches are created when working on new features to make sure the `main` branch has production-quality code
* `Git` branches are cheap and easy to merge
### Benefits of git- Distributed development
* Instead of giving developets a working copy, git allows for local repositories with a complete history of commits 
* This increases the speed of git due to not needing a network connection to create `commits`, inspect previous versions of a file, or perform difference checks between `commits`
* Distributed development minimises the impact of breaks -> if the production branch is broken in a centrilised system then other developers can't check in changes until this is fixed. With git, developers can continue working in local repositories
* With git, if someone accidentally deletes their repository, they can clone someone elses and continue
### Benefits of git- Pull requests
* `Pull requests` are a way to ask a developer to merge one of your branches into their repository 
* Makes it easier for project leads to keep track of changes, and discuss changes before integrating into codebase
* `Pull requests` can be used to ask for help from the rest of the team
* For junior developers, `pull requests` can be seen as code reviews which make sure that their code will not break the system
### Benefits of git- Popular
* Because git is so widely used, companies dont have to train new hires on their workflow
* `Git` is open source, making it easier to use third party librariesand other peoples code in general if they have solved a problem which yu have.
### Benefits of git- Summary
* The aforementioned benefits of `git` all contribute to an overal faster release cycle. `Git` functionality encourages developers to work within the `agile` mindset by making it easy to make small, iterative changes to code bases more frequantly. 
* `Git` supports `CI/CD`, by runnign scripts which occur when certain events occur inside a repository.
* For example, `git` can be used to deploy the most recent commit from the develop branch to a test server whenever anyone merges a pull request into it
## Git basic commands

![](git.png)

* `git init <directory>` - Create an empty `git` repository in the specified directory. Running no arguments initialises the current directory as a git repository
* `git clone <repository>` - Clone specifiec repository onto local machine 
* `git config user.name <name>` - Define author name to be used for all `commits` in current repository. The `-- global` flag can be used to set the uesr for every repository on the machine
* `git add <directory>` - Stages all changes in specifed directory to be committed. Can either specify a `file` or `.` to stage all changes in the repository
* `git commin -m <message>` - Commit the staged snapshot with a descriptive message about the changes.
* `git status` - Lists which files are staged, unstaged and untracked
* `git push -u <remote> <branch>` - Send all committed changes to the specified remote branch of the repository. If the remote repository doesnt exit, a named branch is created.
* `git pull <remote>` - Fetch the specified remote's copy of the current branch and immediatly merge it into the local copy.
* `git checkout -b <branch>` - Create and checkout a new branch . Taking away the `-b` flag will checkout the specified branch

**Checkout means to switch between different versions of a target entity** 

