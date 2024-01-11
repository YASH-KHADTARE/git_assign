git init 

vi master_file.txt  (create a master file)

git checkout -b BRANCH1 (create branch 1)

vi B1.txt (Create text files)

vi B2.txt

git status

git add . (add all fies)

git commit -m "ADD files"

git checkout -b BRANCH2 
vi C1.txt

vi C2.txt 

git status

git add . (add all fies)

git commit -m "ADD files"


git log (get entries and their IDs)

git branch (check branches)

(made a change in file to demonstrate soft and hard reset)

(soft reset -  use to make change in commit statement)

git reset --soft HEAD~1   (soft reset)

git log 

git commit -m "RESET SOFT USE"

git log


(HARD reset -  directly delets the record)

(edit)vi B2.txt

git add .

git commit -m "Update File"

git reset --hard HEAD~1

output - HEAD is now at b629ac8 RESET SOFT USE


deleting branch using -d

git checkout master

git checkout -b BRANCH3

git checkout master

git branch -d BRANCH3


-d vs -D (-D forces to delet branch even if it is pushed)

deleting branch using -D

git checkout master

git checkout -b BRANCH3

git checkout master

git branch -D BRANCH3




git checkout BRANCH1

git diff master (differentiate between master and branch1 files)




edited the B2.txt file and used stash

git stash 



PUSHING EACH BRANCH TO REMOTE

git checkout master

git branch -m main     (renaming master to "main")

git remote add origin https://github.com/YASH-KHADTARE/git_assign.git

git push origin main (entering ID and token generated from github)

git push origin BRANCH1

git push origin BRANCH2




Multiline command
git commit -m "update1" -m "update 2"
