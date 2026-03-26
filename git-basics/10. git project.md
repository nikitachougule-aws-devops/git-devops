# 🚀 Git Production Project

---

## STEP 1: Initialize Project

```bash
mkdir git-production-project
cd git-production-project
git init

```
## STEP 2: Create Base Project Structure

```bash
mkdir app docs
touch README.md app/app.txt docs/workflow.md

```
## Add initial content:

```bash
echo "# Git Production Project" > README.md
echo "Initial app setup" > app/app.txt

```
## STEP 3: First Commit (main branch)

```bash
git add .
git commit -m "chore: initial project setup"

```
## Rename branch to main (if needed):

```bash
git branch -M main

```
## STEP 4: Create Develop Branch

```bash
git checkout -b develop

```
## STEP 5: Create Feature Branch (login)

```bash
git checkout -b feature/login

```
## Make changes:

```bash
echo "Login feature - UI" >> app/app.txt
git add .
git commit -m "feat: add login UI"

echo "Login validation logic" >> app/app.txt
git add .
git commit -m "feat: add login validation"

```
## STEP 6: Merge Feature into Develop

```bash
git checkout develop
git merge feature/login

```
## STEP 7: Create Another Feature (signup)

```bash
git checkout -b feature/signup
echo "Signup feature - UI" >> app/app.txt
git add .
git commit -m "feat: add signup UI"

```
## STEP 8: Create Merge Conflict

```bash
git checkout develop
echo "Updated main app line" > app/app.txt
git add .
git commit -m "chore: update app base"

```
## Now merge signup → conflict

```bash
git merge feature/signup

```
## STEP 9: Resolve Conflict

## Open file → you'll see:

```bash
<<<<<<< HEAD
Updated main app line
=======
Signup feature - UI
>>>>>>> feature/signup

```
## Fix manually:

```bash
Updated main app line
Signup feature - UI

```
## Then:

```bash
git add .
git commit -m "fix: resolve merge conflict between develop and signup"

```
## STEP 10: Demonstrate Rebase

```bash
git checkout feature/signup
git rebase develop

```

## STEP 11: Interactive Rebase (Clean History)

```bash
git rebase -i HEAD~2

```
## STEP 12: Simulate Wrong Commit

```bash
echo "Wrong change" >> app/app.txt
git add .
git commit -m "bad commit"

```
## STEP 13: Undo Using Reset (Local)

```bash
git reset --soft HEAD~1

```
## STEP 14: Recommit Properly

```bash
git commit -m "fix: correct previous mistake"

```
## STEP 15: Simulate Pushed Mistake (Use Revert)

```bash
git revert HEAD

```
## STEP 16: Recover Lost Commit (Reflog)

```bash
git reflog

Then:

```bash
git checkout -b recovery-branch <commit-hash>

```
## STEP 17: Create Release Tag


```bash
git checkout main
git merge develop
git tag v1.0.0

```
## STEP 18: Push to GitHub

```bash
git remote add origin <your-repo-url>
git push -u origin main
git push origin develop
git push origin --tags

```
## STEP 19: Add Documentation Files

```bash
touch docs/branching-strategy.md
touch docs/conflict-resolution.md
touch PR-examples.md
touch commits-history.md
touch tags-and-releases.md

```
## Commit:

```bash
git add .
git commit -m "docs: add project documentation"

```
## FINAL RESULT

- Multiple branches (main, develop, feature/*)

- Feature development workflow

- Merge conflicts (resolved)

- Rebase + interactive rebase

- Reset, revert, reflog usage

- Tags & releases

- Real commit history

