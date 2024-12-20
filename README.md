#### Git Commands Practise

PS C:\Users\Gautam\Desktop\GitHub\Git-Work> 
 *  History restored 

PS C:\Users\Gautam\Desktop\GitHub> git config --global user.email "gautamcholkar36@gmail.com"  
PS C:\Users\Gautam\Desktop\GitHub> cd Git-Work
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git config --global user.name "Gautam"
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git config --global user.email "gautamcholkar36@gmail.com" 
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git config --global core.editor "code --wait"               
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git config --list
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
http.sslcainfo=C:/Program Files/Git/mingw64/etc/ssl/certs/ca-bundle.crt
core.autocrlf=true
core.fscache=true
core.symlinks=false
pull.rebase=false
credential.helper=manager
init.defaultbranch=master
user.name=Gautam
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git config --global --edit
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git config --global --list
user.name=Gautam Cholkar
core.editor=code --wait
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git status
On branch main
Your branch is up to date with 'origin/main'.
nothing to commit, working tree clean
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git add example.py
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git add .
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git commit -m "Added a simple python code"
[main 3de67b3] Added a simple python code
 1 file changed, 13 insertions(+)
 create mode 100644 example.py
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git commit -a -m "Initial Updates"
Your branch is ahead of 'origin/main' by 1 commit.
nothing to commit, working tree clean
[main 8737f22] updated message
 1 file changed, 13 insertions(+)
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git push origin main
Enumerating objects: 4, done.
Delta compression using up to 8 threads
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
   1eb770b..8737f22  main -> main
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git branch
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git branch new_branch
Switched to branch 'new_branch'
Switched to a new branch 'new2_branch'
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git branch -d new2_branch
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git checkout main
Your branch is up to date with 'origin/main'.
Deleted branch new2_branch (was 8737f22).
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git branch -m new_branch sub_branch
* main
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git checkout sub_branch
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git merge s1_branch
merge: s1_branch - not something we can merge
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git checkout main
Switched to branch 'main'
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git merge sub_branch
Already up to date.
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git checkout sub_branch
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git checkout main
Switched to branch 'main'
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git branch feature_branch
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git rebase origin
Current branch main is up to date.
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git rebase --continue
fatal: No rebase in progress?
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git branhc
git: 'branhc' is not a git command. See 'git --help'.

PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git branch
  feature_branch
  sub_branch
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git checkout main
Already on 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git checkout sub_branch
Switched to branch 'sub_branch'
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git status
On branch sub_branch
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   example.py

PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git add example.py
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git commit -m "Updated code in example.py with new Logic"       
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git push -u origin sub_branch
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 1.06 KiB | 1.06 MiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote:      https://github.com/Gautam2901/Git-Work/pull/new/sub_branch
remote:
To https://github.com/Gautam2901/Git-Work.git
branch 'sub_branch' set up to track 'origin/sub_branch'.
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git checkout main
Your branch is up to date with 'origin/main'.
PS C:\Users\Gautam\Desktop\GitHub\Git-Work>
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git pull origin main
Already up to date.
Updating 8737f22..5fcb8cb
 example.py | 60 +++++++++++++++++++++++++++++++++++++++++++++++-------------
 1 file changed, 47 insertions(+), 13 deletions(-)
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git push origin main
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Gautam2901/Git-Work.git
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git remote -v
origin  https://github.com/Gautam2901/Git-Work.git (push)
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git branch
  feature_branch
* main
  sub_branch
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git fetch
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git pull
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git push origin main
Everything up-to-date
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git push -u feature_branch
fatal: 'feature_branch' does not appear to be a git repository
fatal: Could not read from remote repository.

and the repository exists.
Switched to branch 'feature_branch'
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git push origin feature_branch
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: Create a pull request for 'feature_branch' on GitHub by visiting:
remote:      https://github.com/Gautam2901/Git-Work/pull/new/feature_branch
remote:
 * [new branch]      feature_branch -> feature_branch
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git pull origin main
 * branch            main       -> FETCH_HEAD
Updating 8737f22..5fcb8cb
Fast-forward
 1 file changed, 47 insertions(+), 13 deletions(-)
Already up to date.
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git branch
* feature_branch
  main
  sub_branch
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git pull origin main
 * branch            main       -> FETCH_HEAD
Already up to date.
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git checkout main
Your branch is up to date with 'origin/main'.
From https://github.com/Gautam2901/Git-Work
 * branch            main       -> FETCH_HEAD
Already up to date.
Already up to date.
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git pull origin main
From https://github.com/Gautam2901/Git-Work
 * branch            main       -> FETCH_HEAD
Fast-forward
 example.py | 2 +-
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git branch
  feature_branch
* main
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git rebase origin
Current branch main is up to date.
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git branch
  feature_branch
