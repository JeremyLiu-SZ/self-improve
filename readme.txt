1. git config --global user.name "Jeremy Liu"
2. git config --global user.email "jeremy.liu@nxp.com"
3. mkdir empty direction in anywhere you want
4. git init
5. git add readme.txt
6. git commit -m "this is the initial version for using git to manage the file"

//this for second change 

//this for third change

other command
1. git log # //to review every version of the file
2. git log --pretty=oneline # //show one line logfile
3. git reset --hard "version id" "file" // version back OR discard changers in stage
4. git reflog //record of git log
5. git status //the file status
6. git diff -- "version id" "file" //diff version and word directory 
7. git checkout -- "file" //discard changers in work directory

remove
1. git rm 
2. git comit -m ""

link to origin 
git remote add origin https://github.com/JeremyLiu-SZ/self-improve.git
git push -u origin master

branch
1. git branch "branch_name" //create branch 
2. git checkout "branch_name" //switch to branch
OR
1. git checkout -b "branch_name" 

3. git branch //view the branch
4. git merge "branch_name" //merge the branch to master
5. git branch -d "branch_name" //remove branch

6. git merge --no-ff -m "" "branch_name"

7. git merge -D "branch_name" //force remove


stash
1. git stash //save 

2. git stash apply 
3. git stash drop
OR
2. git stash pop

4. git stash list //view the stash 
   git stash apply stash@{0}


information of origin 
1. git remote
2. git remote -v //detail

push to origin
1. git push origin "branch_name"

tag
1. git tag "tag" "version"
2. git tag -a "tag" -m "" "version"
3. git tag -d "tag"

4. git push origin "tag"
5. git push origin --tags

remove tag from origin
1. git tag -d tag
2. git push origin :refs/tags/"tag"


config
git config --global alias.ci commit
git config --global alias.co checkout
git config --global alias.br branch
git config --global alias.last 'log -1'
git config --global alias.unstage 'reset HEAD'
git config --global alias.lg "log --color --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit"
