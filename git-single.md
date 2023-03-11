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
# Latihan Github Danis

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

PS G:\1. Kuliah_STIMK AKAKOM\Materi Kuliah\6. Semester Genap T.A. 2022-2023\6. PRAKTIKUM TEKNOLOGI CLOUD\tekn-cloud-comp -a)uting\minggu-01> git add .
PS G:\1. Kuliah_STIMK AKAKOM\Materi Kuliah\6. Semester Genap T.A. 2022-2023\6. PRAKTIKUM TEKNOLOGI CLOUD\tekn-cloud-computing\minggu-01> git commit -m "latihancommit"
[edit-readme-1 9f53853] latihancommit
 2 files changed, 101 insertions(+)
 create mode 100644 latihan.md

 PS G:\1. Kuliah_STIMK AKAKOM\Materi Kuliah\6. Semester Genap T.A. 2022-2023\6. PRAKTIKUM TEKNOLOGI CLOUD\tekn-cloud-computing\minggu-01> git branch -D edit-readme-1
Deleted branch edit-readme-1 (was 3f5e851).
```