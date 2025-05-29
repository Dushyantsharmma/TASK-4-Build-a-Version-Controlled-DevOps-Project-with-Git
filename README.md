# TASK-4-Build-a-Version-Controlled-DevOps-Project-with-Git
## Git
- Git is a distributed version control system used to track changes in source code during software 
development. It helps teams collaborate, manage code versions, and keep a history of every change made to a 
project.
```sh
Git can tracks the every changes from work directory to remote repository. 
1. Working directory 
2. Stagging area  
3. Local repository 
4. Remote repository
```
## Git Flow
![Image](https://github.com/user-attachments/assets/7fde12db-c42e-427c-a9ed-5490c508eeb2)





## Git connection:

- SSH keypair
- HTTPS
- PAT
## GIT WORKFLOW COMMON CMDS
- Create a folder in local ------git init  #.git is hidden file
- 
![Image](https://github.com/user-attachments/assets/d15dc7f3-78f6-4d0a-800e-dc6a7057624f)




- git config  --global user.name “username”
- git config  --global user.email “email id”
- git clone  -- This cmd use for a clone the repo from remote to local
- mkdir file-1
- git status
  
![Image](https://github.com/user-attachments/assets/14a86b98-4324-4995-b1fd-8ceb8555191a)



- git add file-1
  
![Image](https://github.com/user-attachments/assets/815913fe-1526-493c-a146-573bc921f66a)



- git commit -m “message”

![Image](https://github.com/user-attachments/assets/520aba46-3431-4be5-b6c9-6c5b113874c0)




- git log
  
![Image](https://github.com/user-attachments/assets/d71ff6a9-fee4-4535-accc-f476614acba5)





- git branch -M main
  
![Image](https://github.com/user-attachments/assets/1a74edba-4c25-41cb-8d06-5d824d96740e)






# Git remote add origin <git repo url>


- Git push -u origin main
  
![Image](https://github.com/user-attachments/assets/5a58cc3c-b043-4606-b9c1-b3f2d0bc06f7)





![Image](https://github.com/user-attachments/assets/0ee829d3-e1af-4596-ae72-c86ae7546a5a)







- Git remote -v # if we get an error: remote origin already exists
  
![Image](https://github.com/user-attachments/assets/16401aa4-2ed4-4fdf-9b7f-044ea84a704d)











- Git remote set-url <git hub repo url> #remove existing origin map and add git remote url
  
![image](https://github.com/user-attachments/assets/e9b586e4-e187-4181-bd2a-6c201d969a17)









- Git branch # checking the branches are available
- 
![image](https://github.com/user-attachments/assets/1ef39fb1-4cda-46ca-8899-07f414008a12)








- Git branch dev # create a sub-branch comes under main branch
  
![image](https://github.com/user-attachments/assets/522974b8-9be9-4edd-a13f-0fa29e892c95)









- Git checkout <branch-name> (or) git switch <branch-name> #move from one branch to other branch
  
![image](https://github.com/user-attachments/assets/2356f849-011b-49b3-8cfb-10e3c658ff97)










- Git checkout -b <sub-branch-name> # this cmd use for create branch and switch to branch
  
![image](https://github.com/user-attachments/assets/5d3ce067-3f0c-46c7-8e82-b0fb5bc7223b)













- git branch -m oldname new name -------> to rename a branch
  
![image](https://github.com/user-attachments/assets/2255c8b6-a0ce-45f6-925c-0d66d0c4118f)













- Git branch -D <branch name> ----- to delete a branch
  
![image](https://github.com/user-attachments/assets/f9473e09-d902-4160-94b4-87c306d4e68e)







## Git logs cmds:
- Git log # check the logs
  
![image](https://github.com/user-attachments/assets/29f75a46-9b54-4ad9-9eb0-3cf15c9e0aeb)










- Git log –oneline # it give in one line log
  
  ![image](https://github.com/user-attachments/assets/4f984b48-5251-4e2a-a117-c5b0c7c5efac)







  
- Git pull #solve the merger conflicts and different commit ids 
# Team work with same repo and push and pull conflicts
# Here I am taking to team mates 1. Windows and 2. Linux
- git pull --no-rebase # it fetch the missing commit id and create a new merge commit id
  
![image](https://github.com/user-attachments/assets/796e647c-fd2e-485e-9217-1a2ff2d22e00)














- Git pull --rebase # it will fetch the missing the commit id and recent commit id will placed on the top
  
![image](https://github.com/user-attachments/assets/a6203564-5952-4ecc-88ff-7897adb5d6f1)











![image](https://github.com/user-attachments/assets/08c7875b-f28e-4867-8d9e-572d1f26cef7)

# MERGER CONFLICTS ON SAME FILE OR DIFFERENT FILE
- Git pull –ff #minor changes only use this based on commit id is diff means it will not work
- I am add one file in remote repo and using git pull how it will let’s see
  
![image](https://github.com/user-attachments/assets/2b31b55d-5f98-4323-ac69-e3efeaaea328)










- then use the git pull for both os
- then change in code for one line and add, commit changes, push
- Then execute the same change in same line code in windows os and check the errors
  
![image](https://github.com/user-attachments/assets/bbc81593-2fc6-4fb4-a286-0d35ead270da)









- git log --oneline --all --graph # it shows the graphical representation
  
![image](https://github.com/user-attachments/assets/ef07b592-7d8c-432c-9b79-90f87818bf51)








# Git cherry pick # if we want merge specific commit into upstream branch (like main) cherry pick will help us 
- git cherry-pic <committed>
- git push origin<branch name>

![image](https://github.com/user-attachments/assets/d8f68d92-4cd5-4709-a762-c349918b1c4e)
![image](https://github.com/user-attachments/assets/42c0f10e-cf9b-429d-b27c-de92f0d12f2c)
![image](https://github.com/user-attachments/assets/b76533d5-6faf-42eb-8ae3-149e2fbc5a55)












# Git restore # This cmd can use for undo the changes in working dir only 
- Git restore <filename>

![image](https://github.com/user-attachments/assets/2f1c9cc0-6ebc-4e1c-bd9e-83763518954f)
![image](https://github.com/user-attachments/assets/3ae9db4d-f489-4590-a4f1-cefec55f67e1)









# git stash
- Git stash push <filename>

![image](https://github.com/user-attachments/assets/9626af33-6136-4123-86d0-268fd83b0c63)







- Git stash list
- 
![image](https://github.com/user-attachments/assets/2fa5ba40-113b-47db-b1e1-cf76e23945e8)









- git stash apply stash@{0} #  It act for a reback the file into the stagging area
  
![image](https://github.com/user-attachments/assets/2fcfe146-5479-47ff-8c2b-eda5532671e0)







- git stash pop stash@{0} # it act for a Dropped stash
  
![image](https://github.com/user-attachments/assets/81152e1f-70c6-4828-9401-3df2cabd4b04)









- git stash clear # clear the all stash files
  
![image](https://github.com/user-attachments/assets/35527688-d171-4b7b-9c88-831f53263e51)











- git revert <commit_id> # it can create a extra commit id and clear the data in the file. This is use for after the commit_id
  
![image](https://github.com/user-attachments/assets/673152a6-79ff-43b8-af05-e71e3950827f)









- Git reset # git reset changes your branch’s history or staging area, depending on the mode you use:
  
![image](https://github.com/user-attachments/assets/78b6f328-fba0-4379-8d66-814c96bc72cb)

![image](https://github.com/user-attachments/assets/ccdd42ab-5dff-424a-9620-b89a4099d81d)
![image](https://github.com/user-attachments/assets/048bd8a9-df90-4958-8a14-f46a08d2e148)








- Git diff # it show the changes between in the working and stagging area
  
![image](https://github.com/user-attachments/assets/ec307b5f-647b-47f8-95be-9eed6c2804ef)







- Git diff --staged
  
![image](https://github.com/user-attachments/assets/12af24f5-0b3f-4773-bdbc-207933a5669d)






- Git diff head #
  
![image](https://github.com/user-attachments/assets/2a61ed2a-f2f6-4413-b3d4-8ea18f5a33ef)






# Git pull = git fetch + git merge # pull remote repo
- Git pull <remote url>
- Git merge <branchname> merging the dev in main branch
  
![image](https://github.com/user-attachments/assets/55f3e6c3-5f1f-4fa2-a812-3d208782bd14)
