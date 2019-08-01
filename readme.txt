1. git config --global user.name "Jeremy Liu"
2. git config --global user.email "jeremy.liu@nxp.com"
3. mkdir empty direction in anywhere you want
4. git init
5. git add readme.txt
6. git commit -m "this is the initial version for using git to manage the file"

//this for second change 

//this for third change

other command
1. git log //to review every version of the file
2. git log --pretty=oneline //show one line logfile
3. git reset --hard "version id" "file" // version back OR discard changers in stage
4. git reflog //record of git log
5. git status //the file status
6. git diff -- "version id" "file" //diff version and word directory 
7. git checkout -- "file" //discard changers in work directory

remove
1. git rm 
2. git comit -m ""