* main
  sub_branch
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git push -u origin feature_branch
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Gautam2901/Git-Work.git
   8737f22..5fcb8cb  feature_branch -> feature_branch
branch 'feature_branch' set up to track 'origin/feature_branch'.
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git push origin --delete feature_branch
To https://github.com/Gautam2901/Git-Work.git
 - [deleted]         feature_branch
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git remote -v
origin  https://github.com/Gautam2901/Git-Work.git (fetch)
origin  https://github.com/Gautam2901/Git-Work.git (push)
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git remote set -url origin https://github.com/Gautam2901/Git-Work.git
   or: git remote add [-t <branch>] [-m <master>] [-f] [--tags | --no-tags] [--mirror=<fetch|push>] <name> <url>
   or: git remote rename [--[no-]progress] <old> <new>
   or: git remote remove <name>
   or: git remote set-head <name> (-a | --auto | -d | --delete | <branch>)
   or: git remote [-v | --verbose] show [-n] <name>
   or: git remote prune [-n | --dry-run] <name>
   or: git remote [-v | --verbose] update [-p | --prune] [(<group> | <remote>)...]
   or: git remote set-branches [--add] <name> <branch>...
   or: git remote get-url [--push] [--all] <name>
   or: git remote set-url [--push] <name> <newurl> [<oldurl>]
   or: git remote set-url --add <name> <newurl>
   or: git remote set-url --delete <name> <url>

    -v, --[no-]verbose    be verbose; must be placed before a subcommand

PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git remote set-url origin https://github.com/Gautam2901/Git-Work.git
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git log
Author: Gautam Cholkar <104461444+Gautam2901@users.noreply.github.com>

    Update example.py

commit 5fcb8cb0579139fb0209fdffbb147b36187e6879 (origin/sub_branch, sub_branch, feature_branch)
Date:   Fri Dec 20 02:35:48 2024 +0530

    Updated code in example.py with new Logic

commit 8737f22bd985a6a843a2479ff2c08b104690478b
Author: Gautam Cholkar <gautamcholkar36@gmail.com>
Date:   Fri Dec 20 01:55:14 2024 +0530

    updated message

commit 1eb770b14e1de4775efa10a18baff1e2f63961a4
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git log --online
fatal: unrecognized argument: --online
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git log --oneline
08d6929 (HEAD -> main, origin/main, origin/HEAD) Update example.py
5fcb8cb (origin/sub_branch, sub_branch, feature_branch) Updated code in example.py with new Logic
8737f22 updated message
1eb770b Initial commit
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git log --graph
| Author: Gautam Cholkar <104461444+Gautam2901@users.noreply.github.com>
| Date:   Fri Dec 20 03:12:03 2024 +0530
|
|
* commit 5fcb8cb0579139fb0209fdffbb147b36187e6879 (origin/sub_branch, sub_branch, feature_branch)
| Author: Gautam Cholkar <gautamcholkar36@gmail.com>
|
|     Updated code in example.py with new Logic
|
| Author: Gautam Cholkar <gautamcholkar36@gmail.com>
| Date:   Fri Dec 20 01:55:14 2024 +0530
|
|     updated message
|
* commit 1eb770b14e1de4775efa10a18baff1e2f63961a4
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git show "Initial update"
Use '--' to separate paths from revisions, like this:
'git <command> [<revision>...] -- [<file>...]'
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git show "Initial commit"
fatal: ambiguous argument 'Initial commit': unknown revision or path not in the working tree.
Use '--' to separate paths from revisions, like this:
'git <command> [<revision>...] -- [<file>...]'
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git show Initial commit
fatal: ambiguous argument 'Initial': unknown revision or path not in the working tree.
Use '--' to separate paths from revisions, like this:
'git <command> [<revision>...] -- [<file>...]'
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git show <commit_hash>
At line:1 char:10
+ git show <commit_hash>
+          ~
The '<' operator is reserved for future use.
    + CategoryInfo          : ParserError: (:) [], ParentContainsErrorRecordException
    + FullyQualifiedErrorId : RedirectionNotSupported
Author: Gautam Cholkar <104461444+Gautam2901@users.noreply.github.com>
Date:   Fri Dec 20 03:12:03 2024 +0530

    Update example.py

diff --git a/example.py b/example.py
index 463ddac..7ac9ca8 100644
--- a/example.py
+++ b/example.py
@@ -44,4 +44,4 @@ for i in range(1, n+1):

 print("The cost of most efficient tour = " + str(ans))

