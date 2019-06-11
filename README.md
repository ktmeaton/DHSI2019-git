# DHSI2019-git
DHSI 2019 Git Tutorial

https://ktmeaton.github.io/DHSI2019-git/  

Author: Katherine Eaton  
Created: 2019-06-10

## Part 1. Create a GitHub Account
1. Navigate to https://github.com/  
2. Create an account.  
3. If it doesn't automatically do so, login.  

## Part 2. Create a Repository (ie. Cloud-Based Project)
1. Navigate to your account home (click the cat icon in the top left).   
2. Create a new repository by clicking the green "New" box.   
3. Name your repository (ex. "DHSI2019-git").  
4. Give it a short description ("DHSI 2019 Git Tutorial").  
5. Decide on your privacy settings (public vs. private).  
6. Select “Initialize this repository with a README”.  
    - The README will be a text file in Markdown format and will be the landing page for your project.  
7. Leave the other settings as the default.  

## Part 3. Web-Browser Repository Walkthrough
1. The tabs at the top (Code, Issues, Pull requests...) are for your development use. Code is where all your project files are stored.
2. "Watch" and "Star" are the social media platform options of GitHub (Follow and Like)
3. The next section of tabs (Commits, 1 branch, 0 releases, environment, 1 contributor) relate to the activity and history of your repository.  
- **Commits** - Like the "Save As" function of Git. This will shows all the saved changes to each file.  
- **Branches** - Project development isn't always linear. You can maintain forks or branches of a project if you feel an aspect has changed significantly.  
- **Releases** - If your project has reached a major milestone (yay you got published!!) this is where you provide highly-visible major releases for your audience.  
4. Dropdown menu "Branch: master", this is where you can change between the different branches of your project.  
5. Button "New Pull Request", pull requests are how a project gets merged between different development branches. This can occur just for one user (a researcher testing out different development ideas) or between collaborators.  
6. Buttons "Create new file/Upload file/Find File" simplistic file management in the web browser. There are better options we will demonstrate later, but it works all the same.  
7. Button "Clone or download": this button is to download an entire repository to your computer. You can use the "Download Zip" option if you're interested in using the repository content without developing or contributing. "Cloning" is what we will be doing later in this tutorial to download files but keep them in a format that still allows for git tracking and version control.     

## Part 4. Creating a Webpage
1. Navigate to your repository's home page on GitHub (ex. https://github.com/ktmeaton/DHSI2019-git).
2. In the tab panel (same level as "Code"), click on Settings (Gear Icon) and scroll down to "GitHub Pages".
3. For the Source dropdown menu, select the master branch.
4. For the website Theme Choose, pick a design layout (ex. Cayman)
5. You now have a \_config.yml file in your home directory. Also in Settings under GitHub Pages it will be checkmarked and say “Your site is published at https://ktmeaton.github.io/DHSI2019-git/”
7. Check it out! By default it is your README.md file. Github Pages are websites powered by Jekyll, checkout the documentation for more options.

## Part 5. Install the GitHub Desktop Client 
1. Download GithubDesktopSetup from https://desktop.github.com/  
2. Run the Installer.  
3. Sign in to GitHub.com through installer.  
4. Configure Git to your preferred name and email.  
5. Decide on sending usage stats.  
6. Select demo repository (ktmeaton/DHSI2019-git) and select **“Clone”**.  
7. Choose the “Local path” where you want your project files to be installed to. 

## Part 6. Client GUI Walkthrough
1. Navigation bar at the top (File, Edit, View).  
2. Below is the repository options, first is the repository (project) selector, then the **branch** selector, then the file fetcher. Fetch is not immediately relevant to us, because fetching is what you do when you want to see what everybody else has been working on.   
3. The left panel controls what displays in the main window of the client.    
4. Right now “changes” is selected and there are no changes to our files.  
5. But in the history tab, something has happened. We have an “Initial **commit**”.  
User “Katherine Eaton” 1 changed file our README.md, [+] for additions being made, and added 2 lines.	
6. Let’s view where our local files are.  

## Part 7. Changing Files  
1. Using the text editor of your choice, add the line  “Author: MyName” to your README.md file.  
2. In GitHub Desktop, we now have Changes.  In the bottom by your profile picture, write “Add repository author” as a comment for the change you’re about to **commit**.  
3. Optional, add a description. Then commit to “master”.  
4. We’ve committed our change, and now it’s prompting us to “push” this to the “origin remote”, which is git language for “would you like to sync this to the cloud?” Click “push origin”.  
5. Now if we view on github, the README.md page has the author line we just added.  

