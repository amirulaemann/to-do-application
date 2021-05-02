# to-do-application

Group 5:
1. Muhammad Amirul Aiman Bin Ysuoff 1826557
2. Herda Binti Borhan 1821690
3. Bhuiyan Md Fahim 1821281
4. Julyana Binti Rahmad 1912068

INTRODUCTION

A to-do app that focuses on a simple daily task. To-do apps are popular with the thousands of apps that are produced each year. There are a lot of to-do list applications available from notepads to digital to-do list application. Some of these applications are free, some are fee-based, but the main objective of all of them is to offer classic task scheduling assistance to help us manage and finish the tasks with ease and on time. The problem with most task applications is 
over-engineering. All we need is simplicity. A to-do app is designed to remind the user what to do. The reason most people download task apps but don't use them is because they lose interest and don't experience the benefits of those apps. Stay on a to-do list with 30 actions. It becomes more of a burden than a solution and we feel negative about the web application. This is where our simple, daily presented web app differs. User interface and includes the user entering a specific day every day. At the end of the day the highlight disappears or can be used as the highlight of the next day. It sounds simple and that's why it's great. Users will gradually get more done over time and feel the advantages of your web application over others. Our web application is simple as every day, user just type in one or more big things they want to do. Then, they can add a few little tasks they might also want to get done. User can check the web application during the day to focus on their goals which can keeps user’s aim on the game. This web application works way better than track daily goals on a sticky note. Not going to lie it worked pretty well but for sure people often forget to fill it out or would lose the paper during the day. That is why we create this together because user can take their phone and gives them a friendly nudge every morning to fill in the tings they want to focus on. 

OBJECTIVE

1.	The simple web application to keep us focused on our biggest task every day.
2.	To offer classic task scheduling assistance to help us manage and finish the tasks with ease and on time.
3.	Develop a clearer idea of exactly what user need to do next and will get through their work faster.

Features

The web application purpose aim is to ease users in their daily life. Users may enter their task that they need to do, and the web application will remind them the task that need to do that they insert earlier. Basically, this web application is like the remainder for the users to use. These are the details of the web application.

Insert Task

The user needs to insert the task into the space provided in the web application. The web application later will store the task that users insert earlier. The data provided will be use for reminding them about the task that they need to do.

Remind

The web application will remind the users about the task that they insert. There will be a percentage that indicate the progress of the task completed. The task will disappear when the day is over, or they can carry the task forward to the next day. Besides that, the web application did not limit the users to have only 1 task a day if they carry the task forward to the next day. It will stack with the new task if the users enter a new task for that day. For example, a user inserts a specific task which is Task Aon Wednesday and when the next day which is Thursday, the Task A will disappear, but the user have a choice to carry the task forward to the next day which is Thursday if the user need it. If the user carry the task A that originally need to complete on Wednesday to Thursday and need to add another task on Thursday which is Task B, it will stack with Task A on that day. So, the web application will remind the user that the user has 2 tasks that need to be done on Thursday which are Task A and Task B.

Views: 

Home.blade.php – Display user tasks and its progress for the day. The main goals of the day will be displayed in the bigger size.
Login.blade.php – Display the Log In page
Register.blade.php – Display the registration page
ViewTask.blade.php – Display all of the tasks added by the user, including the details of the task, and user also can tick off the completed task
AddTask.blade.php – Display the columns that need to be included in the task, such as, name of the task, start and end time, and description.

Controllers:

Home.php – 
•	Allows registered user data to be retrieved from the database
•	Redirect the new registered user to the Log in page
•	Allows user to view main task
•	Allows user to view the percentage of completed task, retrieved from ViewTask.php controller

ViewTask.php –
•	Allows user to view the details of the task by retrieve it from database
•	Allows the percentage of completed task to be calculated

AddTask.php – 
•	Allows user to add main task, including the start and end time
•	Allows user to add subtasks, including the start and end time
•	Allows user to edit and delete task

Routes:
•	Routes/web.php 
-	retrieved all of the tasks added by the user from AddTask.blade.php controller
-	retrieved calculation of the percentage of completed task from ViewTask.blade.php controller

Model:
User has one to many relationships with task
 
![image](https://user-images.githubusercontent.com/61687500/116818249-fb0b4600-ab9c-11eb-9958-7ac7096cc4ec.png)


References:
-	https://laravel.com/docs/8.x/controllers
-	https://laravel.com/docs/8.x/routing
-	Justin Pot. (2020, November 19). The 9 best to do list apps of 2021. 
-	https://zapier.com/blog/best-todo-list-apps/#gtasks
