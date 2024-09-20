What is git?

git is a distributed file based version control system

File based?

repository and configurations live in a .git folder we can investigate copy or paste no services or container
branch names and tags are like domain names


Plumming and porcelane

What is a repository?

A repository represent a single project.typically one project have one repo.
Essentailly its just a directory that contains a project.That being the only defference is it has a .git directory in it.

 
git init

this initialize a git directory inside your project

status

files in git repos has several states

untracted:not being tracked by git
staged:marked for inclusion in the next commit
committed:saved to the repo history

git status

this shows current status of the the repo.tells you files states

index

git add

make a directory or whole project or selected files tracked basically added to index to track
make the file state to staged

commit

after staging a file we can commit 
a commit is basically a snapshot at any given time of the repo. 

git log

git repo is usually a long list of commits where each one of them represent the full state of the repository at a specific given point of time

git log show you the histry of the commits in a repo


git --no-pager log 

shows you the git log without opening a second screen

git log -n 10 

shows you the last 10 commits

git commit hash

git hash doesnt need to be secure it just there to avoid collusions

Hashing

a hash is a fixed size string or number derived form an input of any size generated using mathematical algo

same input gives you the same output everytime

eg:SHA-2,SHA-1,MD5 etc

git uses SHA-1 for hashing 

Git inputs for its hash

Parent commit hash,commit message,date and time,Author,file changes and more

Git cat-file -p

if you wanna see the git object files u cant since they are stored in compressed raw byte formso git gives us with a command which is git cat-file command 
with cat-file command should follow the -p commit hash.
running this command gives the output:

> git cat-file -p 5ba786fcc93e8092831c01e71444b9baa2228a4f

tree 4e507fdc6d9044ccd8a4a3061324c9f711c4667d
author ThePrimeagen <the.primeagen@aol.com> 1705891256 -0700
committer ThePrimeagen <the.primeagen@aol.com> 1705891256 -0700

A: add contents.md

Tree

gits way of storing a directory

Blob 

gits way of storing a file

how ever we cant see the contents of the file itself thats because the blob object stores it and it has a seperate hash and we can use the same command followed by blob hash to see the contents of the file





























