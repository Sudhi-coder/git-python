This is the file to know about git and github.
Git is the version control system which is used for developers to maintain the code and work it remotely.

There are 2 types of version control system:
=> Centralised Version Control
=> Distributed Version Control 

In Centralised Version Control, the developers have to maintain a central repository and then they have work it on the remote repository. This cannot be work it on a offline. They cannot download it. It needs continuous network to work.

Git commands:

      => git --version

To configure in the git
      => git config --global user.name
      => git config --global user.email

To keep tracking of our file, we use
       => git init

no longer tracking is necessary,
       => rm -rf .git

To see the status of the file, whether it is uploaded to remote repository or committed 

        => git status

Add gitignore because, the file contain our info about operating systems, personal preferences and so on. To avoid it in a public view add gitignore file
touch .gitignore


Three areas that our files will cover
=> working area => untracked and modified file will be presented

=> Staging area => it tracked,organized and ready to commit to the remote repository

			=> here we will be adding files with git commands
			=> git add <file_name> or git add -A or git add .

To check whether the files or tracked or not, => git status

To remove the file from staging,use
           
		   => git reset <file_name>

We need to commit the changes to the remote repository 
          => git commit -m "first commit"

Once commit is done, then our working directory will be clean. 

So that all the files are tracked and unmodified, until we made any changes to the files.

To view the commit ID(hash number, which is unique) and detailed info of who committed the files, will use:
           => git log

To add the remote repo to our local repo:
            => git remote add origin https://github.com/Pavithra-r15/git-tutorial.git

Then push the code which we have committed
        => git push -u origin main/master

=> Remote area => should clone the remote repository
				=> git clone <url>

Then add the files, commit it and then do some changes to the file

Follow the same steps and continue with the the commands

	=> git diff
	=> git status
	=> git add
	=> git commit -m "initial commit" 

This command is to check the repository whether it is updated from other branches or by other developers.
		=> git pull origin main/master

To push our code or changes to the remote repository 

		=> git push origin main/master 

Remote repository:
Creating branch 

            => git branch <branch_name>

To checkout the branch

            => git checkout <branch_name>
            
or use,it will create and switch the branch

            => git ceckout -b <branch_name>
            => git switch -c <branch_name>

To merge the branch 

            => git branch --merged

To merge the branch

            => git merge <branch_name>

To push it in the remote repo

            => git push origin main

To delete the branch in local

            => git branch -d <branch_name>

To delete the branch in remote repo

            => git push origin --delete <branch_name>





