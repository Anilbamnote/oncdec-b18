Git (global information tracker) is software that serves as a tool for version control, helping developers manage and collaborate on projects efficiently.

GitHub is a platform and a service rather than just a tool or software. 

1.INITIALIZEGIT/CLONE REPO
   clone an existing repo using git clone <repo-url>
   OR initializing new repo using git init command ---> .git
 2. EDIT FILES:-
    Work on ur project file in the working directory.----cd repo---touch new---gglh---
 3.  STAGE CHANGES:-
   use git add or git add . to stage changes  git add <file_name>....multiple files---add----git add .
 4. Commit Changes:-
   used git commit -m "commit msg" to save ur changes to local repo.
 5. Push To Remote :-
   git push
 6. PULL UPDATES:-
    pull updated code from remote repo using command >>> git pull
 7.  Branching:-
   create new branch for feature devlopment using >>  git branch <branch name>  ---default--main/master
 8. merge changes:-
   Mearge feature branches to main branch using git merge
 9. Resolve Conflict:-
    git log
     --------------------------------------------------------------------------------------------------------------
     
git clone
   git init
   git add  ----staging area
   git add .  ------all file adeed
   
   git resotr---unstaging area---untrack
   git restore --stage <file-name>

   git commit -----git config --global user.email "anil@gmail.com"
                    git config --global user.name "Anil"
   git push
   
   git revert <commit id>..
   git revert 5ceca0db....git log <show commit id of privious code>

   git log
   git log --oneline  ------recent changes done on particular dire
   
   git remote-----show ur remote repo location
   
   git remote -v ----remotee repo url 
     
     git branch <branchPname>
     
     git branch 
     
     git checkout -b '<branch name>'
     
     git switch <bramch name>
     
     git push origin iata ----push chnages in reture branch...
     
     git merge <source-branch> <main/master-branch>
     
     note:- first present in main branch ---then merge ur feture branch
     
     after merge--hit git add ,git commit,git push origin main
     
     1. Remove a Feature Branch Locally
     >  Before deleting the branch, ensure you are not currently on it:--
     git checkout main
     
     Use the following command to delete the branch locally:
     
      >. git branch -d <feature-branch-name>
      
      2. Remove a Feature Branch from GitHub (Remote Repository)
       >  To delete the branch from the remote repository:

>>>>>>>>Delete the Remote Branch
>>>>>>>>Use the following command:-

   >>> git push origin --delete <feature-branch-name>

     
     List all remote branches to confirm the deletion:
 
    >> git branch -r
     
     
   	PULLING branch FROM GITHUB
   	
   	git branch -f <remote-repo-name> origin/<remote-branch name>
   	ex- git branch -f test origin/test
   	
   	  
     
    GIT RESET, GIT REVERT, 
    
    git reset:- this cmd is used to revert the commit that u did in ur local workspace.this cmd reqired commit id
    
    note: if we used reset cmd we need commit id of just privious code which is ok..and running well fsg
    
    reset cmd used to move changes from commit area to working area.
    -----------------------------------------------------
    dis Adv:-
    it dosent make commit history
    we cant revert code if we hit hard reset.
    cant revert single commint
    once code reset cant be undo that code.
  --------------------------------------------------------  
    type of reset cmd:-
    a> soft reset
    b> hard reset
    
    soft reset:-
    git reset --soft <commit-id>
 ex--git reset  hlhg  ----to show hit >> git log --onelog
 
 hard reset:- new changes fulldeleted.
 
 git reset --hard <commit-id> -------n ot used in real-time-----used soft reset.
 ------------------------------------------------------------------------------------
 
 GIT REVERT:- thsi cmd is used when  we want to revert those commit that we want to go back tha code in working area .
 
 
 if we revert single commit then used revert cmd.
 maintain history of all commit isted of only revert comiit is remove from history.but maintai revert commit id history.
 
 git reset removes the commit historywhen we are reseting the changes and revert will retain the commit history after reverting the commits.
 
 git revert <commit-id> ----used --git log --oneline -----show commoit -id.
 
 Adv:-
 > maintain comit history
 > we can bring back our reverted code
 >used to revert single commit id
 > 
 
 Git RESTOTRE
 
 it is used for remove files from staging area .
 
-------------------------------------------------------------------------------------------------------
 
 git fetch:-
 
 download ur remote repo code in ur staging area but not in ur local area..
 
 git fetch -----only show info of ur remote repo new modified files on terminal--i.e---staging area 
 
 -------------------------------------------------------
 gitlab
 
 paid---but some feature are free
 
 
 comminity based---free----commercial,---enterprice--
    
     
   ------------------------------------------------------------------------------------
   