
  $git config --global user.name

  $git config --global user.name "Ravindra Kumar"
  
  $git config --global user.name
   Ravindra Kumar
    
  $ git config --global user.email "netivenkatravindrakumar@gmail.com"
   
  $ git config --global user.email
   netivenkatravindrakumar@gmail.com
   
  $ mkdir myntrasales
  
  $ ll
  total 0
  drwxr-xr-x 1 Ravi 197121 0 Sep 11 12:21 myntrasales/
  
  $ cd myntrasales/
  
  $ git init
   Initialized empty Git repository in D:/Git/myntrasales/.git/

  $ git clone https://github.com/Venkatravindrakumar/wforwomen.git
    Cloning into 'wforwomen'...
    remote: Enumerating objects: 3, done.
   remote: Counting objects: 100% (3/3), done.
   remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
   Receiving objects: 100% (3/3
 Make a change in project and update to local Repository 
 
  Ravi@DESKTOP-QO9FJ4D MINGW64 /d/Git/myntrasales (master)
  $ cd ..
  $ avi@DESKTOP-QO9FJ4D MINGW64 /d/Git
  
  $ ll
  total 0
  drwxr-xr-x 1 Ravi 197121 0 Sep 11 12:42 myntrasales/
  drwxr-xr-x 1 Ravi 197121 0 Sep 11 12:42 wforwomen/
  
  $ cd myntrasales/
  
  $git status 
  On branch master
  No commits yet
  nothing to commit (create/copy files and use "git add" to track)
  
  $ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md
no changes added to commit (use "git add" and/or "git commit -a")

  $ git add README.md
  
  $  git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md
		
   $ $ git commit README.md -m "README.md file is upadated"
[main 471b183] README.md file is upadated
 1 file changed, 8 insertions(+), 1 deletion(-)
    
	$ git status
 On branch main
 Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

  nothing to commit, working tree clean
  
 
   $ git push
   Enumerating objects: 5, done.
   Counting objects: 100% (5/5), done.
   Delta compression using up to 4 threads
  Compressing objects: 100% (2/2), done.
  Writing objects: 100% (3/3), 511 bytes | 255.00 KiB/s, done.
  Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
   To https://github.com/Venkatravindrakumar/wforwomen.git
   fe3ae2d..471b183  main -> main
   
   
   $ ll
total 14
-rw-r--r-- 1 Ravi 197121 6223 Sep 11 13:28 Index.html
-rw-r--r-- 1 Ravi 197121  405 Sep 11 13:04 README.md
-rw-r--r-- 1 Ravi 197121  100 Sep 11 13:36 Scripts.js
-rw-r--r-- 1 Ravi 197121 3974 Sep 11 13

  $$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Index.html
        Scripts.js
        styles.css

nothing added to commit but untracked files present (use "git add" to track)

   $ git add .
   
  $ git status 
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   Scripts.js
        new file:   index.html
        new file:   styles.css
 

   $ git commit -m "updating wforwomen page with index.html scripts.js styles.css"
[main 3fbf458] updating wforwomen page with index.html scripts.js styles.css
 3 files changed, 337 insertions(+)
 create mode 100644 Scripts.js
 create mode 100644 index.html
 create mode 100644 styles.css
 
    $ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)
  
  $ git push
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 2.42 KiB | 1.21 MiB/s, done.
Total 5 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Venkatravindrakumar/wforwomen.git
   471b183..3fbf458  main -> main
  
 $ git branch
* main
 $git branch feature1
 $ git branch
 $ git checkout feature1
 $ ll
 $git checkout main 
 $git checkout -b feature2
 $ll
 $git branch
  feature1
* feature2
  main
 $ git checkout main
 $ git branch -d feature1
 Deleted branch feature1 (was 3fbf458).
 $ git reflog
 $ git checkout -b feature1
  Switched to a new branch 'feature1'
  $






  
	 
	 




   
   

