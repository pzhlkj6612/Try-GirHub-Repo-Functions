first line

----

some dangling commit:

[88481e88b6aa54c2d39d58bab0400e23bed3a693](
https://github.com/pzhlkj6612/Try-GirHub-Repo-Functions/commit/88481e88b6aa54c2d39d58bab0400e23bed3a693)

[8bb6500ad980bdce4c91cbfcc359a6d0871f3077](https://github.com/pzhlkj6612/Try-GirHub-Repo-Functions/commit/8bb6500ad980bdce4c91cbfcc359a6d0871f3077)

```
$ git fsck --no-reflogs
Checking object directories: 100% (256/256), done.
Checking objects: 100% (12/12), done.
dangling commit 894cfcc2f4bbefc932475afce4bdf7a6a825c26e
dangling commit 88481e88b6aa54c2d39d58bab0400e23bed3a693
dangling tree 4b825dc642cb6eb9a060e54bf8d69288fbee4904
dangling commit 8bb6500ad980bdce4c91cbfcc359a6d0871f3077
```

the [894cfcc2f4bbefc932475afce4bdf7a6a825c26e](https://github.com/pzhlkj6612/Try-GitHub-Repo-Functions/commit/894cfcc2f4bbefc932475afce4bdf7a6a825c26e) is unreachable by URL, I don't know why:

```
$ git show 894cfcc2f4bbefc932475afce4bdf7a6a825c26e
commit 894cfcc2f4bbefc932475afce4bdf7a6a825c26e
Author: Mozi 
Date:   Fri Mar 30 22:27:10 2018 +0800

    First...

diff --git a/README.md b/README.md
index 08fe272..c7f3e92 100644
--- a/README.md
+++ b/README.md
@@ -1 +1,2 @@
 first line
+sensitive info
```

