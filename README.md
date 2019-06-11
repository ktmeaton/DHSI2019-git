# DHSI2019
DHSI 2019 Git Tutorial

https://ktmeaton.github.io/DHSI2019-git/  

Author: Katherine Eaton  

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
**Commits** - Like the "Save As" function of Git. This will shows all the saved changes to each file.  
**Branches** - Project development isn't always linear. You can maintain forks or branches of a project if you feel an aspect has changed significantly.  
**Releases** - If your project has reached a major milestone (yay you got published!!) this is where you provide highly-visible major releases for your audience.  
4. Dropdown menu "Branch: master", this is where you can change between the different branches of your project.  
5. Button "New Pull Request", pull requests are how a project gets merged between different development branches. This can occur just for one user (a researcher testing out different development ideas) or between collaborators.  
6. Buttons "Create new file/Upload file/Find File" simplistic file management in the web browser. There are better options we will demonstrate later, but it works all the same.  
7. Button "Clone or download": this button is to download an entire repository to your computer. You can use the "Download Zip" option if you're interested in using the repository content without developing or contributing. "Cloning" is what we will be doing later in this tutorial to download files but keep them in a format that still allows for git tracking and version control.     

## Part 4. Install the GitHub Desktop Client 
1. Download GithubDesktopSetup from https://desktop.github.com/  
2. Run the Installer.  
3. Sign in to GiHhub.com through installer.  
4. Configure Git to your preferred name and email.  
5. Decide on sending usage stats.  
6. Select demo repository (ktmeaton/DHSI2019-git) and select **“Clone”**.  
7. Choose the “Local path” where you want your project files to be installed to. 

## Part 5. Client GUI Walkthrough
1. Navigation bar at the top (File, Edit, View).  
2. Below is the repository options, first is the repository (project) selector, then the **branch** selector, then the file fetcher. Fetch is not immediately relevant to us, because fetching is what you do when you want to see what everybody else has been working on.   
3. The left panel controls what displays in the main window of the client.    
4. Right now “changes” is selected and there are no changes to our files.  
5. But in the history tab, something has happened. We have an “Initial **commit**”.  
User “Katherine Eaton” 1 changed file our README.md, [+] for additions being made, and added 2 lines.	
6. Let’s view where our local files are.  

## Part 6. Changing Files  
1. Using the text editor of your choice, add the line  “Author: MyName” to your README.md file.  
2. In GitHub Desktop, we now have Changes.  In the bottom by your profile picture, write “Add repository author” as a comment for the change you’re about to **commit**.  
3. Optional, add a description. Then commit to “master”.  
4. We’ve committed our change, and now it’s prompting us to “push” this to the “origin remote”, which is git language for “would you like to sync this to the cloud?” Click “push origin”.  
5. Now if we view on github, the README.md page has the author line we just added.  

## Part 7. Adding Files  
1. Using your file explorer, create a folder called "writing" in the git repository (same place as the README.md).  
2. Place a document of some type in there (ex. pdf, txt, etc.) Mine will be an empty Word doc called paper.docx.  
3. In the desktop client, comment the **commit** “create paper.docx”, commit the change, and push to the origin remote.  
4. Create folders called "data" and "code" in the git repository".  
5. Create empty text files "text-analysis.py" and "data-visualization.R" in the "code" folder.  
6. In the desktop client, comment the  **commit** “added text analysis and viz code”, commit the change, and push to the origin remote.  
7. View your files on GitHub in the web browser.  

