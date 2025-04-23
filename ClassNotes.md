### Google Cloud Platform - 6.5 Class Notes - Taught by Theo WAF aka Mookie aka Suge WAF @ CloudRow Records ☁️ 😁  - April 22, 2025

##Step by Step Notes & Diagrams

1. Open Gitbash on your Windows desktop, or Terminal on your Macintosh desktop (DON'T USE POWERSHELL!!!)

![1](https://github.com/user-attachments/assets/9d591797-ba56-4cb9-8a77-49400cc599a5)

   
3. Type in PWD (Present Working Directory) KNOW WHERE YOU ARE!
4. LS = Lists folders
5. DON'T STORE YOUR FILES/CODE/OR WORK IN ONEDRIVE (You'll be sorry...)
6. In GitBash, navigate to this folder to store your repo -> cd Users/Documents/TheoWAF/class6.5/
7. Command To Know: pwd: Print the current working directory, ls: List directory contents, cd: Change directory, mkdir: Create a new directory, rmdir: Remove an empty directory, touch: Create a new empty file, cp: Copy files or directories, mv: Move or rename files or directories, rm: Delete files or directories, cat: View file contents, nano: Open file in Nano text editor, chmod: Change file permissions, chown: Change file owner or group, echo: Display a message or variable, clear: Clear the terminal screen
8. Create a new folder with the 'mkdir' command, call it whatever you want
9. mkdir gcp if you don't have gcp folder
10. go to your github, click on repositories
11. create a new repo, name it whatever, click on Create Repo
12. On the next page that says "Quick setup - if you've done this kind of thing before", create a new tab and NEVER click off this page!!!
13. Click on copy ...create a new repository on the command line, screenshot it, whatever...copy that to your notepad
14. Go back to your Gitbash
15. git clone your repo from Github
16. Add a file to your repo from gitbash -> echo "# sample1" >> README.md
17. Add another file and add text to the file by doing this by checking the end of the echo command -> echo "i dont know" >> idontknow.txt
18. Use the command 'cat' to see inside your txt file -> cat idontknow.txt
19. In Gitbash, run 'git init'
20. git status
21. git add .
22. git status
23. git commit -m "add a comment here"
24. git branch -M main
25. git remote add origin "your git repo link here"
26. git push -u origin main
