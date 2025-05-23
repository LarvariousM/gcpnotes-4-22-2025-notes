# Google Cloud Platform - 6.5 Class Notes - Taught by Theo WAF aka Mookie - April 22, 2025

Prerequisites for this Tutorial

* A **GitHub Account**
* A **Git or GitBash Terminal** (should've been installed during the Class 6.5 Installation Walkthrough)




### How To Create A GitHub Account

1. Go to https://www.github.com, and click on the Sign Up Button

![1](https://github.com/user-attachments/assets/6468179d-dfba-4cdf-8e6d-b6026c3a04dc)

2. You'll be taken to this next page, input your **email**, **password**, **username**, **country/region**, and click on the Continue button.

![2](https://github.com/user-attachments/assets/898ce7a4-f53c-405a-8c77-59456309261b)

3. On the next page, you'll be tested to make sure you're not the droid the FBI has been looking for, verify the image!

![3](https://github.com/user-attachments/assets/b1cf7dfe-5516-4214-88e5-ece6a7d4a7a5)

4. You will be sent a launch code/eight digit code to your email. Login to your email and copy this code.

![4](https://github.com/user-attachments/assets/5a0ff9d6-a70c-4aa3-9117-100c5293607d)

5. Come back to this page, and input your code sent to your email.

![5](https://github.com/user-attachments/assets/ce324745-0da1-4546-8f5b-410e122fd296)

6. If done correctly, you'll be directed to this page and your GitHub account has been successfully created. Please sign in to your GitHub account!




### How To Install GIT on your Local Machine (if you didn't install during the Class 6.5 Installation Walkthrough)

1. Go to this website to download the necessary Git file for your computer -> https://learn.microsoft.com/en-us/devops/develop/git/install-and-set-up-git. The webpage will look similar to the image below 

![1](https://github.com/user-attachments/assets/cbea7254-45c1-4d42-9b3c-f79075ebc0fa)

2. Select and click on the necessary installation for your computer.

![2](https://github.com/user-attachments/assets/cd9cc720-8fb9-40ca-8c30-daa50096dffe)

3. I have a **Windows** computer, so I've selected "Install Git for Windows". The download link will take me to this page below.

![3](https://github.com/user-attachments/assets/d0ea4225-05b3-4eed-abcb-144eda3c17d2)

4. We now need to confirm what **System Type (32 bit or 64 bit)** our computer has to select the correct installation. That's very simple, on your computer press the windows button, or go to your Windows search bar located and type in "This PC", and click on Properties.

![4](https://github.com/user-attachments/assets/7a608f82-99a9-49ec-843b-d5b76331be3d)

5. Under **Device Specifications**, you'll see your **System Type**.

![5](https://github.com/user-attachments/assets/d7aae0d3-9d6c-4ccc-accf-e1bd53b9d92d)

6. Return to the previous page and click on the installation type to download Git on your computer. After the download is completed, open up **Powershell (Run as Administrator)**, and input the following command 👉 `git --version`, to confirm that Git has been installed. 

![6](https://github.com/user-attachments/assets/71b190ca-d05b-4c6b-aaa7-2b2b9b2ce714)

7. Press the Windows button on your keyboard or go to the Windows search bar, and type in GitBash and (Run as Administrator).

![7](https://github.com/user-attachments/assets/f5b04b26-63e4-493c-a8a1-0881008ead72)

8. Your GitBash terminal should look like this image below.

![8](https://github.com/user-attachments/assets/60d23cc4-c389-4016-ae9c-1be6e4ead6dd)

There you have it, you've signed up for a **GitHub account** and you've installed **Git** on your computer. We're now ready to RDP and SSH into remote satellites in orbit and launch secret nukes! Just kidding...you're ready to follow along with the rest of this tutorial! Continue on...




## Step by Step Notes & Diagrams for Creating a Repository on Your Local Machine and Pushing It To A GitHub Repository

**Here is a list of CLI Commands To Know For The Future, we will be using these later**

```
{

pwd: Print the current working directory,
ls: List directory contents,
cd: Change directory,
mkdir: Create a new directory,
rmdir: Remove an empty directory,
touch: Create a new empty file,
cp: Copy files or directories,
mv: Move or rename files or directories,
rm: Delete files or directories,
cat: View file contents,
nano: Open file in Nano text editor,
chmod: Change file permissions,
chown: Change file owner or group,
echo: Display a message or variable,
clear: Clear the terminal screen

}
```

**Very Important CLI Commands To Remember In Order To Push/Update Files To An Online GitHub Repository"**

```
{
1. git init
2. git status
3. git add [filenmame], or git add . 👈 [to add multiple files]
4. git status
5. git commit -m "add a comment here"
6. git branch -M main
7. git remote add origin "your github repository url link here"
8. git push -u origin main
}
```

1. Open Gitbash on your Windows desktop, or Terminal on your Macintosh desktop, then click on "Run as Administrator" (DON'T USE POWERSHELL!!!)

![1](https://github.com/user-attachments/assets/0a57e1f0-8069-43e8-a689-42cb9e08f1e7)

   
2. Inside Gitbash Terminal, type in `PWD` (Present Working Directory) to find your current location. As you can see in the diagram listed below, I'm currently located in my Users directory called Larva. I need to change my current location to the Documents folder. 

![2](https://github.com/user-attachments/assets/d13c0752-5233-4f8b-8c97-bc97dc8081aa)


3. To navigate to the Documents folder, we need to list the directories, and change directories one by one. To list directories, type the command `LS`. 

![3](https://github.com/user-attachments/assets/8a2f1c2d-6062-4e1c-85b8-5ef901d9b0f1)

4. The listed directories will be shown from the previous command and now we see our Documents folder, let's input the command `cd Documents/` to change our location to Documents.

Then, input the command 👉 `pwd` to see our current location, and input the command `ls`, to list our directories and files in the Documents folder. 

![4](https://github.com/user-attachments/assets/3711a9f7-f8fa-4aa1-a7ea-1a609b8103f5)

5. Input the command `cd TheoWAF/` to change our location to TheoWAF folder. Input the following command `ls`, to list the directories in the TheoWAF folder. We're looking for the folder called **class6.5**. So input the command `cd class6.5/` to change directory location to that folder.

![5](https://github.com/user-attachments/assets/061f6296-e38e-4781-9cec-9c4faa9681e2)

6. Now that we're inside the class6.5 folder, let's input the command `ls` to list directories inside of that folder and we see a folder called **GCP**.

**SIDENOTE**: If you don't have a directory named GCP, input the following comamnd `mkdir gcp` if you don't have gcp folder. We want to go to that folder, so input the command `cd gcp/`. Type `ls` to list the directories inside of the gcp folder. We see a folder called terraform, input the command cd terraform/ to go to that location. 

**ANOTHER SIDENOTE**: If you don't have the directory inside named Terraform, input the command `mkdir terraform` if you don't have terraform folder. Input the command `ls` to list any directories or files, and in the image below, we see no content and this is our destination. HOO-RAY!

![6](https://github.com/user-attachments/assets/e23fb97c-07f8-41f4-9c59-6b6f9e811d4d)

6. **PUBLIC SERVICE ACCOUNCEMENT**: DON'T STORE YOUR FILES/CODE/OR WORK IN THE ONEDRIVE FOLDER (You'll be forever sent and stuck in Cloud Purgatory, and we won't be able to help you...sorry☹️)

![7](https://github.com/user-attachments/assets/e2bc4b36-4a3e-44b4-ae34-d173987a3261)



7. In GitBash, this is the folder you're going to store your current repo 👉 cd Users/Documents/TheoWAF/class6.5/GCP/Terraform/

8. At the present location in Gitbash CLI, create a new folder with the `mkdir` command, call it whatever you want. I'm calling my directory, lizzolikesyou. Then input the command `ls` to confirm that you've created the directory.

![8](https://github.com/user-attachments/assets/312a8db5-c38b-4f62-8e2b-d159679201de)


9. Alright, open up your favorite browser, click on the address bar, and type in the url address https://www.github.com, go to your github, click on repositories, and click on the New button to create a new repository.

![9](https://github.com/user-attachments/assets/c2c1e115-5723-446b-be87-12b650a4f766)


10. Create a new repo, name it whatever, make it a Public Repo, click on Create Repo.

![10](https://github.com/user-attachments/assets/894e20de-248c-497c-9bd0-61be09e78cdf)

11. For the love of God, on this page that says **"Quick setup - if you've done this kind of thing before"**, create a new tab and **NEVER DELETE** this page\tab!!!

![11](https://github.com/user-attachments/assets/bd7254db-77af-4acd-b779-e4f96c77f9be)


12. Click on copy ...create a new repository on the command line, screenshot it, whatever...copy that to your notepad

![12](https://github.com/user-attachments/assets/839044eb-54b5-4f91-881c-2a49b879b5f9)

` https://github.com/LarvariousM/ihatelizzo.git `

13. Go back to your Gitbash terminal, and input the command `git clone "https:github.com/YOURUSERNAME/REPO.GIT"` to clone your repo from Github to the folder location you've created inside terraform in the CLI.

![13](https://github.com/user-attachments/assets/cd9cb327-31f1-45da-9d54-18fbfa365618)

14. Add a file to your repo from gitbash, by inputting this command 👉 `echo "# sample1" >> README.md, insert command`, then run this command `ls` to confirm that the file has been created.

![14](https://github.com/user-attachments/assets/2015641a-d633-473e-b295-66d6aecc8cbd)

15. Add another file of your choice and add custom text to the file by doing this by checking the end of the echo command 👉 `echo "i dont know" >> idontknow.txt`. You can read what the txt file contains by inserting the command -> `cat idontknow.txt`

![15](https://github.com/user-attachments/assets/611d5904-56af-4ada-a4aa-4b607899e96d)

16. We now have two files inside our repo, and the next objective is to push these files from Gitbash to GitHub. In order to accomplish that, go to your Gitbash terminal, make sure you're still located in the repo folder by inserting this command -> `pwd`, then insert the command 👉`'git init'` to initialize your GitHub.

![16](https://github.com/user-attachments/assets/8e9074e3-cb2d-42c2-adc1-ea054ae1c972)

17. Next, we're going to check the status of our Git Repository to see what files are being tracked and what files are not being tracked, by inserting this command 👉 `git status`. As you can see in the diagram below, we have two files that are not being tracked on our local machine, and we need to track them from our local machine to the internet in order to push them to GitHub.

![17](https://github.com/user-attachments/assets/57fbb4cc-bc4a-4bd4-bbb8-1100879c075a)


18. In order to track these two files and push them to the GitHub, you have two options. The first option is by adding one single file by inserting the command 👉 `git [filename]`, or the second option is to add all files by inserting this command 👉 `git add .` I'm going to use the second option!

![18](https://github.com/user-attachments/assets/1864e831-e5af-4d75-b638-928dd3da10dc)

19. Let's now check and see if the two files are now being tracked so that we can commit and push them to our GitHub repository, by inserting this command again -> `git status`

![19](https://github.com/user-attachments/assets/98e3f30e-b4ba-40c8-9feb-62692072632c)

20. We now have both files being tracked and they are now ready to be commited to our online GitHub Repository, we can commit them by inserting this command 👉 `git commit -m "add a comment here"`. SIDE-NOTE: Each time you commit files to an online GitHub Repository, give a clear and concise reason as to why you're committing these files to the GitHub Repository, because you may be working with a team or other individuals and they need to know what changes were made, in case they may need to revert back to older files in case there was a mistake. VERY IMPORTANT!


HOWEVER, I ran across an error that tells me that `"Author identity unknown"`. This means that my GitBash/Powershell does not know who I am, and I need to identify myself first from GitHub. 

![20](https://github.com/user-attachments/assets/d36ea20c-919d-4be6-a764-ef8748f325bb)

In order to remedy this error, I need to configure my GitHub account to the GitBash terminal, and we can do that by inserting the command -> git config --global user.name [YOUR GITHUB USERNAME], and git config --global user.email [YOUR GITHUB EMAIL ASSOCIATED WITH GITHUB]. We can verify that our GitHub account is associated with our GitBash terminal by running these two commands, 👉 `git config user.name`, and 👉 `git config user.email`

![21](https://github.com/user-attachments/assets/87ac358a-50f2-4bfb-9191-330cbf16f7a3)

21. Now, let's try to run the command 👉 `git commit -m "add a comment here"` again to see if it works. It works!!! Both files have been committed to our GitHub Repository, but we're not done yet. 

![22](https://github.com/user-attachments/assets/2ca1b4ed-1421-4a38-b77d-de519c19a1d8)

22. Let's set our correct branch in the GitHub Repository, by running this command 👉 `git branch -M main`

![23](https://github.com/user-attachments/assets/b1273f09-c688-4222-b4b5-3ae342f825d3)

23. Do you remember the time? That time we created an empty GitHub Repository online and I told you to not delete that page??? Well...we need to go back there and locate our GitHub Repository link, and run this next command in GitBash 👉 `git remote add origin "your git repo link here"`.

![24](https://github.com/user-attachments/assets/b66df70e-adc8-45a5-9d42-bf7833e9e312)

I received this error message above because I've already associated this folder from GitHub earlier in one of our steps. Otherwise, if you receive this error message or not, please continue. We're almost done. 

24. Finally, we're ready to push these files from our local machine to our online GitHub Repository. Run this final command to push those said files 👉 `git push -u origin main`

After running this command, you may receive this dialogue box requesting you to sign in to GitHub. Click on [Sign on with Browser]

![25](https://github.com/user-attachments/assets/41a518e4-145c-4329-b269-0e24f6187294)

You receive this code when your files have been pushed to the online GitHub Repository.

![26](https://github.com/user-attachments/assets/bed89d27-fd10-49a6-96a6-9950b0c39fa4)

We can also confirm in the browser if our files have been pushed to our GitHub Repository. 

![27](https://github.com/user-attachments/assets/8de582b4-e42b-45b2-a3b5-e1305f18b0a1)

That's all folks, we have created an empty GitHub repository online, created files in the GitBash terminal on our local machine, and pushed them to our online GitHub Repository.

