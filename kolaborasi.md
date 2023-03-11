```php
$ git clone https://github.com/danisapriyanto/rtfm.git
Cloning into 'rtfm'...
remote: Enumerating objects: 130, done.
Receiving objects:  73% (95/130)sed 0 (delta 0), pack-reused 130Receiving objects:  61% (80/130)
Receiving objects: 100% (130/130), 1.30 MiB | 4.06 MiB/s, done.
Resolving deltas: 100% (51/51), done.

$ git clone https://github.com/danisapriyanto/rtfm.git
Cloning into 'rtfm'...
remote: Enumerating objects: 130, done.
Receiving objects:  73% (95/130)sed 0 (delta 0), pack-reused 130Receiving objects:  61% (80/130)
Receiving objects: 100% (130/130), 1.30 MiB | 4.06 MiB/s, done.
Resolving deltas: 100% (51/51), done.

$ git remote -v
origin  https://github.com/danisapriyanto/rtfm.git (fetch)
origin  https://github.com/danisapriyanto/rtfm.git (push)

$ git remote add upstream https://github.com/danisapriyanto/rtfm.git

$ git remote -v
origin  https://github.com/danisapriyanto/rtfm.git (fetch)
origin  https://github.com/danisapriyanto/rtfm.git (push)
upstream        https://github.com/danisapriyanto/rtfm.git (fetch)
upstream        https://github.com/danisapriyanto/rtfm.git (push)

$ git fetch upstream
From https://github.com/danisapriyanto/rtfm
 * [new branch]      master     -> upstream/master

HP@DESKTOP-C8KRFKI MINGW64 /g/1. Kuliah_STIMK AKAKOM/Materi Kuliah/6. Semester Genap T.A. 2022-2023/6. PRAKTIKUM TEKNOLOGI CLOUD/rtfm (master)
$ ls -la
total 672
drwxr-xr-x 1 HP 197121      0 Mar 11 21:48 ./
drwxr-xr-x 1 HP 197121      0 Mar 11 21:48 ../
drwxr-xr-x 1 HP 197121      0 Mar 11 22:01 .git/
-rw-r--r-- 1 HP 197121   4157 Mar 11 21:48 01-install-git.md
-rw-r--r-- 1 HP 197121   1277 Mar 11 21:48 02-konfigurasi-git.md
-rw-r--r-- 1 HP 197121   1416 Mar 11 21:48 03-mengelola-repo-sendiri.md
-rw-r--r-- 1 HP 197121  16354 Mar 11 21:48 03-mengelola-repo-sendiri-account.md
-rw-r--r-- 1 HP 197121    712 Mar 11 21:48 03-mengelola-repo-sendiri-organisasi.md
-rw-r--r-- 1 HP 197121  10007 Mar 11 21:48 04-kolaborasi.md
drwxr-xr-x 1 HP 197121      0 Mar 11 21:48 images/
-rw-r--r-- 1 HP 197121 621542 Mar 11 21:48 install-git.odt
-rw-r--r-- 1 HP 197121   1044 Mar 11 21:48 README.md

$ git checkout -b add-contributor
Switched to a new branch 'add-contributor'

$ git branch
* add-contributor
  master

$ git status
On branch add-contributor
nothing to commit, working tree clean

$ git status
On branch add-contributor
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

$ git add -A

$ git commit -m "Add: contributor"
[add-contributor 8fbc5a0] Add: contributor
 1 file changed, 2 insertions(+)

$ git checkout master
Switched to branch 'master'
Your branch is up to date with 'origin/master'.

$ git push origin add-contributor
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 310 bytes | 310.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'add-contributor' on GitHub by visiting:
remote:      https://github.com/danisapriyanto/rtfm/pull/new/add-contributor
remote:
To https://github.com/danisapriyanto/rtfm.git
 * [new branch]      add-contributor -> add-contributor

$ git checkout master
Already on 'master'
Your branch is up to date with 'origin/master'.

$ git branch
  add-contributor
* master

$ git fetch upstream
From https://github.com/danisapriyanto/rtfm
 * [new branch]      add-contributor -> upstream/add-contributor

$ git merge upstream/master
Already up to date.

$ git push origin master
Everything up-to-date

```