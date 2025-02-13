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

我们通过一个机器人的比喻来理解三个仓库间的联系，以及整个Git的工作流。

- **Forking**: When you fork a repository, you create your own copy to work on. 由旗舰店开设分店，就是fork的过程，创建一个自己的副本。

- **Cloning**: After forking, you clone the repository to your local computer. 你想要对机器人模型做出一定的修改，需要实操调试，所以在家里复制了一个机器人来调试。同时为了保证不破坏这个机器人样本，你再创建一个机器人副本，在这上面修改，这就是创建分支。

- **Commits**: Each time you save a change, Git creates a "commit" (a snapshot of your project at that moment).

- **Pushing**: Once you've made changes, push them to your forked repository.
  - Example: Use the command `git push origin <branch-name>` to upload your changes.

- **Pull Requests**: When your changes are ready, submit a Pull Request (PR) to the original repository.
  - Example: The maintainers of the original project will review your changes and decide whether to merge them.

- **merge**: 原始仓库的审核员审核后，会将你的修改合并进去。这时因为我们的修改是在本地进行的，所以很可能在我们修改的过程中，别人也对相同的部分进行了修改，这就会产生冲突。最终怎么合并，由原始仓库管理人员决定。

- **Pull**: 这一步实际上实在创建分支后，每一次修改前，拉取最新的原始仓库到本地，保证你的修改是在最新的版本上进行的。Pull from the remote repository，你可能并不是一次就完成机器人修改，可能今天做两小时，明天做两小时，在你没做的时候，其他人也能通过以上流程对机器人修改，并提交到旗舰店且合并。所以每次编辑前，都要拉取最新的旗舰店模型，在最新的基础上进行修改。这时同样有可能产生冲突，至于是否由最新的覆盖掉，还是保留你自己的修改，由你自己决定。

## 3. How Git Enables Version Control and Collaboration

### Version Control

每一次commit都能够追溯

- Git tracks changes through **commits** and **branches**, enabling version control.

### Collaboration

任何时间、任何地点、任何人都能够对原始仓库进行刚刚那一系列的工作流操作，同时因为各自在各自forked仓库中，各自创建的分支中，所以互不干扰，相互协作。

- GitHub facilitates collaboration through **forking**, **Pull Requests**, and **code reviews**. - This workflow ensures that multiple people can work on the same project without conflicts.

## 4. Why This Workflow Works

- **Isolation**: Each contributor works on their own fork and branches, avoiding conflicts.
- **Transparency**: Every change is tracked, making it easy to see who did what and when.
- **Collaboration**: Pull Requests encourage discussion and review, improving the quality of contributions.

## Next Steps

Now that you understand why Git and GitHub are so powerful, let's dive into **how to use them** with GitHub Desktop in the next section.
