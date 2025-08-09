# How to Synchronize a Local Folder with a GitHub Repository

Follow these steps to keep a folder on your computer in sync with a GitHub repository.

## 1. Install Git

If you haven’t already, [download and install Git](https://git-scm.com/downloads) for your operating system.

## 2. Clone the Repository (First Time Only)

If you haven’t cloned the repository yet:

```sh
git clone https://github.com/your-username/your-repository.git
```

Replace `your-username` and `your-repository` with the appropriate values. This creates a folder named after the repository and connects it to GitHub.

## 3. Navigate to Your Local Repo Folder

```sh
cd your-repository
```

## 4. Make Changes Locally

Edit, add, or delete files within the folder as needed.

## 5. Check Repository Status

See what’s changed:

```sh
git status
```

## 6. Stage and Commit Your Changes

Add all changed files:

```sh
git add .
```

Commit with a message:

```sh
git commit -m "Describe your changes"
```

## 7. Pull the Latest Changes from GitHub

Before pushing, make sure you have the latest updates from GitHub:

```sh
git pull origin main
```

> Replace `main` with your branch name if it’s different.

## 8. Push Your Changes to GitHub

```sh
git push origin main
```

## 9. Repeat Steps 4–8 as Needed

Continue making changes, committing, pulling, and pushing to keep your local folder and the GitHub repository in sync.

---

### Additional Tips

- To synchronize with a different branch, replace `main` with the branch name.
- If you get merge conflicts when pulling, resolve them locally, then add, commit, and push again.
- To see which remote repositories are connected:

  ```sh
  git remote -v
  ```

- To add a new remote (if you cloned manually):

  ```sh
  git remote add origin https://github.com/your-username/your-repository.git
  ```

---

**For more information, see the [GitHub Docs: Syncing your branch](https://docs.github.com/en/get-started/using-git/syncing-your-branch).**