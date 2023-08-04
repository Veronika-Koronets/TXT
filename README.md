# TXT

## 1. Create an external repository called XML
Going to https://github.com/Veronika-Koronets?tab=repositories, then click "New", enter a name "TXT", make it public and choose "Add a README file" and description.

## 2. Clone repository to local PC
Im going to my new repository. Click Code-->Local-->HTTP and copy this link

```
kv@kvPC MINGW64 /d
$ git clone https://github.com/Veronika-Koronets/TXT2.git
Cloning into 'TXT'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.
```

## 3. Create new.txt file in the local repo

```
kv@kvPC MINGW64 /d
$ cd TXT

kv@kvPC MINGW64 /d/TXT2 (main)
$ ls -la
total 13
drwxr-xr-x 1 kv 197121 0 Aug  3 18:49 ./
drwxr-xr-x 1 kv 197121 0 Aug  3 18:49 ../
drwxr-xr-x 1 kv 197121 0 Aug  3 18:49 .git/
-rw-r--r-- 1 kv 197121 6 Aug  3 18:49 README.md


kv@kvPC MINGW64 /d/TXT (main)
$ touch new.txt
```

## 4. Add a file for tracking

```
kv@kvPC MINGW64 /d/TXT (main)
$ git add new.txt

kv@kvPC MINGW64 /d/TXT (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   new.txt
```

## 5. Do commit file

```
kv@kvPC MINGW64 /d/TXT (main)
$ git commit -m new.txt
[main a5aaee3] new.txt
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 new.txt
```

## 6. Send the file to remote repository
Use ``git push`` for it

```
kv@kvPC MINGW64 /d/TXT (main)
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 275 bytes | 137.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Veronika-Koronets/TXT2.git
   18e7ee6..a5aaee3  main -> main
```

## 7. Edit the content of the “new.txt” file - write information about yourself (full name, age, number of pets, future desired salary). Everything is written in TXT format.

```
kv@kvPC MINGW64 /d/TXT (main)
$ cat > new.txt
Name: K.Veronika Gennadyevna,
Age: 22,
Number of pets: 1,
Future desired salary: 1300.
```

## 8. Send the changes to remote repository
When we want to commit file, that was commited before, use command ``git commit -am "file name" ``. It combine ``git add`` and ``git commit -m``

```
kv@kvPC MINGW64 /d/TXT (main)
$ git commit -am "new.txt"
warning: in the working copy of 'new.txt', LF will be replaced by CRLF the next time Git touches it
[main 633ad2d] new.txt
 1 file changed, 4 insertions(+)
```

```
kv@kvPC MINGW64 /d/TXT (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 361 bytes | 120.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Veronika-Koronets/TXT2.git
   a5aaee3..633ad2d  main -> main
```

## 9. Create preferences.txt file.

```
kv@kvPC MINGW64 /d/TXT (main)
$ touch preferences.txt
```

## 10. In the preferences.txt file, add information about your preferences (Favorite movie, favorite series, favorite food, favorite season, side you would like to visit) in TXT format

```
kv@kvPC MINGW64 /d/TXT (main)
$ cat > preferences.txt
 favourite_film: Legally_Blonde,
 favourite_series : Blacklist,
 favourite_food : pizza,
 favourite_season : spring
 Country_wish_to_visit : Norway
```

## 11. Create a file skills.txt add information about the skills that will be studied in the course in TXT format.

```
kv@kvPC MINGW64 /d/TXT (main)
$ cat > skills.txt
Git, Terminal, Postman, SQL, Charles
```

## 12. Do one-string commit
## 13. Send 2 files at once to an external repository
Use git add --> git commit -m --> git push

or
```
kv@kvPC MINGW64 /d/TXT (main)
$ git add . && git commit -m "adding preferences.txt and skills.txt" && git push
warning: in the working copy of 'preferences.txt', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'skills.txt', LF will be replaced by CRLF the next time Git touches it
[main 40022e1] adding preferences.txt and skills.txt
 2 files changed, 6 insertions(+)
 create mode 100644 preferences.txt
 create mode 100644 skills.txt
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 513 bytes | 171.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Veronika-Koronets/TXT2.git
   633ad2d..40022e1  main -> main
```

## 14. Create a bug_report.txt file on the web interface
Go to our repo, "Add file" --> "Create new file"

## 15. Make Commit changes (save) changes on the web interface
Press the button "Commit changes"

## 16. Modify the bug_report.txt file on the web interface, add a bug report in TXT format.

## 17. Make Commit changes (save) changes on the web interface.

## 18. Synchronize external and local TXT repository

```
kv@kvPC MINGW64 /d/TXT (main)
$ git pull
remote: Enumerating objects: 7, done.
remote: Counting objects: 100% (7/7), done.
remote: Compressing objects: 100% (5/5), done.
remote: Total 6 (delta 2), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (6/6), 1.52 KiB | 44.00 KiB/s, done.
From https://github.com/Veronika-Koronets/TXT2
   40022e1..04d4a04  main       -> origin/main
Updating 40022e1..04d4a04
Fast-forward
 bug_report.txt | 14 ++++++++++++++
 1 file changed, 14 insertions(+)
 create mode 100644 bug_report.txt
```

```
kv@kvPC MINGW64 /d/TXT (main)
$ ls -la
total 17
drwxr-xr-x 1 kv 197121   0 Aug  3 20:28 ./
drwxr-xr-x 1 kv 197121   0 Aug  3 18:49 ../
drwxr-xr-x 1 kv 197121   0 Aug  3 20:28 .git/
-rw-r--r-- 1 kv 197121   6 Aug  3 18:49 README.md
-rw-r--r-- 1 kv 197121 516 Aug  3 20:28 bug_report.txt
-rw-r--r-- 1 kv 197121  87 Aug  3 19:06 new.txt
-rw-r--r-- 1 kv 197121 148 Aug  3 19:09 preferences.txt
-rw-r--r-- 1 kv 197121  37 Aug  3 19:09 skills.txt

kv@kvPC MINGW64 /d/TXT (main)
$ cat bug_report.txt
ID: 12
 Severity: major ,
 Priority: high ,
 Title:  not all sections are displayed when the main page is reloaded,
 Environment: 1. Samsung Galaxy A12 Android 12, Opera,
                          2. Windows 10, Opera,
 Precondition: open Opera,
 STR: Press restart character in address bar at the top of the page pull down on the mobile phone,
 Expected Result: all page sections are present,
 Actual result: not all sections are present,
 Attachment: video,
 Postcondition: none,
 Author: @nick
```
