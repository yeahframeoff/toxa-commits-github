toxa-commits-github
===================

My CVS hometask.
================

My hometask report:

1) Created file "production_ready_1.txt" in root dir
2) Edited its content

3) Checked status of working copy

```
$ git status

On branch master

Initial commit

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        production_ready_1.txt

nothing added to commit but untracked files present (use "git add" to track)
```

4) Stashed changes in "production_ready_1.txt" via command:

```
$ git add production_ready_1.txt
```

5) commited changes

```
$ git commit
[master (root-commit) 444fcc8] Added file production_ready_1.txt
 1 file changed, 1 insertion(+)
 create mode 100644 production_ready_1.txt
```

6) pushed first changes to origin/master

```
$ git push origin master
Username for 'https://github.com': yeahframeoff
Password for 'https://yeahframeoff@github.com':
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 272 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/yeahframeoff/toxa-commits-github.git
 * [new branch]      master -> master
```

7) The same with file "production_ready_2.txt"

```
$ git add production_ready_2.txt

$ git commit
[master e80d981] Added file production_ready_2.txt
 1 file changed, 2 insertions(+)
 create mode 100644 production_ready_2.txt

$ git push origin master
Username for 'https://github.com': yeahframeoff
Password for 'https://yeahframeoff@github.com':
Counting objects: 4, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 332 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/yeahframeoff/toxa-commits-github.git
   444fcc8..e80d981  master -> master

```

8) Created branch 'develop' and moved onto it:

```
$ git branch develop
$ git checkout develop
Switched to branch 'develop'
```

9) Created file "hello_world.cpp" in root dir

10) Stashed changes and commited

```
$ git add hello_world.cpp
$ git commit
[develop 7063563] Added develop file "hello_world.cpp"
 1 file changed, 8 insertions(+)
 create mode 100644 hello_world.cpp
```

11) Pushed changes onto new remote branch 'origin/develop'

```
$ git push origin develop
Username for 'https://github.com': yeahframeoff
Password for 'https://yeahframeoff@github.com':
Counting objects: 4, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 421 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/yeahframeoff/toxa-commits-github.git
 * [new branch]      develop -> develop
```

12) Changed hello_world.cpp, commited and pushed

```
$ git add hello_world.cpp

$ git commit
[develop 917dc4f] Replaced "stdio.h" to "iostream" in hello_world.cpp
 1 file changed, 4 insertions(+), 2 deletions(-)

$ git push origin develop
Username for 'https://github.com': yeahframeoff
Password for 'https://yeahframeoff@github.com':
Counting objects: 6, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 397 bytes | 0 bytes/s, done.
Total 3 (delta 1), reused 0 (delta 0)
To https://github.com/yeahframeoff/toxa-commits-github.git
   7063563..917dc4f  develop -> develop
```

13) Added branch develop-feature1, changed hello_world.cpp and production_ready.txt, commited and pushed

```
$ git branch develop-feature1
$ git checkout develop-feature1
M       hello_world.cpp
M       production_ready_1.txt
Switched to branch 'develop-feature1'
$ git status
On branch develop-feature1
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   hello_world.cpp
        modified:   production_ready_1.txt

no changes added to commit (use "git add" and/or "git commit -a")
$ git commit -a
[develop-feature1 6529e8e] Added time output
 2 files changed, 5 insertions(+), 1 deletion(-)
$ git push origin develop-feature1
Username for 'https://github.com': yeahframeoff
Password for 'https://yeahframeoff@github.com':
Counting objects: 8, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 548 bytes | 0 bytes/s, done.
Total 4 (delta 0), reused 0 (delta 0)
To https://github.com/yeahframeoff/toxa-commits-github.git
 * [new branch]      develop-feature1 -> develop-feature1
```
14) One more commit

```
$ git add dvlup-feat1.txt
$ git commit
[develop-feature1 28f7d91] 0001: Feature 1 (added file dvlup-feat1.txt)
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 dvlup-feat1.txt
$ git push origin develop-feature1
Username for 'https://github.com': yeahframeoff
Password for 'https://yeahframeoff@github.com':
Counting objects: 6, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 302 bytes | 0 bytes/s, done.
Total 3 (delta 1), reused 0 (delta 0)
To https://github.com/yeahframeoff/toxa-commits-github.git
   6529e8e..28f7d91  develop-feature1 -> develop-feature1
```
15) The same on develop-feature2

