# Latihan
<hr>

```php
$ git config --list
diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
http.sslbackend=openssl
http.sslcainfo=C:/Program Files/Git/mingw64/ssl/certs/ca-bundle.crt
core.autocrlf=true
core.fscache=true
core.symlinks=false
core.fsmonitor=true
pull.rebase=false
credential.helper=manager-core
credential.https://dev.azure.com.usehttppath=true
init.defaultbranch=master
user.name=Danis Apriyanto
user.email=danisapriyanto@ugm.ac.id
```

```php
git clone
$ git clone https://github.com/andikarifki/ujian-paradigma
Cloning into 'ujian-paradigma'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 3 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.

$ git init
Initialized empty Git repository in G:/1. Kuliah_STIMK AKAKOM/Materi Kuliah/6. Semester Genap T.A. 2022-2023/6. PRAKTIKUM TEKNOLOGI CLOUD/tekn-cloud-computing/minggu-01/.git/

$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        gambar-01.jpg
        latihan.md/
      
nothing added to commit but untracked files present (use "git add" to track)

$ git add .

$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   gambar-01.jpg
        new file:   latihan.md

$ git commit -m "firstcommit"
[master (root-commit) ac66825] firstcommit
 2 files changed, 12 insertions(+)
 create mode 100644 gambar-01.jpg
 create mode 100644 latihan.md

 $ git remote add origin https://github.com/danisapriyanto/tekn-cloud-computing.git

 $ git push -u origin master
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 94.40 KiB | 15.73 MiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/danisapriyanto/tekn-cloud-computing.git
 * [new branch]      master -> master
branch 'master' set up to track 'origin/master'.
```

```php
PS G:\1. Kuliah_STIMK AKAKOM\Materi Kuliah\6. Semester Genap T.A. 2022-2023\6. PRAKTIKUM TEKNOLOGI CLOUD\tekn-cloud-computing\minggu-01> git checkout -b edit-readme-1
Switched to a new branch 'edit-readme-1'
```

```php
PS G:\1. Kuliah_STIMK AKAKOM\Materi Kuliah\6. Semester Genap T.A. 2022-2023\6. PRAKTIKUM TEKNOLOGI CLOUD\tekn-cloud-computing\minggu-01> git status
On branch edit-readme-1
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   git-single.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        latihan.md

no changes added to commit (use "git add" and/or "git commit -a")
```