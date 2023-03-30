# Task-5.-CI-CD-Pipeline-with-jenkins-and-Github
This repository aims to build CD-CI pipelines for sample project- 
https://github.com/pranayDgr8/node-todo-cicd
using jenkins.

Launch EC2 instance with ubuntu

![image](https://user-images.githubusercontent.com/63444224/228719870-2613d205-11f9-4023-8d98-dd76872a9c8a.png)



install java jdk(command 3,4 in commands file)
install jenkins(cmd 5,6,7,8)
this will generate IP for jenkins on port 8080

![image](https://user-images.githubusercontent.com/63444224/228721640-32ece974-8e02-4ab4-abf8-51653f03d8b3.png)








we need allow this IP on port 8080 .This can be done from EC2->instances->Security->Inbound Rules->Edit InBound Rules

![image](https://user-images.githubusercontent.com/63444224/228722092-2c48d8a7-6cc2-451d-83bd-5a83723de2b0.png)






Now go to IP:8080, jenkins will ask for authentication key.

cmd 5 will generate key which can be used to authenticate jenkins.
after authentication user cn create login and password for jenkins.
After logging to Jenkins create new ITEM.
Give item name and github link of sample code whose pipeline needs to be built.




![image](https://user-images.githubusercontent.com/63444224/228722586-903ae5b0-18cd-461c-ae65-a13d113fbabf.png)




Jenkins will be integreated to github.

![image](https://user-images.githubusercontent.com/63444224/228722741-ca4507ed-da20-49c0-853b-c131cfd25749.png)


After integration follow the instructions that developer has mentioned in the readme.This will run the app in the github.


This process can be done using docker 

Install Docker(cmnd 14)
Create Dockerfile and add commands(cmnd 15-20) to that file.
Run docker file in demon mode(cmnd 21,22,23)
![image](https://user-images.githubusercontent.com/63444224/228724086-86166b89-694f-4600-a47a-f08c719c0676.png)

This process can be furthur automated in jenkins.
Follow the instructions 24 - 27.
Add docker commands to jenkins Shell.
![image](https://user-images.githubusercontent.com/63444224/228726483-80213ee0-73a5-4cc3-bf72-5cadd32cb35d.png)

Build the script in jenkins.
![image](https://user-images.githubusercontent.com/63444224/228726654-d20628c1-1551-4c92-aa18-5e3dcaae687e.png)


Allow port 8000 in EC2 inbound rules before running.
The developer's would run in port 8000.

![image](https://user-images.githubusercontent.com/63444224/228726951-373d7556-f67a-4946-ab05-999f494e28ec.png)

