# TXT2


``
kv@kvPC MINGW64 /d
$ git clone https://github.com/Veronika-Koronets/TXT2.git
Cloning into 'TXT2'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.
``
``
kv@kvPC MINGW64 /d
$ cd TXT2

kv@kvPC MINGW64 /d/TXT2 (main)
$ ls -la
total 13
drwxr-xr-x 1 kv 197121 0 Aug  3 18:49 ./
drwxr-xr-x 1 kv 197121 0 Aug  3 18:49 ../
drwxr-xr-x 1 kv 197121 0 Aug  3 18:49 .git/
-rw-r--r-- 1 kv 197121 6 Aug  3 18:49 README.md
``
kv@kvPC MINGW64 /d/TXT2 (main)
$ touch new.txt

kv@kvPC MINGW64 /d/TXT2 (main)
$ git add new.txt

kv@kvPC MINGW64 /d/TXT2 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   new.txt


kv@kvPC MINGW64 /d/TXT2 (main)
$ git commit -m new.txt
[main a5aaee3] new.txt
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 new.txt

kv@kvPC MINGW64 /d/TXT2 (main)
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 275 bytes | 137.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Veronika-Koronets/TXT2.git
   18e7ee6..a5aaee3  main -> main

kv@kvPC MINGW64 /d/TXT2 (main)
$ cat > new.txt
Name: K.Veronika Gennadyevna,
Age: 22,
Number of pets: 1,
Future desired salary: 1300.


kv@kvPC MINGW64 /d/TXT2 (main)
$ git commit -am "new.txt"
warning: in the working copy of 'new.txt', LF will be replaced by CRLF the next time Git touches it
[main 633ad2d] new.txt
 1 file changed, 4 insertions(+)

kv@kvPC MINGW64 /d/TXT2 (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 361 bytes | 120.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Veronika-Koronets/TXT2.git
   a5aaee3..633ad2d  main -> main

kv@kvPC MINGW64 /d/TXT2 (main)
$ touch preferences.txt

kv@kvPC MINGW64 /d/TXT2 (main)
$ cat > preferences.txt
 favourite_film: Legally_Blonde,
 favourite_series : Blacklist,
 favourite_food : pizza,
 favourite_season : spring
 Country_wish_to_visit : Norway


kv@kvPC MINGW64 /d/TXT2 (main)
$ cat > skills.txt
Git, Terminal, Postman, SQL, Charles


kv@kvPC MINGW64 /d/TXT2 (main)
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

kv@kvPC MINGW64 /d/TXT2 (main)
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

kv@kvPC MINGW64 /d/TXT2 (main)
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

kv@kvPC MINGW64 /d/TXT2 (main)
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


kv@kvPC MINGW64 /d/TXT2 (main)
$
