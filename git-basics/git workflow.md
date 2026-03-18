# 🔄 Basic Git Workflow

A **basic Git workflow** is the standard sequence developers follow to track changes, collaborate, and manage code safely.


```
git checkout -b feature-branch   # Create branch
# make changes
git add .                        # Stage changes
git commit -m "message"          # Commit
git pull origin main             # Sync with latest code
git push origin feature-branch   # Push to remote

🎯 Flow

Create Branch → Add → Commit → Pull → Push → PR → Merge
