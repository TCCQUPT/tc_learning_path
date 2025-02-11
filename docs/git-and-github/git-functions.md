# Why We Use Git & GitHub

We've already talked about that Git and GitHub are the foundation of Docs-like-code workflow. To understand why they are so powerful, let's break down how they work and how they enable version control and collaboration. In the first, we need to know the concept of the repository in Git.

## 1. The Three Layers of Git: Remote, Forked, and Local repositories

Git operates across three main layers:

1. **The Original Repository (Remote)**

    This is the main project hosted on GitHub (e.g., a popular open-source project like VS Code).

    - You can view the code and documentation, but you **can't directly edit it**.
    - To contribute, you need to create your own copy.

2. **Your Forked Repository (Remote)**

    Forking creates a **personal copy** of the original repository under your GitHub account.

    - This is where you can freely make changes without affecting the original project.
    - Think of it as your own "sandbox" to experiment and contribute.

3. **Your Local Repository**

    This is the copy of the repository on your computer.

    - You can edit files, test changes, and commit updates here.
    - Once you're happy with your changes, you can push them back to your forked repository.

Then how the three layers enable git achieve version control and collaboration. To understand it, we need to know previously the total workflow of Git and GitHub, as well as some terms.

## 2. The workflow of Git

- **Forking**: When you fork a repository, you create your own copy to work on.
  - Example: You fork a documentation project to add a new section.

- **Cloning**: After forking, you clone the repository to your local machine.
  - Example: Use the command `git clone <repository-url>` to download the repository to your computer.

- **Pull**: Pull from the remote repository

- **Branching**: Create a new branch for each task or feature.
  - Example: Create a branch called `add-tutorial` to write a new tutorial.

- **Commits**: Each time you save a change, Git creates a "commit" (a snapshot of your project at that moment).
  - Commits are like checkpoints in a video game—you can always go back to them if something goes wrong.
  - Example: If you accidentally delete a file, you can revert to a previous commit to restore it.

- **Pushing**: Once you've made changes, push them to your forked repository.
  - Example: Use the command `git push origin <branch-name>` to upload your changes.

- **Pull Requests**: When your changes are ready, submit a Pull Request (PR) to the original repository.
  - Example: The maintainers of the original project will review your changes and decide whether to merge them.

## 3. How Git Enables Version Control and Collaboration

### Version Control

每一次commit都能够追溯

### Collaboration

任何时间、任何地点、任何人都能够对原始仓库进行刚刚那一系列的工作流操作，同时因为各自在各自forked仓库中，各自创建的分支中，所以互不干扰，相互协作。

## 4. Why This Workflow Works

- **Isolation**: Each contributor works on their own fork and branches, avoiding conflicts.
- **Transparency**: Every change is tracked, making it easy to see who did what and when.
- **Collaboration**: Pull Requests encourage discussion and review, improving the quality of contributions.

## Key Takeaways

- Git tracks changes through **commits** and **branches**, enabling version control.
- GitHub facilitates collaboration through **forking**, **Pull Requests**, and **code reviews**.
- This workflow ensures that multiple people can work on the same project without conflicts.

## Next Steps

Now that you understand why Git and GitHub are so powerful, let's dive into **how to use them** with GitHub Desktop in the next section.
