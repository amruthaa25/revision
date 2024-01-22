
EXPERIMENT 5: Git stash
	Create a new repository in github and add a simple text file
	Get inside your working directory in local system and perform the following-
git clone https://github.com/namratasgit/stashrepo.git //cloning a remote repo to local system
cd stashrepo   // get into the cloned repo
git init	 
git branch feature1   //create new branch – feature1
git checkout feature1	// switch to feature branch

// perform the following actions
notepad second.txt		
git add .
git stash	// stash the second.txt file
notepad third.txt
git add .
git commit –m “F2”  //commit the third.txt file
git log 
ls
git stash apply
ls
git stash
git checkout main  // switch to main branch
git merge main		// perform merge
git branch feature2   //create new branch – feature2
git checkout feature2	// switch to feature branch 

//perform the following actions
notepad fourth.txt
git add .
git stash		// stash the fourth.txt file
git checkout main		//switch to main branch
git merge main	// perform merge on main
git push origin main	//push changes to github repo