-# This code is contributed by Serjeel Ranjan
\ No newline at end of file
+# This code is contributed by Serjeel Ranjan
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git diff
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git diff --cached
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git blame example.py
5fcb8cb0 (Gautam Cholkar 2024-12-20 02:35:48 +0530  2)
i to j
5fcb8cb0 (Gautam Cholkar 2024-12-20 02:35:48 +0530  4) # this matrix can be calculated for any given graph using
5fcb8cb0 (Gautam Cholkar 2024-12-20 02:35:48 +0530  5) # all-pair shortest path algorithms
5fcb8cb0 (Gautam Cholkar 2024-12-20 02:35:48 +0530  6) dist = [[0, 0, 0, 0, 0], [0, 0, 10, 15, 20], [       
5fcb8cb0 (Gautam Cholkar 2024-12-20 02:35:48 +0530  7)         0, 10, 0, 25, 25], [0, 15, 25, 0, 30], [0, 20, 25, 30, 0]]
5fcb8cb0 (Gautam Cholkar 2024-12-20 02:35:48 +0530  8)
5fcb8cb0 (Gautam Cholkar 2024-12-20 02:35:48 +0530  9) # memoization for top down recursion
5fcb8cb0 (Gautam Cholkar 2024-12-20 02:35:48 +0530 10) memo = [[-1]*(1 << (n+1)) for _ in range(n+1)]       
5fcb8cb0 (Gautam Cholkar 2024-12-20 02:35:48 +0530 11)
5fcb8cb0 (Gautam Cholkar 2024-12-20 02:35:48 +0530 12)
5fcb8cb0 (Gautam Cholkar 2024-12-20 02:35:48 +0530 13) def fun(i, mask):
5fcb8cb0 (Gautam Cholkar 2024-12-20 02:35:48 +0530 14)     # base case
5fcb8cb0 (Gautam Cholkar 2024-12-20 02:35:48 +0530 15)     # if only ith bit and 1st bit is set in our mask,PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git reset example.py
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git reset --hard 1eb770b14e1de4775efa10a18baff1e2f63961a4       
HEAD is now at 1eb770b Initial commit
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git checkout --example.py
error: unknown option `example.py'
usage: git checkout [<options>] <branch>
   or: git checkout [<options>] [<branch>] -- <file>...

    -b <branch>           create and checkout a new branch
    -B <branch>           create/reset and checkout a branch
    -l                    create reflog for new branch
    --[no-]guess          second guess 'git checkout <no-such-branch>' (default)
    --[no-]overlay        use overlay mode (default)
    -q, --[no-]quiet      suppress progress reporting
    --[no-]recurse-submodules[=<checkout>]
                          control recursive updating of submodules
    --[no-]progress       force progress reporting
    -m, --[no-]merge      perform a 3-way merge with the new branch
    --[no-]conflict <style>
                          conflict style (merge, diff3, or zdiff3)
    -d, --[no-]detach     detach HEAD at named commit
                          set branch tracking configuration
    -f, --[no-]force      force checkout (throw away local modifications)
    --[no-]orphan <new-branch>
    --[no-]overwrite-ignore
                          update ignored files (default)
    --[no-]ignore-other-worktrees
                          do not check if another worktree is holding the given ref
    -2, --ours            checkout our version for unmerged files
    -3, --theirs          checkout their version for unmerged files
    -p, --[no-]patch      select hunks interactively
    --[no-]ignore-skip-worktree-bits
                          do not limit pathspecs to sparse entries only
    --[no-]pathspec-from-file <file>
    --[no-]pathspec-file-nul
                          with --pathspec-from-file, pathspec elements are separated with NUL character

PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git revert 1eb770b14e1de4775efa10a18baff1e2f63961a4
[main f4ef59c] Revert "Initial commit"
 1 file changed, 1 deletion(-)
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> qqexit
At line:1 char:1
+ qqexit
+ ~~~~~~
    + CategoryInfo          : ObjectNotFound: (qqexit:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> ^C
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git pull origin main
From https://github.com/Gautam2901/Git-Work
 * branch            main       -> FETCH_HEAD
Merge made by the 'ort' strategy.
 example.py | 47 +++++++++++++++++++++++++++++++++++++++++++++++
 1 file changed, 47 insertions(+)
 create mode 100644 example.py
error: pathspec 'Final Updates' did not match any file(s) known to git
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git add .
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git add example.py
On branch main
  (use "git push" to publish your local commits)
nothing to commit, working tree clean
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git push origin main
Enumerating objects: 6, done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (4/4), 495 bytes | 495.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git branch
  feature_branch
* main
  sub_branch
merge: feature - not something we can merge
Already up to date.
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git branch
  feature_branch
  sub_branch
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git status
On branch main
Your branch is up to date with 'origin/main'.

PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git add .
On branch main
Your branch is up to date with 'origin/main'.

PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git stash
No local changes to save
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git checkout feature_branch
Switched to branch 'feature_branch'
Your branch is based on 'origin/feature_branch', but the upstream is gone.
  (use "git branch --unset-upstream" to fixup)
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git status
On branch feature_branch
Your branch is based on 'origin/feature_branch', but the upstream is gone.
  (use "git branch --unset-upstream" to fixup)

nothing to commit, working tree clean
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git rebase --show-current-patch
fatal: No rebase in progress?
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git log --oneline
5fcb8cb (HEAD -> feature_branch, origin/sub_branch, sub_branch) Updated code in example.py with new Logic   
8737f22 updated message
1eb770b Initial commit
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git diff example.py
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git checkout PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git config user.name "Gautam"
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git config --global user.name "Gautam"
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git config --global user.email "gautamcholkar36@gmail.com"   
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git config --global core.editor "code --wait"
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git config --list
>> diff.astextplain.textconv=astextplain
>> filter.lfs.clean=git-lfs clean -- %f
>> filter.lfs.smudge=git-lfs smudge -- %f
>> filter.lfs.process=git-lfs filter-process
>> filter.lfs.required=true
>> http.sslbackend=openssl
>> http.sslcainfo=C:/Program Files/Git/mingw64/etc/ssl/certs/ca-bundle.crt
>> core.autocrlf=true
>> core.fscache=true
>> core.symlinks=false
>> pull.rebase=false
>> credential.helper=manager
>> credential.https://dev.azure.com.usehttppath=true
>> init.defaultbranch=master
>> user.name=Gautam
>> ...skipping...
>> diff.astextplain.textconv=astextplain
>> filter.lfs.clean=git-lfs clean -- %f
>> filter.lfs.smudge=git-lfs smudge -- %f
>> filter.lfs.process=git-lfs filter-process
>> filter.lfs.required=true
>> http.sslbackend=openssl
>> http.sslcainfo=C:/Program Files/Git/mingw64/etc/ssl/certs/ca-bundle.crt
>> core.autocrlf=true
>> core.fscache=true
>> core.symlinks=false
>> pull.rebase=false
>> credential.helper=manager
>> credential.https://dev.azure.com.usehttppath=true
>> init.defaultbranch=master
>> user.name=Gautam
>> ...skipping...
>> diff.astextplain.textconv=astextplain
>> filter.lfs.clean=git-lfs clean -- %f
>> filter.lfs.smudge=git-lfs smudge -- %f
>> filter.lfs.process=git-lfs filter-process
>> filter.lfs.required=true
>> http.sslbackend=openssl
>> http.sslcainfo=C:/Program Files/Git/mingw64/etc/ssl/certs/ca-bundle.crt
>> core.autocrlf=true
>> core.fscache=true
>> pull.rebase=false
>> credential.helper=manager
>> credential.https://dev.azure.com.usehttppath=true
>> init.defaultbranch=master
>> user.name=Gautam
>> user.email=gautamcholkar36@gmail.com
>> core.editor=code --wait
>> core.bare=false
>> core.symlinks=false
>> core.ignorecase=true
>> user.name=Gautam
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git config --local --list
>> core.repositoryformatversion=0
>> core.filemode=false
>> core.bare=false
>> core.symlinks=false
>> core.ignorecase=true
>> user.name=Gautam
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git config local --list  
>> error: key does not contain a section: local
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git config --local --list
>> core.repositoryformatversion=0
>> core.filemode=false
>> core.bare=false
>> core.logallrefupdates=true
>> core.symlinks=false
>> core.ignorecase=true
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git config --global --list
>> user.name=Gautam
>> user.email=gautamcholkar36@gmail.com
>> core.editor=code --wait
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git status
>> On branch master
>>
>> No commits yet
>>
>> Untracked files:
>>   (use "git add <file>..." to include in what will be committed)
>>         Git-Work/
>> 
>> nothing added to commit but untracked files present (use "git add" to track)
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git add .
>> warning: adding embedded git repository: Git-Work
>> hint: You've added another git repository inside your current repository.
>> hint: Clones of the outer repository will not contain the contents of
>> hint: the embedded repository and will not know how to obtain it.
>> hint: If you meant to add a submodule, use:
>> hint:
>> hint:   git submodule add <url> Git-Work
>> hint:
>> hint: If you added this path by mistake, you can remove it from the
>> hint: index with:
>> hint:
>> hint:   git rm --cached Git-Work
>> hint:
>> hint: See "git help submodule" for more information.
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work>
>>  *  History restored
>>
>> PS C:\Users\Gautam\Desktop\GitHub> git config --global user.email "gautamcholkar36@gmail.com"
>> PS C:\Users\Gautam\Desktop\GitHub> cd Git-Work
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git config --global user.name "Gautam"
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git config --global user.email "gautamcholkar36@gmail.com"   
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git config --global core.editor "code --wait"
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git config --list
>> filter.lfs.smudge=git-lfs smudge -- %f
>> filter.lfs.process=git-lfs filter-process
>> filter.lfs.required=true
>> http.sslcainfo=C:/Program Files/Git/mingw64/etc/ssl/certs/ca-bundle.crt
>> core.autocrlf=true
>> core.fscache=true
>> core.symlinks=false
>> pull.rebase=false
>> credential.helper=manager
>> init.defaultbranch=master
>> user.name=Gautam
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git config --global --edit
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git config --global --list
>> user.name=Gautam Cholkar
>> core.editor=code --wait
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git status
>> On branch main
>> Your branch is up to date with 'origin/main'.
>> nothing to commit, working tree clean
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git add example.py
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git add .
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git commit -m "Added a simple python code"
>> [main 3de67b3] Added a simple python code
>>  1 file changed, 13 insertions(+)
>>  create mode 100644 example.py
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git commit -a -m "Initial Updates"
>> Your branch is ahead of 'origin/main' by 1 commit.
>> nothing to commit, working tree clean
>> [main 8737f22] updated message
>>  1 file changed, 13 insertions(+)
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git push origin main
>> Enumerating objects: 4, done.
>> Delta compression using up to 8 threads
>> Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
>>    1eb770b..8737f22  main -> main
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git branch
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git branch new_branch
>> Switched to branch 'new_branch'
>> Switched to a new branch 'new2_branch'
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git branch -d new2_branch
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git checkout main
>> Your branch is up to date with 'origin/main'.
>> Deleted branch new2_branch (was 8737f22).
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git branch -m new_branch sub_branch
>> * main
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git checkout sub_branch
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git merge s1_branch
>> merge: s1_branch - not something we can merge
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git checkout main
>> Switched to branch 'main'
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git merge sub_branch
>> Already up to date.
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git checkout sub_branch
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git checkout main
>> Switched to branch 'main'
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git branch feature_branch
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git rebase origin
>> Current branch main is up to date.
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git rebase --continue
>> fatal: No rebase in progress?
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git branhc
>> git: 'branhc' is not a git command. See 'git --help'.
>> 
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git branch
>>   feature_branch
>>   sub_branch
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git checkout main
>> Already on 'main'
>> Your branch is up to date with 'origin/main'.
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git checkout sub_branch
>> Switched to branch 'sub_branch'
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git status
>> On branch sub_branch
>> Changes not staged for commit:
>>   (use "git add <file>..." to update what will be committed)
>>   (use "git restore <file>..." to discard changes in working directory)
>>         modified:   example.py
>> 
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git add example.py
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git commit -m "Updated code in example.py with new Logic"    

>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git push -u origin sub_branch
>> Enumerating objects: 5, done.
>> Counting objects: 100% (5/5), done.
>> Compressing objects: 100% (3/3), done.
>> Writing objects: 100% (3/3), 1.06 KiB | 1.06 MiB/s, done.
>> Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
>> remote:
>> remote:      https://github.com/Gautam2901/Git-Work/pull/new/sub_branch
>> remote:
>> To https://github.com/Gautam2901/Git-Work.git
>> branch 'sub_branch' set up to track 'origin/sub_branch'.
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git checkout main
>> Your branch is up to date with 'origin/main'.
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work>
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git pull origin main
>> Already up to date.
>> Updating 8737f22..5fcb8cb
>>  example.py | 60 +++++++++++++++++++++++++++++++++++++++++++++++-------------
>>  1 file changed, 47 insertions(+), 13 deletions(-)
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git push origin main
>> Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
>> To https://github.com/Gautam2901/Git-Work.git
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git remote -v
>> origin  https://github.com/Gautam2901/Git-Work.git (push)
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git branch
>>   feature_branch
>> * main
>>   sub_branch
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git fetch
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git pull
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git push origin main
>> Everything up-to-date
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git push -u feature_branch
>> fatal: 'feature_branch' does not appear to be a git repository
>> fatal: Could not read from remote repository.
>> 
>> and the repository exists.
>> Switched to branch 'feature_branch'
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git push origin feature_branch
>> Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
>> remote: Create a pull request for 'feature_branch' on GitHub by visiting:
>> remote:      https://github.com/Gautam2901/Git-Work/pull/new/feature_branch
>> remote:
>>  * [new branch]      feature_branch -> feature_branch
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git pull origin main
>>  * branch            main       -> FETCH_HEAD
>> Updating 8737f22..5fcb8cb
>> Fast-forward
>>  1 file changed, 47 insertions(+), 13 deletions(-)
>> Already up to date.
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git branch
>> * feature_branch
>>   main
>>   sub_branch
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git pull origin main
>>  * branch            main       -> FETCH_HEAD
>> Already up to date.
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git checkout main
>> Your branch is up to date with 'origin/main'.
>> From https://github.com/Gautam2901/Git-Work
>>  * branch            main       -> FETCH_HEAD
>> Already up to date.
>> Already up to date.
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git pull origin main
>> From https://github.com/Gautam2901/Git-Work
>>  * branch            main       -> FETCH_HEAD
>> Fast-forward
>>  example.py | 2 +-
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git branch
>>   feature_branch
>> * main
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git rebase origin
>> Current branch main is up to date.
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git branch
>>   feature_branch
>> * main
>>   sub_branch
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git push -u origin feature_branch
>> Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
>> To https://github.com/Gautam2901/Git-Work.git
>>    8737f22..5fcb8cb  feature_branch -> feature_branch
>> branch 'feature_branch' set up to track 'origin/feature_branch'.
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git push origin --delete feature_branch
>> To https://github.com/Gautam2901/Git-Work.git
>>  - [deleted]         feature_branch
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git remote -v
>> origin  https://github.com/Gautam2901/Git-Work.git (fetch)
>> origin  https://github.com/Gautam2901/Git-Work.git (push)
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git remote set -url origin https://github.com/Gautam2901/Git-Work.git
>>    or: git remote add [-t <branch>] [-m <master>] [-f] [--tags | --no-tags] [--mirror=<fetch|push>] <name> <url>
>>    or: git remote rename [--[no-]progress] <old> <new>
>>    or: git remote remove <name>
>>    or: git remote set-head <name> (-a | --auto | -d | --delete | <branch>)
>>    or: git remote [-v | --verbose] show [-n] <name>
>>    or: git remote prune [-n | --dry-run] <name>
>>    or: git remote [-v | --verbose] update [-p | --prune] [(<group> | <remote>)...]
>>    or: git remote set-branches [--add] <name> <branch>...
>>    or: git remote get-url [--push] [--all] <name>
>>    or: git remote set-url [--push] <name> <newurl> [<oldurl>]
>>    or: git remote set-url --add <name> <newurl>
>>    or: git remote set-url --delete <name> <url>
>> 
>>     -v, --[no-]verbose    be verbose; must be placed before a subcommand
>> 
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git remote set-url origin https://github.com/Gautam2901/Git-Work.git
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git log
>> Author: Gautam Cholkar <104461444+Gautam2901@users.noreply.github.com>
>> 
>>     Update example.py
>> 
>> commit 5fcb8cb0579139fb0209fdffbb147b36187e6879 (origin/sub_branch, sub_branch, feature_branch)
>> Date:   Fri Dec 20 02:35:48 2024 +0530
>> 
>>     Updated code in example.py with new Logic
>> 
>> commit 8737f22bd985a6a843a2479ff2c08b104690478b
>> Author: Gautam Cholkar <gautamcholkar36@gmail.com>
>> Date:   Fri Dec 20 01:55:14 2024 +0530
>> 
>>     updated message
>> 
>> commit 1eb770b14e1de4775efa10a18baff1e2f63961a4
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git log --online
>> fatal: unrecognized argument: --online
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git log --oneline
>> 08d6929 (HEAD -> main, origin/main, origin/HEAD) Update example.py
>> 5fcb8cb (origin/sub_branch, sub_branch, feature_branch) Updated code in example.py with new Logic        
>> 8737f22 updated message
>> 1eb770b Initial commit
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git log --graph
>> | Author: Gautam Cholkar <104461444+Gautam2901@users.noreply.github.com>
>> | Date:   Fri Dec 20 03:12:03 2024 +0530
>> |
>> |
>> * commit 5fcb8cb0579139fb0209fdffbb147b36187e6879 (origin/sub_branch, sub_branch, feature_branch)        
>> | Author: Gautam Cholkar <gautamcholkar36@gmail.com>
>> |
>> |     Updated code in example.py with new Logic
>> |
>> | Author: Gautam Cholkar <gautamcholkar36@gmail.com>
>> | Date:   Fri Dec 20 01:55:14 2024 +0530
>> |
>> |     updated message
>> |
>> * commit 1eb770b14e1de4775efa10a18baff1e2f63961a4
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git show "Initial update"
>> Use '--' to separate paths from revisions, like this:
>> 'git <command> [<revision>...] -- [<file>...]'
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git show "Initial commit"
>> fatal: ambiguous argument 'Initial commit': unknown revision or path not in the working tree.
>> Use '--' to separate paths from revisions, like this:
>> 'git <command> [<revision>...] -- [<file>...]'
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git show Initial commit
>> fatal: ambiguous argument 'Initial': unknown revision or path not in the working tree.
>> Use '--' to separate paths from revisions, like this:
>> 'git <command> [<revision>...] -- [<file>...]'
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git show <commit_hash>
>> At line:1 char:10
>> + git show <commit_hash>
>> +          ~
>> The '<' operator is reserved for future use.
>>     + CategoryInfo          : ParserError: (:) [], ParentContainsErrorRecordException
>>     + FullyQualifiedErrorId : RedirectionNotSupported
>> Author: Gautam Cholkar <104461444+Gautam2901@users.noreply.github.com>
>> Date:   Fri Dec 20 03:12:03 2024 +0530
>>
>>     Update example.py
>>
>> diff --git a/example.py b/example.py
>> index 463ddac..7ac9ca8 100644
>> --- a/example.py
>> +++ b/example.py
>> @@ -44,4 +44,4 @@ for i in range(1, n+1):
>>
>>  print("The cost of most efficient tour = " + str(ans))
>>
>> -# This code is contributed by Serjeel Ranjan
>> \ No newline at end of file
>> +# This code is contributed by Serjeel Ranjan
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git diff
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git diff --cached
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git blame example.py
>> 5fcb8cb0 (Gautam Cholkar 2024-12-20 02:35:48 +0530  2)
>> i to j
>> 5fcb8cb0 (Gautam Cholkar 2024-12-20 02:35:48 +0530  4) # this matrix can be calculated for any given graph using
>> 5fcb8cb0 (Gautam Cholkar 2024-12-20 02:35:48 +0530  5) # all-pair shortest path algorithms
>> 5fcb8cb0 (Gautam Cholkar 2024-12-20 02:35:48 +0530  6) dist = [[0, 0, 0, 0, 0], [0, 0, 10, 15, 20], [    

>> 5fcb8cb0 (Gautam Cholkar 2024-12-20 02:35:48 +0530  7)         0, 10, 0, 25, 25], [0, 15, 25, 0, 30], [0, 20, 25, 30, 0]]
>> 5fcb8cb0 (Gautam Cholkar 2024-12-20 02:35:48 +0530  8)
>> 5fcb8cb0 (Gautam Cholkar 2024-12-20 02:35:48 +0530  9) # memoization for top down recursion
>> 5fcb8cb0 (Gautam Cholkar 2024-12-20 02:35:48 +0530 10) memo = [[-1]*(1 << (n+1)) for _ in range(n+1)]    

>> 5fcb8cb0 (Gautam Cholkar 2024-12-20 02:35:48 +0530 11)
>> 5fcb8cb0 (Gautam Cholkar 2024-12-20 02:35:48 +0530 12)
>> 5fcb8cb0 (Gautam Cholkar 2024-12-20 02:35:48 +0530 13) def fun(i, mask):
>> 5fcb8cb0 (Gautam Cholkar 2024-12-20 02:35:48 +0530 14)     # base case
>> 5fcb8cb0 (Gautam Cholkar 2024-12-20 02:35:48 +0530 15)     # if only ith bit and 1st bit is set in our mask,PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git reset example.py
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git reset --hard 1eb770b14e1de4775efa10a18baff1e2f63961a4    

>> HEAD is now at 1eb770b Initial commit
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git checkout --example.py
>> error: unknown option `example.py'
>> usage: git checkout [<options>] <branch>
>>    or: git checkout [<options>] [<branch>] -- <file>...
>>
>>     -b <branch>           create and checkout a new branch
>>     -B <branch>           create/reset and checkout a branch
>>     -l                    create reflog for new branch
>>     --[no-]guess          second guess 'git checkout <no-such-branch>' (default)
>>     --[no-]overlay        use overlay mode (default)
>>     -q, --[no-]quiet      suppress progress reporting
>>     --[no-]recurse-submodules[=<checkout>]
>>                           control recursive updating of submodules
>>     --[no-]progress       force progress reporting
>>     -m, --[no-]merge      perform a 3-way merge with the new branch
>>     --[no-]conflict <style>
>>                           conflict style (merge, diff3, or zdiff3)
>>     -d, --[no-]detach     detach HEAD at named commit
>>                           set branch tracking configuration
>>     -f, --[no-]force      force checkout (throw away local modifications)
>>     --[no-]orphan <new-branch>
>>     --[no-]overwrite-ignore
>>                           update ignored files (default)
>>     --[no-]ignore-other-worktrees
>>                           do not check if another worktree is holding the given ref
>>     -2, --ours            checkout our version for unmerged files
>>     -3, --theirs          checkout their version for unmerged files
>>     -p, --[no-]patch      select hunks interactively
>>     --[no-]ignore-skip-worktree-bits
>>                           do not limit pathspecs to sparse entries only
>>     --[no-]pathspec-from-file <file>
>>                           read pathspec from file
>>     --[no-]pathspec-file-nul
>>                           with --pathspec-from-file, pathspec elements are separated with NUL character  
>>
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git revert 1eb770b14e1de4775efa10a18baff1e2f63961a4
>> [main f4ef59c] Revert "Initial commit"
>>  1 file changed, 1 deletion(-)
>>  delete mode 100644 README.md
>> PS C:\Users\Gautam\Desktop\GitHub\Git-Work> qqexit
>> qqexit : The term 'qqexit' is not recognized as the name of a cmdlet, function, script file, or operable 
>> program. Check the spelling of the name, or if a path was included, verify that the path is correct and  
>> try again.
>> At line:1 char:1
>> + qqexit
>> + ~~~~~~
>>     + CategoryInfo          : ObjectNotFound: (qqexit:String) [], CommandNotFoundException
>>     + FullyQualifiedErrorId : CommandNotFoundException
>>
Oops, something went wrong.  Please report this bug with the details below.
Report on GitHub: https://github.com/lzybkr/PSReadLine/issues/new
-----------------------------------------------------------------------
Last 200 Keys:
 v e Space c h a n g e s Space Backspace b e Backspace Backspace Space b e f o r e Space f i x i n g Space r e b a s e " Enter
 g i t Space s t a s h Enter
 g i t Space c h e c k o u t Space f e a t u r e _ b r a n c h Enter
 g i t Space s t a t u s Enter
 g i t Backspace Backspace Backspace Backspace g i t Space r e b a s e Space - - s h o w - c u r r e n t - p g i t Space l o g Space o n e l i n e Backspace Backspace Backspace Backspace Backspace Backspace Backspace - - o n e i n e Backspace Backspace Backspace l i n e Enter
 g i t Space d i f f Space e x a m p l e . p y Enter
 g i t Space c h e c k o u t Space Ctrl+v Ctrl+z

