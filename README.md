# Commonly Used Git Commands for Version Control and Deployment

This document lists 50 commonly used Git commands, categorized by their functionality, along with a brief description of each command.

---

## 1. Repository Initialization
1. **`git init`**  
   Initialize a new Git repository.

2. **`git clone <repo_url>`**  
   Clone an existing repository into a local folder.

3. **`git remote add <name> <url>`**  
   Add a remote repository URL.

---

## 2. Configuration
4. **`git config --global user.name "Your Name"`**  
   Set the global username for commits.

5. **`git config --global user.email "you@example.com"`**  
   Set the global email for commits.

6. **`git config --global core.editor "code --wait"`**  
   Set the default editor for Git (e.g., VS Code).

7. **`git config --list`**  
   View all Git configurations.

8. **`git config --global --edit`**  
   Edit global configuration settings.

---

## 3. Staging and Committing
9. **`git status`**  
   Show the current status of the working directory.

10. **`git add <file>`**  
    Stage a specific file for commit.

11. **`git add .`**  
    Stage all changes in the directory.

12. **`git commit -m "message"`**  
    Commit staged changes with a message.

13. **`git commit -a -m "message"`**  
    Stage and commit all changes in one step.

14. **`git commit --amend -m "updated message"`**  
    Edit the last commit message.

---

## 4. Branching
15. **`git branch`**  
    List all branches.

16. **`git branch <branch_name>`**  
    Create a new branch.

17. **`git checkout <branch_name>`**  
    Switch to an existing branch.

18. **`git checkout -b <branch_name>`**  
    Create and switch to a new branch.

19. **`git branch -d <branch_name>`**  
    Delete a branch locally.

20. **`git branch -m <old_name> <new_name>`**  
    Rename a branch.

21. **`git merge <branch_name>`**  
    Merge a branch into the current branch.

22. **`git rebase <branch_name>`**  
    Rebase the current branch onto another branch.

---

## 5. Remote Repositories
23. **`git fetch`**  
    Fetch updates from the remote repository.

24. **`git pull`**  
    Fetch and merge changes from the remote repository.

25. **`git push origin <branch_name>`**  
    Push a local branch to the remote repository.

26. **`git push -u origin <branch_name>`**  
    Push a branch and set upstream for future pulls.

27. **`git push origin --delete <branch_name>`**  
    Delete a branch from the remote repository.

28. **`git remote -v`**  
    List remote repository URLs.

29. **`git remote set-url origin <new_url>`**  
    Update the URL of the remote repository.

---

## 6. Viewing History
30. **`git log`**  
    Show commit history.

31. **`git log --oneline`**  
    Show commit history in one line per commit.

32. **`git log --graph`**  
    Show branch and commit history visually.

33. **`git show <commit_hash>`**  
    Show details of a specific commit.

34. **`git diff`**  
    Show unstaged changes.

35. **`git diff --cached`**  
    Show staged changes.

36. **`git blame <file>`**  
    Show who last modified each line of a file.

---

## 7. Undoing Changes
37. **`git reset <file>`**  
    Unstage a file.

38. **`git reset --hard <commit_hash>`**  
    Reset the repository to a specific commit.

39. **`git checkout -- <file>`**  
    Discard changes in a specific file.

40. **`git revert <commit_hash>`**  
    Create a new commit to reverse changes of a specific commit.

41. **`git clean -f`**  
    Remove untracked files.

---

## 8. Tags
42. **`git tag`**  
    List all tags.

43. **`git tag -a <tag_name> -m "message"`**  
    Create an annotated tag.

44. **`git push origin <tag_name>`**  
    Push a tag to the remote repository.

45. **`git tag -d <tag_name>`**  
    Delete a tag locally.

46. **`git push origin --delete <tag_name>`**  
    Delete a tag from the remote repository.

---

## 9. Deployment
47. **`git stash`**  
    Save changes temporarily.

48. **`git stash pop`**  
    Reapply stashed changes.

49. **`git cherry-pick <commit_hash>`**  
    Apply a specific commit to the current branch.

50. **`git archive --format=zip HEAD > archive.zip`**  
    Create a zip file of the current repository version.

---

This list covers most commands necessary for Git version control and deployment workflows. Let me know if you need a deeper dive into any specific category!
