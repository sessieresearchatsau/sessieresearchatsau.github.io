# Git/GitHub
Git is a distributed version control system that tracks changes in source code and other files. It allows multiple people to work on the same project simultaneously without overwriting each other’s work. Every developer has a full copy of the repository, including its history, which makes branching, merging, and reverting changes efficient and reliable. Git is the foundation for most modern collaborative software development workflows.
 
GitHub is a cloud‑based platform built on top of Git. It provides hosting for repositories, collaboration tools (issues, pull requests, project boards), and integrations with CI/CD pipelines. GitHub makes it easy to share code, review contributions, and manage projects in a centralized way. For teams, it’s not just a storage space but also a hub for collaboration and documentation. This is why we use it manage all Sessie research.

When contributing to shared repositories, it’s important to follow the team’s established guidelines. These rules ensure consistency, maintainability, and fairness in how contributions are reviewed and merged. You can find the details in our [Contribution Policy](policy/contribution-policy.md). Always review it before opening a pull request.

## GitHub Desktop and Command Line  
There are two main ways to interact with GitHub repositories:

- **[GitHub Desktop](https://github.com/apps/desktop)**: A graphical client that simplifies common Git tasks like cloning repositories, committing changes, and syncing with remote branches. It’s beginner‑friendly and integrates well with GitHub accounts.  
- **[Command Line](https://git-scm.com/install/)**: Offers full control and flexibility. Here are some common commands:

```bash
# Clone a repository
git clone https://github.com/username/repository.git

# Check repository status
git status

# Stage and commit changes
git add .
git commit -m "Add new feature"

# Push changes to GitHub
git push origin main

# Pull the latest changes
git pull origin main
```

## IDE Integration  
Modern IDEs such as **PyCharm**, **Visual Studio Code**, and **IntelliJ IDEA** provide built‑in Git and GitHub integration. This means you can commit, push, pull, and resolve merge conflicts directly inside your development environment. For teams, this reduces context‑switching and makes version control part of the natural coding workflow.


## Additional Resources
- [Common Git commands | GitLab Docs](https://docs.gitlab.com/topics/git/commands/)
- [Git - Reference](https://git-scm.com/docs)
- [Git Guide](https://github.com/git-guides)
- [Get started with GitHub documentation - GitHub Docs](https://docs.github.com/en/get-started)
- [GitHub Docs](https://docs.github.com/en)
- [GitHub | PyCharm Documentation](https://www.jetbrains.com/help/pycharm/github.html)