```
$ git checkout develop
Switched to branch 'develop'
$ git branch develop-feature2
$ git checkout develop-feature2
$ git add hello_world.cpp
$ git commit
[develop-feature2 b0e5b5d] 0002: Feature 2 (added random output to hello_world.cpp)
 1 file changed, 4 insertions(+)
$ git commit -a
[develop-deature2 e0864d5] 0002: Feature 2 (Added info in production_ready.txt)
 1 file changed, 2 insertions(+), 1 deletion(-)

 $ git push origin develop-feature2
Username for 'https://github.com': yeahframeoff
Password for 'https://yeahframeoff@github.com':
Total 0 (delta 0), reused 0 (delta 0)
To https://github.com/yeahframeoff/toxa-commits-github.git
 * [new branch]      develop-feature2 -> develop-feature2
```

16) Merge develop-feature1 into develop

```
$ git checkout develop
Switched to branch 'develop'
$ git merge develop-feature1
Updating 917dc4f..28f7d91
Fast-forward
 dvlup-feat1.txt        | 0
 hello_world.cpp        | 2 ++
 production_ready_1.txt | 4 +++-
 3 files changed, 5 insertions(+), 1 deletion(-)
 create mode 100644 dvlup-feat1.txt
$ git push origin develop
Username for 'https://github.com': yeahframeoff
Password for 'https://yeahframeoff@github.com':
Total 0 (delta 0), reused 0 (delta 0)
To https://github.com/yeahframeoff/toxa-commits-github.git
   917dc4f..28f7d91  develop -> develop
```

17) Merge develop into master

```
$ git checkout master
Switched to branch 'master'
Your branch is up-to-date with 'origin/master'.
$ git merge develop
Updating e80d981..28f7d91
Fast-forward
 dvlup-feat1.txt        |  0
 hello_world.cpp        | 12 ++++++++++++
 production_ready_1.txt |  4 +++-
 3 files changed, 15 insertions(+), 1 deletion(-)
 create mode 100644 dvlup-feat1.txt
 create mode 100644 hello_world.cpp
$ git push origin master
Username for 'https://github.com': yeahframeoff
Password for 'https://yeahframeoff@github.com':
Total 0 (delta 0), reused 0 (delta 0)
To https://github.com/yeahframeoff/toxa-commits-github.git
   e80d981..28f7d91  master -> master
```

17) Delete branch develop-feature2 locally and remotely

```
$ git checkout develop
Switched to branch 'develop'
$ git branch -D develop-feature2
Deleted branch develop-feature2 (was e0864d5).
$ git push origin --delete develop-feature2
Username for 'https://github.com': yeahframeoff
Password for 'https://yeahframeoff@github.com':
To https://github.com/yeahframeoff/toxa-commits-github.git
 - [deleted]         develop-feature2
```

18) Tag current master state as v1.0 'release1'

```
$ git tag -a v1.0 -m release1
$ git push --tags
Username for 'https://github.com': yeahframeoff
Password for 'https://yeahframeoff@github.com':
Counting objects: 1, done.
Writing objects: 100% (1/1), 158 bytes | 0 bytes/s, done.
Total 1 (delta 0), reused 0 (delta 0)
To https://github.com/yeahframeoff/toxa-commits-github.git
 * [new tag]         v1.0 -> v1.0
```


### PART 1

1.1) Command that outputs the message and author of each commit from branch "develop-feature1", which havr been made for last 3 hours and which are not on parent branches (develop, master):

```
$ git log develop-feature1 --pretty=format:"%h - %an: %s " --since=3.hours --max-parents=0
```

1.2) For each commit from branches master, develop which message contains specified issue number (for example, 231), outputs its subject, author name and date.

```
$ git log develop master --pretty=format:"%s - %an: %ad " --grep=231
```

### PART 2

## Selective merge

Variant 1

Assume we're now now on develop-feature1 and we already pulled and found out that the coworker commited 3 more commits. Run following command to retrieve those 3 commits and our critical one:
```
$ git checkout develop-feature1

$ git log -4 --pretty=format:"%h"
```
Our "critical commit" appears on the bottom of the list with its hash. Remember the hash, then checkout to develop and merge with this commit:
```
$ git checkout develop

$ git merge here_write_the_hash
```

For example:

```
$ git checkout develop-feature1

$ git log -4 --pretty=format:"%h"
e41e822
0227e30
75b71ae
fb4f0f9
```

The hash to remember is ```fb4f0f9```

```
$ git checkout develop

$ git merge fb4f0f9
```

Variant 2

```
$ git checkout develop-feature1
$ git reset HEAD~3
$ git checkout develop
$ git merge develop-feature1
$ git checkout develop-feature1
$ git reset ORIG_HEAD
```