Exception:
System.ArgumentOutOfRangeException: The value must be greater than or equal to zero and less than the console's buffer size in that dimension.
Parameter name: top
Actual value was -429.
   at System.Console.SetCursorPosition(Int32 left, Int32 top)
   at Microsoft.PowerShell.PSConsoleReadLine.ReallyRender(RenderData renderData, String defaultColor)       
   at Microsoft.PowerShell.PSConsoleReadLine.ForceRender()
   at Microsoft.PowerShell.PSConsoleReadLine.ProcessOneKey(ConsoleKeyInfo key, Dictionary`2 dispatchTable, Boolean ignoreIfNoAction, Object arg)
   at Microsoft.PowerShell.PSConsoleReadLine.InputLoop()
   at Microsoft.PowerShell.PSConsoleReadLine.ReadLine(Runspace runspace, EngineIntrinsics engineIntrinsics) 
-----------------------------------------------------------------------

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.
do so (now or later) by using -c with the switch command. Example:
  git switch -c <new-branch-name>
Or undo this operation with:

  git switch -
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git chekout 1eb770b14e1de4775efa10a18baff1e2f63961a4 --example.py
git: 'chekout' is not a git command. See 'git --help'.

        checkout
.py
error: pathspec 'example.py' did not match any file(s) known to git
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git add example.py
fatal: pathspec 'example.py' did not match any files
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git checkout main
Previous HEAD position was 1eb770b Initial commit
Your branch is up to date with 'origin/main'.
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git checkout origin/main -- example.py
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git add example.py
On branch main
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git branch -d feature_branch
Deleted branch feature_branch (was 5fcb8cb).
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git -D feature_branch
unknown option: -D
usage: git [-v | --version] [-h | --help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git push origin main
fatal: unable to access 'https://github.com/Gautam2901/Git-Work.git/': Could not resolve host: github.com   
origin  https://github.com/Gautam2901/Git-Work.git (fetch)
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git push origin main
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git tag
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git tag -a v1.0 -m "First release version"
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git push origin v1.0
Enumerating objects: 1, done.
Writing objects: 100% (1/1), 175 bytes | 175.00 KiB/s, done.
To https://github.com/Gautam2901/Git-Work.git
 * [new tag]         v1.0 -> v1.0
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git tag -d v1.0
Deleted tag 'v1.0' (was 09d5d2e)
To https://github.com/Gautam2901/Git-Work.git
 - [deleted]         v1.0
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git stash
No local changes to save
No stash entries found.
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git cheryy-pick abc1234d56789xyz
git: 'cheryy-pick' is not a git command. See 'git --help'.

The most similar command is
        cherry-pick
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git cherry-pick abc1234d56789xyz
fatal: bad revision 'abc1234d56789xyz'
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git archieve --format=zip HEAD > archieve.zip
git: 'archieve' is not a git command. See 'git --help'.

The most similar command is
        archive
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git archieve --format=zip HEAD > archive.zip
git: 'archieve' is not a git command. See 'git --help'.

The most similar command is
        archive
PS C:\Users\Gautam\Desktop\GitHub\Git-Work> git archive --format=zip HEAD > archive.zip
PS C:\Users\Gautam\Desktop\GitHub\Git-Work>