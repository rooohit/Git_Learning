create a folder called git
open git bash from this folder
git init(intialise the git repository)
touch names.txt
git status
one file will be here that are unttracted
git add .
git status
changes to be commite now the files are in staged area and are getting tracted
git commit -m "First file has been commited"
git status
nothing will be there
add some text in the file
git status
modified karai hui hai
again you can do
git add . or names.txt
git status
they will be in staged area, now you can backtrac it from here and unsatge these
git restore --staged  names.txt
git status
git add names.txt
git commit -m "adding some content in the files name.txt"
Now if you want to go in a perticular date or time from where you think that code was right then you can go there

do 
git log
see the time there time of commit and copy the hash value of that commit

git reset hash

what this command will do is it will move all the commits done after that hash those changes will now be moved to unttraced area and if you want you can move it again to commit 


Or if you do not want to commit this directories and keep it behind the seen or save somewhere

you can do
git add .
then 
git stash
this files will be save somewhere and you can call it any time you want.

and if you want to pull them back

git stash pop
git stash clear 
will clear the bckground

to sync the project to github make one repo on github and copy its ur
git remote add origin url
git remote -v(to see the remote url to push and pull)

git push origin master (pushing our work on github with the help of origin which sort of refrence github url and pushing the master branch)

git branch -M main(it will add main in place or master in you git bash cuse github hs upgraded it to main so it will give you error while pushing)

fork(you can fork other people projects and work on it on your local pc by cloning it)

git clone URL(of the project to clone.)

origin is the url that is your personal github url and upstream url will be the one from where you have forked the project

git remote add upstream URL(of the repo that you have forked from other person github)








