# endterm
#first ill initiate my git file in my folder
C:\20211CDV0015>git init
Reinitialized existing Git repository in C:/20211CDV0015/.git/

#then ill add my remote url to link my account
C:\20211CDV0015>git remote add origin https://github.com/duckhitches/endterm.git
error: remote origin already exists.

#ill create a master branch and add add.pyfile
C:\20211CDV0015>git branch -M master

C:\20211CDV0015>notepad add.py

C:\20211CDV0015>git commit -m "addfile"
On branch master

Initial commit

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Dockerfile
        add.py
        index.html

nothing added to commit but untracked files present (use "git add" to track)

C:\20211CDV0015>git add add.py

C:\20211CDV0015>git commit -m "addfile"
[master (root-commit) d4d2f95] addfile
 1 file changed, 4 insertions(+)
 create mode 100644 add.py

#then ill create a feature-branch and add diff.py
C:\20211CDV0015>git branch feature-branch

C:\20211CDV0015>notepad diff.py

C:\20211CDV0015>git add diff.py

C:\20211CDV0015>
C:\20211CDV0015>git commit -m "difffile"
[master 7a1b7ce] difffile
 1 file changed, 4 insertions(+)
 create mode 100644 diff.py

C:\20211CDV0015>git checkout feature-branch
Switched to branch 'feature-branch'

#then ill create dicv.pyffile
C:\20211CDV0015>git checkout master branch
error: pathspec 'branch' did not match any file(s) known to git

C:\20211CDV0015>git checkout feature-branch
Already on 'feature-branch'

C:\20211CDV0015>notepad diff.py

C:\20211CDV0015>git add diff.py

C:\20211CDV0015>git commit -m "difffile"
[feature-branch d5b9306] difffile
 1 file changed, 4 insertions(+)
 create mode 100644 diff.py

C:\20211CDV0015>git checkout master
Switched to branch 'master'

C:\20211CDV0015>notepad product.py

C:\20211CDV0015>git add product.py

C:\20211CDV0015>git commit -m "productfile"
[master d0b0f45] productfile
 1 file changed, 4 insertions(+)
 create mode 100644 product.py

C:\20211CDV0015>git checkout feature-branch
Switched to branch 'feature-branch'

#thn ill perform rebase 
C:\20211CDV0015>git rebase feature-branch
Current branch feature-branch is up to date.

C:\20211CDV0015>git checkout master
Switched to branch 'master'

C:\20211CDV0015>notepad div.py

C:\20211CDV0015>git add div.py

C:\20211CDV0015>git commit -m "divfile"
[master 8da1d99] divfile
 1 file changed, 4 insertions(+)
 create mode 100644 div.py

C:\20211CDV0015>git checkout feature-branch
Switched to branch 'feature-branch'

C:\20211CDV0015>notepad modulus.py

C:\20211CDV0015>git add modulus.py

C:\20211CDV0015>git commit -m "modulusfile"
[feature-branch 573eb7a] modulusfile
 1 file changed, 4 insertions(+)
 create mode 100644 modulus.py

C:\20211CDV0015>git rebase feature-branch
Current branch feature-branch is up to date.

#at last we'll push the commites to the master
C:\20211CDV0015>git push origin master
