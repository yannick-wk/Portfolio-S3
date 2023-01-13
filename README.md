# Portfolio-S3 / Readers guide
This repository will be dedicated as my portfolio for S3 FHICT. The format of this repository will be developed during this semester.

## Learning outcomes
For an overview of all learning outcomes for this semester, click [here](Documents/learning-outcomes.md).

## Individual project
My project called Happilly, it's a Medicine Reminder application where the user can set reminders for their medicine intake. The project with all the repos and other files can be found in [the Front-end Github](https://github.com/yannick-wk/Happilly-Frontend) and [on the Back-end GitHub](https://github.com/yannick-wk/Happilly-Backend).

## Group project
In this semester we're also tasked with working on a project within a group. The repository for this project can be found [here (Frontend)](https://github.com/JSchuurmans03/WoC-Frontend) and [here (Backend)](https://github.com/JSchuurmans03/WoC-Backend).

## Self-evaluation
### Web application
###### You design and build user-friendly, full-stack web applications

By conducting research on design and selecting the appropriate front-end tools for my project, creating user stories, establishing requirements, reviewing them, and utilizing a framework such as Quasar, I developed a full-stack web application using Quasar (Vue), C# for the back-end and Entity Framework as ORM with a PostGreSQL Database. And I have done a UX research that can be found [here](Documents/ux-research.md) I believe that I have demonstrated proficiency in this learning outcome. 

#### UX 
As per the feedback received in the UX Research/tests, it has been noted that the homepage is too hard to navigate to and it is too difficult to see some buttons. I need to simplify the majority of the elements to make it more user-friendly. Also, the logo functionality was not clear to the majority of participants, because on most websites it leads back to the home page, I need to make separate "back" and "back to reminders/medicine" buttons for better navigation. The medicine page was generally understood well, but minor UI changes were requested. The Reminder page needs to change a little bit as well. I will be implementing these changes and will be conducting another round of feedback to see if the problems are resolved.

#### What went well?
Having the idea for what kind of app I wanted to make made it easy for me to start researching and prototyping early. The creation of the back-end was done in C# and went well but instead of using a standard SOLID structure I wanted to try using [Clean Architecture](Documents/clean-architecture.md). I implemented it into my API project and learned a lot about the differences, for my application it might not have been needed but it was nice to learn and know what I can use in the future. For the front-end I got a running app pretty quickly but still very bare. I had to learn Quasar (vue3) but I got the hang of it quite quickly. Setting up the database with Entity Framework was succesful with relations between tables and I even got it to host on a Docker network with the API. For Distributed communications I used async methods in the front and back-end and made a prototype using SignalR which can be found [here](Prototypes/SignalRProto/).

#### What didnt go well?
I think because I was trying to do too many things at the same time, like researching and having big plans for the application, I got lost quite quickly and it put me off track. A difficult part for me was definitely getting back into working on the app itself after having been distracted by researching so much. But after having feedback conversations with Hans I got back on track. 

#### What am I going to do better next time?
Writing things down and project planning. Because I lost track I didn't know where I left off anymore and it really slowed down my progression in my application development. Just overall programming more would help me too because I noticed that I progress quite quickly when I do.

### Software quality
###### You use software tooling and methodology that continuously monitors and improve the software quality during software development

I have used tools such as Postman/Swagger to ensure that all endpoints in my system are functioning correctly and returning the appropriate data. Additionally, I have used Sonarcloud to verify the quality of my code and test automatically with an in-memory database whenever I push code and will be able to see the coverage on Sonar Cloud of the pushed code. More tests were made with JMeter and Cypress for End to End tests, Performance tests and UX tests. I have also conducted research on OWASP Security and how it was used in my project. Through these actions, I believe that I have demonstrated proficiency in this learning outcome. More on Quality Assurance [here](Documents/quality-assurance.md)

#### Quality Assurance
Looking back at the semester I learned a lot about testing and types of testing. I figured out how to test with JMeter, Cypress and UX tests. I was already familiar with integration tests but I didn't make a lot of them in the past. Now I know how to and in the other types/programs. I struggled with integration tests the most because it was more about testing all the ins and outs of the back-end itself and where everything went through with each test/method. And that with Sonar Cloud you can get so much more information about the code quality. It really helped a lot and I will definitely be using it again.

#### What went well?
Setting up new types of tests, automating some of them and finding out about new types of tools to do so. Automatically running code analysis with Sonar Cloud, it was setup pretty quickly. End to End testing with Cypress and Load testing with JMeter. Writing a research document on [OWASP and Broken Access Control](Documents/owasp-security.md) and how it was used in my application with [CORS](Documents/cors-research.md) and the use of UserSecrets in Docker and dotNET.

#### What didnt go well?
What didnt go well is that I delayed doing the security research and thats the reason why I took so long to fix my CORS issue in the Back-end API.

#### What am I going to do better next time?
I want to start earlier and when I have a problem I want to tackle it as soon as possible, ofcourse with the right priorities.

### Agile method
###### You can implement the software process for your project according to a given agile software development method

By utilizing an Agile method that I researched extensively, as seen in the research document [here](Documents/agile.md), and consistently planning and tracking progress in the GitHub environment, I have demonstrated proficiency in this learning outcome.

