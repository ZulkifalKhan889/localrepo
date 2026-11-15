This repo is for learning git workflow

Branches: basically we have one main branch let say we have main branch whicch contain the whole workflow of our application for example we have ecommerce application which is working going on and there is commit a comit b and commit c already done
now our manager asks us to add the payment method what we do we dont go and create that in main what we do is create another branch with another name for exmaple we create feature1 branch for this then we create payment and we commit not to the main
but this new branch and then we check this our if everthing works out and is everything good but remeber that in new branch the commit a b and c are already in this from the main branch its just like the copy of the main branch so we test the new commit 
on it if this works good then we merge it with main branch and this new payment method comes to main branch with commit d 

if error occurs when merging both the bracnhes that is called merge conflicts
to merge feature1 with main we do:  git merge feature1

also the pull is used to get the remote repo to out local repo the remote is on github and the localrepo is basicallly the folder that is in our system 

next there comes undoing changes the changes that gets commit mistakenly like we dont want to commit it so how to undo that

#first case: staged changes 
these are the changes that are add but not commited yet so what we can do if we have done changes in multiple files then what we can do is to we write: git reset so only those files get rest that has unstages changes

#w2nd case: commited changes 
let say you add the changes adn also commited it then what how to reset that so if the commit is 1(latest commit which is known as head) we do : git reset head~1

and if we have done many commits let say 4 adn we want to go back to 1 adn delter those 3 additional comit so what we do we copy the hash of 1 and put it there in git code 
e.g: git reset hash 
hash is a code for commit 1 and if we do the above we go back to the commit 1 and then start from there
