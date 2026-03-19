# 🔀 Pull Request (PR) Workflow

## Pull Request

In professional environments, merging is almost never done directly.

A **Pull Request (PR)**:

- Is a formal request to merge one branch into another  
- Triggers:
  - Code review by teammates  
  - Automated tests (CI/CD pipelines)  
- Acts as a discussion and quality-control checkpoint  

---

## 🔄 Typical PR Lifecycle

1. Developer pushes branch to remote (e.g., GitHub/GitLab)  
2. Opens a PR targeting `main`  
3. Reviewers:
   - Comment on code  
   - Request changes if needed  
4. Once approved and checks pass:
   - PR is merged  
   - Branch is often deleted  

---

## 💻 In Practice

```bash
git checkout -b feature/new-feature
# make changes
git add .
git commit -m "Add new feature"
git push origin feature/new-feature
# open PR on GitHub
