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

We use a robot metaphor to understand the relationships between three repositories and the entire Git workflow.

- **Forking**: When you fork a repository, you create your own copy to work on.
  - Creating a branch store by the flagship store is the process of forking, making a copy of your own.

- **Cloning**: After forking, you clone the repository to your local computer.
  - To modify the robot model, you need hands-on debugging. You copy a robot to your home for adjustments. To avoid damaging the original robot sample, you create a duplicate robot to modify — this is creating a branch.

- **Commits**: Each time you save a change, Git creates a "commit" (a snapshot of your project at that moment).
  - Every time you make a modification (e.g., adjusting the robot’s arm), you take a "snapshot" of your changes. This snapshot is a commit.

- **Pushing**: Once you've made changes, push them to your forked repository.
  - After finalizing your robot’s arm design, you ship the modified robot back to your branch store. This is pushing your changes.

- **Pull Requests**: When your changes are ready, submit a Pull Request (PR) to the original repository.
  - Example: The maintainers of the original project will review your changes and decide whether to merge them.
  - You submit a design proposal to the flagship store, asking them to incorporate your arm design into their official model. This is a pull request.

- **merge**: The original repository’s maintainers review your changes and decide whether to merge them.
  - While you were modifying your local copy, others might have changed the same part of the robot, causing conflicts. The final decision on how to merge the changes lies with the flagship store’s managers.

- **Pull**: Before every time starting new modifications, always pull the latest version from the original repository to ensure your work is based on the newest updates.
  - You might not finish modifying the robot in one go (e.g., working two hours today and two tomorrow). While you’re paused, others might modify and merge their changes into the flagship store’s model. Before editing again, always pull the latest model from the flagship store to avoid conflicts. You can choose whether to overwrite your changes with the latest version or keep your modifications.

## 3. How Git Enables Version Control and Collaboration

### Version Control

Git tracks changes through commits and branches, enabling precise version control. Each commit records who made the change, when it was made, and a description of the modifications.

### Collaboration

Anyone can contribute to the original repository from anywhere, at any time. By working in their own forked repositories and branches, collaborators avoid interference and enable parallel development.

## Next Steps

Now that you understand why Git and GitHub are so powerful, let's dive into **how to use them** with GitHub Desktop in the next section.
