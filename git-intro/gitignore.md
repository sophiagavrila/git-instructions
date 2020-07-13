## Creating `.gitignore`
Let's say that our `log.txt` file contained persornal preferences that we didn't want other people seeing when they viewed this repository.  To hide this file, we create a file called `.gitignore`.  

1. Git Bash within your project directory and use the `touch` command to create 2 files.

```
$ touch log.txt
$ touch .gitignore
```

2. Open the `.gitignore` file in a text editor of your choice and write the names of the files you want to be ignored.  In this case we will write `log.txt`.

3. When you rerun `git status` you will notice that the `log.txt` file is no longer tracked and you will instead see a `.gitignore` file.

 To add a particular file to the Staging Area to commit, such as `.gitignore`, for example, run `git add .gitignore`.  If you want to add all files that you've made changes to, run `git add . `

    * If you ever want to *remove* files from the staging area, (for example, `.gitignore`), you can run the command `git reset .gitignore`.  Running `git reset` will remove everything from the staging area.

4. Once the files have been added, you must **commit** them.  Run the command `git commit -m "add .gitignore"`.  The message in the quotation marks pertains to any information that you might have changed in the lines of code or files that you want to update in the remote repository.

5. Running the command `git log` will show you the unique hash for the commit that you just made.

### References
* [.gitignore](https://git-scm.com/docs/gitignore)