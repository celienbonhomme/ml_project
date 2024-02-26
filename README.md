# ML project

## Virtual Environment
Use the following command in your terminal to activate the Conda environment:

```bash
conda activate name_of_the_environment
```

## Trello Board
[Trello](https://trello.com/b/dKmqPYaQ/mlproject) is a tool for organizing and managing tasks related to our machine learning project. Here's how we can use it effectively:

#### Lists and Cards

- **To Do:** Contains tasks that need to be done.
- **In Progress:** Contains tasks that are currently being worked on.
- **Testing:** Contains tasks that are ready for testing.
- **Done:** Contains tasks that have been completed.

Each task is represented by a card, which can be moved between lists as it progresses through the workflow.

## Git shortcuts
To simplify common Git commands, you can set up shortcuts using aliases in your Git configuration.

1. Open your terminal.

2. Run the following commands to set up the aliases:

   ```bash
   git config --global alias.st status
   git config --global alias.co checkout
   git config --global alias.br branch
   ```

## Git strategy

#### Using the `dev` Branch

In this project, we use a `dev` branch as an intermediary branch between the `master` branch and feature branches. The `dev` branch serves as a staging area for features before they are merged into the master branch. Here's how we use the `dev` branch:

1. **Merging into `dev`:** Once the feature is complete and tested, merge it into the `dev` branch using `git checkout dev` followed by `git merge feat/new-feature`.

2. **Testing:** Test the merged features in the `dev` branch to ensure they work correctly together.

3. **Merging into `master`:** When the `dev` branch contains a set of features ready for release, merge `dev` into `master` using `git checkout master` followed by `git merge dev`.


#### Creating a New Feature Branch

When starting work on a new feature, follow these steps to create a new branch:

1. **Create the Branch:** Use the command `git checkout -b feat/new-feature-name` to create a new branch for your feature

2. **Work on Your Feature:** Make your changes and commits on this branch. Remember to commit often and write clear, descriptive commit messages.

3. **Push Your Branch:** Once your feature is complete and tested locally, push your branch to the remote repository using `git push origin feat/new-feature-name`.



## Commit Message Conventions
Each commit should start with a prefix indicating the nature of the change, followed by a concise description of the change.

- **feat:** for adding new features to the project.
- **fix:** for bug fixes.
- **docs:** for documentation changes.
- **style:** for changes that do not affect the meaning of the code (formatting, spaces, etc.).
- **refactor:** for code changes that neither fix a bug nor add a feature.
- **test:** for adding or modifying tests.
- **chore:** for maintenance tasks, dependency updates, etc.

## Git Commands

#### Local Changes

- **git status:** Check the status of your working directory and staging area.
- **git add <file>:** Add a file to the staging area.
- **git commit -m "Message":** Commit changes with a descriptive message.
- **git diff:** Show changes between commits, the staging area, and the working directory.

#### Branching

- **git branch:** List all branches in the repository.
- **git branch <branch-name>:** Create a new branch.
- **git checkout <branch-name>:** Switch to a branch.
- **git merge <branch>:** Merge a branch into the current branch.

#### Remote Repositories

- **git push <remote> <branch>:** Push local changes to a remote repository.
- **git pull <remote> <branch>:** Fetch and merge changes from a remote repository.

#### History

- **git log:** Display the commit history.
- **git log --oneline:** Display the commit history in one line per commit.
- **git checkout <commit>:** Check out a specific commit.

#### Undoing Changes

- **git reset <file>:** Unstage a file.
- **git revert <commit>:** Create a new commit that undoes a previous commit.