## Part 8. Adding Files  
1. Using your file explorer, create a folder called "writing" in the git repository (same place as the README.md).  
2. Place a document of some type in there (ex. pdf, txt, etc.) Mine will be an empty Word doc called paper.docx.  
3. In the desktop client, comment the **commit** “create paper.docx”, commit the change, and push to the origin remote.  
4. Create folder "code" in the git repository.  
5. Create empty text files "text-analysis.py" and "data-visualization.R" in the "code" folder.  
6. In the desktop client, comment the  **commit** “added text analysis and viz code”, commit the change, and push to the origin remote.  7. Create folder called "data" in the git repository.  
8. Create empty text files "raw-data.txt" and "processed-data.txt in the "data" folder.  
9. In the desktop client, comment the  **commit** “added raw and processed data”, commit the change, and push to the origin remote. 
10. View your files on GitHub in the web browser.  

## Part 9. Syncing Changes (Browser - Desktop)
1. In the GitHub web browser, navigate to the file data/raw-data.txt and click the small pencil icon to edit it.  
2. Add the line “Rawdataisn’tsobadright?”  
3. In the GitHub Desktop client, make sure that “Changes” is the panel that is selected. Click the fetch origin button at the top panel next to “Current repository” and “Current branch”. The main window should pop up saying that “1 commit from the origin remote” is available.  
4. Click “pull” to fully download that changed file. If you open up code/raw-data.txt on your local computer, you will see that it now also has our new line.  

## Part 10. Some Basic Time Travel (ie. Revert)
1. Add a line to the file code/text-analysis.py "This line of code works as expected."  
(Desktop Client: Comment "Works as expected", commit, push)  
2. Add another line to code/text-analysis.py "This line of code breaks the entire project!!!"  
(Desktop Client: Comment "Didn't test this change", commit, push)  
3. Add another line to code/text-analysis.py "This line of code is neutral."  
(Desktop Client: Comment "This doesn't work anymore", commit push)  
4. Change the left panel to the tab "History".  
[**WARNING: Major error alert upcoming**]  
Github Desktop must perform reverts one by one, and step by step in reverse chronological order. If you try to revert a commit that is NOT THE MOST RECENT commit in Github Desktop, you will generate major error that must be solved with command-line programming knowledge. If this happens and you do not have this knowledge, please delete your github project folder from your file browser and the Github Desktop client should automatically prompt you to clone your repository again. You can then restart Part 10 from Step 4.  
5. Right click on the history event "This doesn't work anymore", select Revert This Commit.  
6. A new event has occurred in the history: Revert "This doesn't work anymore". Select it with your mouse and you will see that the last line has been deleted (minus sign). But we have one more change to undo.  
7. Right click on the history event "Didn't test this change", select Revert This Commit.   
8. Another new event has appeared: Revert "Didn't test this change". Select it with your mouse and you will see the code-breaking line was deleted. Our text-analysis.py has been reverted to a functional state. But we need to commit those changes.  
9. This time, no comment is needed as the "Revert" comment has been applied. Simply click "Push origin". View on GitHub and go look at that file.  
 
**Advanced Time Travel (ie. Checkout, Revert, Reset)**  
10. Advanced time travel requires command-line usage of git.  
11. Atlassian has excellent tutorials on how to undo changes and revert to previous states of projects or specific files.  
https://www.atlassian.com/git/tutorials/undoing-changes  

## Part 11. Collaboration (Self)
1. In Github Desktop, select the “Current Branch” dropdown menu in the top panel. Click the new branch button, and call it “self-collaboration”. Click publish branch.  
2. Click the “View on Github” and use the “Branch: master” dropdown menu to confirm that a self-collaboration branch was created. For now, it is identical to the master branch.  
3. The Github Desktop client now will constantly prompt you with a new option to “Create a Pull Request” which is how you would propose your changes to a collaborator (or in this case to yourself).  
4. In your computer’s text editor, open the file code/data-visualization.R and add the line “self-collaboration proposed changes: color-blind friendly palettes for data visualization!”  
5. In Github Desktop, comment and commit. Note that it now says “Commit to self-collaboration”. Click the button “Push origin”.  
6. This change now exists only on the self-collaboration branch, not on the master branch. You can explore this difference on the GitHub browser if you’re interested.  
7. Click “Create a Pull Request” which will automatically redirect us to an github in an internet browser where our proposed change is being explained. The dropdown menus indicated that branch base:master is receiving <- a change from the branch self-collaboration, and the checkmark indicates there are no conflicts.  
8. Write an informative description of the change, then click “Create pull request”.  
9. To accept the merging of branches, click “Merge pull request” and then “Confirm”  
10. The master branch now the file changes that were made in our self-collaboration branch.  
11. In Github Desktop, switch the branch to master, fetch the updated changes from the origin, and pull the changes we’ve just made.  
