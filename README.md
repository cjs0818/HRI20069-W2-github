# Remote & Branch

  ```
    $ mkdir HRI-20069-W2-github
    $ cd HRI-20069-W2-github/
    $ git init
    
    Initialized empty Git repository in /home/jschoi/work/HRI-20069-W2-github/.git/
  ````

For your convenience, do this alias for git log.
  ```
    $ git config --global alias.log0 "log --branches --decorate --graph --oneline"
  ```
  
Make a new file called master.txt and add a line typing "01".
  ```
    $ vi master.txt
    01
  ```
Then, add & commit
  ```
    $ git add .
    $ git commit -am "The first commit"
    [master (root-commit) 049fb0b] The first commit
     1 file changed, 1 insertion(+)
     create mode 100644 master.txt
   ```

Add a remote repository using github.com assuming you already have a repository of 'git@github.com:your_ID/HRI20069-W2-github.git'
  ```
    $ git remote add origin git@github.com:your_ID/HRI20069-W2-github.git
    $ git push -u origin master
    Counting objects: 3, done.
    Writing objects: 100% (3/3), 221 bytes | 0 bytes/s, done.
    Total 3 (delta 0), reused 0 (delta 0)
    To git@github.com:your_ID/HRI20069-W2-github.git
     * [new branch]      master -> master
    Branch master set up to track remote branch master from origin.
  ```