### Agile method decision
The method I have chosen for both individual and group projects is SCRUM. I chose SCRUM because I am already familiar with the method and have used it successfully in the past. It has always been an effective way to implement agile methodology in my projects. I did consider other methods, but ultimately found that SCRUM best suited my needs. The primary advantage of SCRUM is the ability to work in sprints and observe progress throughout the project. Setting realistic goals and achieving them each sprint, as well as the transparency that allows all team members to see the work of others, are major benefits of the method. Additionally, SCRUM allows for the flexibility to re-prioritize items within the project, allowing for adjustments to the project's focus as needed.

#### What went well?
I had experience with SCRUM and it was easy to apply this semester for my own project as well as the group project.

#### What didnt go well?
In the group project our roles were often unclear using SCRUM. We wanted to rotate roles so we could all have each role atleast once but that led to confusion and I'm looking to improve that next time I start a project. 

#### What am I going to do better next time?
Set roles and stick to them, or try and put it into a document to see who has been which role already and see who's turn it is next.

### CI/CD
###### You implement a (semi)automated software release process that matches the needs of the project context.

Through conducting research on the appropriate tests for my project and the types of tests available, automating a workflow file to execute my test scripts, testing endpoints with Postman/Swagger, testing integrity of the backend, implementing performance tests, testing the entire CRUD system, and running the backend and database on a Docker network with a Docker Compose, I have demonstrated proficiency in this learning outcome. More about CICD can be found [here](Documents/cicd.md).

#### What went well?
I set up a continuous integration and continuous deployment pipeline using Github actions CI/CD for both my API and ORM database. This pipeline automatically runs tests and deploys my application when changes are made and pushed to the main or development branches. To ensure security, I added secret variables for sensitive information such as passwords and keys. Pushing changes to the main branch will trigger a build, deployment, testing and analysis.

#### What didnt go well?
I didn't get the frontend to run on a docker container/network

#### What am I going to do better next time?
I want to run all components of the project on docker network in containers next time I make a project.

### Cultural differences and ethics
###### You recognize and take into account cultural differences when working with multi-site teams, and are aware of ethical aspects in software development

I have conducted research on the topic of Ethics and Culture on its application in the IT industry my own take and experience and based on that, I would currently rate my proficiency in this learning outcome as "Proficient". My research document can be found [here](Documents/cultural-differences-and-ethics.md).

#### What went well?
Researching the topic and immediately recognizing the cultures in different countries with their working culture and their ethics. I also saw the same thing with the ethical aspects in software development and when we had to prepare for the workshop I did the test to see what kind of Team Role I had in a company and what kind of "Color" I think in. 

#### What didnt go well?
I waited too long with researching Cultural differences and Ethics and it stalled my learning progression of this learning outcome.

#### What am I going to do better next time?
Next time I want to atleast do some pre-research so that I atleast have some base of the topic and can later understand it faster and research it.

### Requirements and design
###### You translate (non-functional) requirements to extend existing (architectural) designs and can validate them using multiple types of test techniques

By establishing a range of functional and non-functional requirements, creating user stories, and conducting research on the design approach for my project with an architectural model (C3), I believe that I have demonstrated proficiency in this learning outcome. The design research document can be found [here](Documents/ux-research.md). And the Analysis document can be found [here](Documents/happilly-analysis.md) with requirements, quality attributes and C3.

#### What went well?
I did a UX research with tests on 2 groups of users and got useful results that I later applied to my project.

#### What didnt go well?
The only thing that didn't go well is that I waited too long with the designs.

#### What am I going to do better next time?
Next time I want to design from the start so that I can later see the improvements and changes I made in my project so I can learn from my errors and decisions.

### Business processes
###### You can explain simple business processes and relate them to the development of your software project.

By conducting appropriate research and creating a business process based on a feature within my Happilly system and having done a workshop about the business processes and usermapping stories I would rate my proficiency in this learning outcome as proficient. More about the business process can be found [here](Documents/business-process.md) and the workshop documentation can be found [here](https://github.com/fontys-open-up/2223nj-db03/tree/main/user-story-mapping-workshop)

#### What went well?
Looking back, having done the workshop with user story mapping really helped with understanding and implementing a business process for my own project. I have also made a business process of my own project [here](Documents/business-process.md). 

#### What didnt go well?
I didn't really have issues with the business process it was pretty straight forward.

#### What am I going to do better next time?
I want to make more/more clear business processes. For it to be more clear which steps I should consider for the process.

### Professional
###### You act in a professional manner during software development and learning

Throughout the semester, I have had several feedback sessions with Hans regarding the progress of my application and my learning outcomes. I recorded the details of these conversations using feedpulse. Additionally, I have presented our sprint deliveries to World of Content / Hans (for Happilly), (or other relevant group) and consistently sought feedback from the product owners, and then incorporated that feedback into our/my product. I would rate my proficiency in this learning outcome as proficient. You can view the communication between the stakeholder/coaches and I in FeedPulse.

#### What went well?
Communicating with the coaches, the people at World of Content, my own project group and other groups. I had a weekly feedback appointment with Hans which kept him up to date with what I did every week. This way he could keep track of my progression on my individual project Happilly. Putting the feedback in to FeedPulse was also something that went well.

#### What didnt go well?
With the group project not living up to the expectations of the required products we were supposed to deliver. But that was a good learning moment because, it just shows how important it is to plan something/a project out.

#### What am I going to do better next time?
I'd like to involve both coaches more next time instead of only getting feedback from one. I also want to start using my notes more after taking them because I realized that I dont use them as much as I should.