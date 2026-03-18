#  Git Commands

---

## 🔹 git help

Shows a list of all Git commands.

---

## 🔹 git init

Initializes a folder as a new Git repository.

---

## 🔹 ls -a

Lists all files, including hidden files like `.git`.

---

## 🔹 git config --global user.name & user.email

Sets your identity for commits.

git config --global user.name "your Name"

git config --global user.email "your@email.com"

---

## 🔹 git status

Shows the current state of files (tracked, untracked, staged).

---

## 🔹 git add

Moves files to the staging area.

---

## 🔹 git commit

Saves staged changes to the local repository.

`git commit -m "Your commit message"`

---

## 🔹 git log

Displays commit history.

---

## 🔹 git clone

Copies a remote repository to your local machine.

`git clone <repository_url>`

---

## 🔹 git push

Uploads local commits to GitHub.

`git push origin main`

---

## 🔹 Authentication

GitHub requires authentication for push operations.

- Use a **Personal Access Token (PAT)** instead of a password  

---

## 🔹 Store Credentials

Save your credentials locally to avoid repeated login.

`git config --global credential.helper store`

---

## 🔹 git pull

Fetches and merges latest changes from remote repository.

`git pull origin main`

---

## 🔄 Basic Git Workflow

git init

git add .

git commit -m "Initial commit"

git push origin main
