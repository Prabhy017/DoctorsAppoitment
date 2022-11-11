# DoctorsAppoitment
Asp.net application for booking doctor appoitment


About the project
---------------------------------------
Implemented Asp.net core web application which can be deployed to different VMs. The application shows the apointments for both 
patient and doctors.Both can register themseleves with their phone number and few details. Patients can book appointments
with doctor from a specific department.

The visio diagram is availble which showcases the architechture for High availability and Disaster recovery.

The Database can be implemented in azure sql database.The script for creation of tables is attached.The connection string can be added
in the appsettings json file in the web app.

Implemented DAL and Entity C# class library for Entityframnework.

Added different Apis which can be used as a microservice to fetch appointments and other actions.

Designed two screens for Registering new user and signing in.Couldn't complete the action part because of less bandwidth.



Auto Deployements
---------------------------------------------
Azure Devops CI/CD can be implemented for commiting the code to the Git Repository and then deploying it into different environments
through the pipelines. 

Developers can create a feature branch from the latest Dev branch and can do their changes.Once done they can create a pull
request to merge the code into the main branch.Any other senior developer can do the review of the changes done and then will
approve for merge codes.
Once the changes are added to the main branch we can run the pipeline for deploying it to different environments.
We will deploy it to DEV,SIT and UAT and once the testing part is completed with all the bug fixes we are ready to deploy
it to PROD environment.In the intial stages we can trigger the pipeline manually to ave better contrl on the deployement.
Going forward we can add some test cases which will be executed everytime we commit code and if it has successfully executed automatic deployement can be done.
 

 
Executing the application
--------------------------------------------------
Open the sln file in the Visual studio and add the connection string for the sql database in appsettings json. Then run the project.It will land you on the register
page where new users can create their login.
Added a sign in link for the registered users.
