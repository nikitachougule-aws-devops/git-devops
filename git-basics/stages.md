# 🔄 Stages of Git

Git manages code through three main stages, which represent the lifecycle of your changes:

---

## 1. Working Directory (Untracked Area)

- This is the area where you create, edit, and delete files in your project.

---

## 2. Staging Area (Tracked Area)

- The staging area is where you prepare changes before committing them.
- Files are added using the command: `git add <file-name>`
- Git starts tracking these files
- You can control which changes go into the next commit

---

## 3. Git Directory (Local Repository)

- This is where Git permanently stores your committed changes along with their history.
- Changes are saved using: `git commit -m "your message"`
- Git keeps a complete version history
- You can revert, compare, and track all past changes

## 🔁 Simple Flow

Working Directory (edit) → Staging Area (add) → Local Repository (commit)


## 💡 Summary

- **Working Directory** → Writing notes  
- **Staging Area** → Selecting what to save  
- **Repository** → Saving in permanent record
