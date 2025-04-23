# Google Cloud Platform - 6.5 Class Notes - Taught by Theo WAF aka Mookie aka Suge WAF @ CloudRow Records ☁️ 😁  - April 22, 2025

## Step by Step Notes & Diagrams

1. Open Gitbash on your Windows desktop, or Terminal on your Macintosh desktop, then click on "Run as Administrator" (DON'T USE POWERSHELL!!!)

![1](https://github.com/user-attachments/assets/0a57e1f0-8069-43e8-a689-42cb9e08f1e7)

   
2. Inside Gitbash Terminal, type in PWD (Present Working Directory) to find your current location. As you can see in the diagram listed below, I'm currently located in my Users directory called Larva. I need to change my current location to the Documents folder. 

![2](https://github.com/user-attachments/assets/d13c0752-5233-4f8b-8c97-bc97dc8081aa)


3. To navigate to the Documents folder, we need to list the directories, and change directories one by one. To list directories, type LS. 

![3](https://github.com/user-attachments/assets/8a2f1c2d-6062-4e1c-85b8-5ef901d9b0f1)

4. The listed directories will be shown from the previous command and now we see our Documents folder, let's input the command cd Documents/ to change our location to Documents. Then, input the command pwd to see our current location, and input the command ls, to list our directories and files in the Documents folder. 

![4](https://github.com/user-attachments/assets/3711a9f7-f8fa-4aa1-a7ea-1a609b8103f5)

5. Input the command cd TheoWAF/ to change our location to TheoWAF folder. Input the following command ls, to list the directories in the TheoWAF folder. We're looking for the folder called class6.5. So input the command cd class6.5/ to change directory location to that folder.

![5](https://github.com/user-attachments/assets/061f6296-e38e-4781-9cec-9c4faa9681e2)

6. Now that we're inside the class6.5 folder, let's input the command ls to list directories inside of that folder and we see a folder called gcp. SIDENOTE: If you don't have a directory named GCP, input the following comamnd mkdir gcp if you don't have gcp folder. We want to go to that folder, so input the command cd gcp/. Type ls to list the directories inside of the gcp folder. We see a folder called terraform, input the command cd terraform/ to go to that location. ANOTHER SIDENOTE: If you don't have the directory inside named Terraform, input the command mkdir terraform if you don't have terraform folder. Input the command ls to list any directories or files, and in the image below, we see no content and this is our destination. HOO-RAY!

![6](https://github.com/user-attachments/assets/e23fb97c-07f8-41f4-9c59-6b6f9e811d4d)

6. PUBLIC SERVICE ACCOUNCEMENT: DON'T STORE YOUR FILES/CODE/OR WORK IN ONEDRIVE (You'll be forever sent and stuck in Cloud Purgatory, and we won't be able to help you...sorry☹️)

![7](https://github.com/user-attachments/assets/e2bc4b36-4a3e-44b4-ae34-d173987a3261)



8. In GitBash, this is the folder you're going to store your current repo -> cd Users/Documents/TheoWAF/class6.5/GCP/Terraform/
9. Here is a list of CLI Commands To Know For The Future, we will be using these later:

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

11. At the present location in Gitbash CLI, create a new folder with the 'mkdir' command, call it whatever you want. I'm calling my directory, lizzolikesyou. Then input the command ls to confirm that you've created the directory.

![8](https://github.com/user-attachments/assets/312a8db5-c38b-4f62-8e2b-d159679201de)


13. Alright, open up your favorite browser, open the url https://www.github.com, go to your github, click on repositories, and click on the New button to create a new repository.

![9](https://github.com/user-attachments/assets/c2c1e115-5723-446b-be87-12b650a4f766)


14. Create a new repo, name it whatever, make it a Public Repo, click on Create Repo.

![10](https://github.com/user-attachments/assets/894e20de-248c-497c-9bd0-61be09e78cdf)

15. For the love of God, on this page that says "Quick setup - if you've done this kind of thing before", create a new tab and NEVER click off this page!!!

![11](https://github.com/user-attachments/assets/bd7254db-77af-4acd-b779-e4f96c77f9be)


16. Click on copy ...create a new repository on the command line, screenshot it, whatever...copy that to your notepad

![12](https://github.com/user-attachments/assets/839044eb-54b5-4f91-881c-2a49b879b5f9)

` https://github.com/LarvariousM/ihatelizzo.git `

17. Go back to your Gitbash, and input the command `git clone` to clone your repo from Github to the folder location you've created inside terraform in the CLI.

![13](https://github.com/user-attachments/assets/cd9cb327-31f1-45da-9d54-18fbfa365618)

18. Add a file to your repo from gitbash -> echo "# sample1" >> README.md
19. Add another file and add text to the file by doing this by checking the end of the echo command -> echo "i dont know" >> idontknow.txt
20. Use the command 'cat' to see inside your txt file -> cat idontknow.txt
21. In Gitbash, run 'git init'
22. git status
23. git add .
24. git status
25. git commit -m "add a comment here"
26. git branch -M main
27. git remote add origin "your git repo link here"
28. git push -u origin main
