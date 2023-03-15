
# GIT: 
Git is version control software that lets you keep track of your code.

* keep track of changes to code
* Syncronize code between people
* Test changes to the code without removing the original
    - Like try making some changes but you don't wanna mess with already working one
    - We can make changes to seperate branch
* Revert back to old versions of code.
    - When you mess up

### Basic Commands
1. Clone the repo
        This downloads(gets a copy) the repo(codes) from internet by giving the link.
```
git clone <url>
```

* You dont need to keep track of every piece of code you write you just have to update as you write some basic 
changes or features. We call `commit` to tell we want to save something.

2. Tell git to track specific file or folder
        By this you tell git to register the file to keep track of it for future purpose
    * while working with larger files we want to just save whats required
    * by this u tell to just commit this file not all of the files

```
git add <filename_to_register>
```
3. Take snapshot of changes
    By this your telling git to save what I have added(registered) 
    * we can add a comment or referance messege for why and what have we done changes
```
git commit -m "I changed this and added these features"
```
output
```
$ git commit -m "Home page added"
[main (root-commit) 235dafb] Home page added
 1 file changed, 12 insertions(+)               # 12 insertions(lines of code) added
 create mode 100644 homepage.html               # on homepage.html file
```

All of the above (changes) you did was only on your local 

4. You can check the status of the repo
```
git status
```
5. Finally upload on internet
    Now push to github to a use anywhere
```
git push
```
6. After this if you want to commit new version of code along with message
```
git commit -am "message here"
```
* this doesn't add any other new file
* just commits the existing added file.

7. Get the code of from git
    * when your colleague has written a extra feature and you want to make a copy of that

```
git push
```
* As soon as you do that you have the latest version of the file that was online 

What if you make changes(pull) on the file you was half working and that got disappeared, then we call this as
`Merge Conflicts`

### Other basic commands:
1. List the directories(folder and files) in pwd
```
ls
```

2. Create a new file in terminal 
```
touch <name_of_file_.extension>
```
---

## Temp
…or create a new repository on the command line
```
echo "# eduhub" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/warandrule/eduhub.git
git push -u origin main
```
…or push an existing repository from the command line
```
git remote add origin https://github.com/warandrule/eduhub.git
git branch -M main
git push -u origin main
```