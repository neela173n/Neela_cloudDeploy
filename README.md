 Deploying ToDo list application on cloud 
-
In this project , I have deployed a to-do app, which allows us to add our day to day tasks,edit and delete tasks once its completed. This application is deployed using Google cloud Platform for enabling public to access the application.

set up and runnning the application:
-
Install python 3.13.1 and run the execution file and complete the process of download.

Install the open source python framework in the same directory, and FLASK which helps us to design a flexible application.

VS code is used as the source code editor to save and run the  codes required for effective functioning of the website. The file structure is as follows:

-->main.py (backend code for flask)

-->requirements.txt (for flask which is a python dependency)

-->procfile (for deploying on cloud platforms)

-->/Templates (html)
  -->Index.html
  
  -->edit.html

-->/statics (css and js files)

  -->styles.css(for adding a background colour for the page )

 Running the project:

 command to run project locally in the terminal : "python main.py" 

 Commands to push local progect to the github repository:
 -
 -Install and login to the github account

 -Navigate to the folder where project files are saved , right-click and open git bash in that location.Execute the below commands in bash terminal

 -> $ git config --global user.name "neela173n"
       
 -> $ git config --global user.email "neela173n@gmail.com"
       
 -> $ git init
       
 -> $ git commit -m "initial commit"
       
  -> $ git add .
       
  -> $ git remote add origin https://github.com/neela173n/Neela_cloudDeploy.git  [Insert respective github public repository link]
       
  -> $ git push origin main

Instructions to deploy Github repo on a public server, here, google account using "CLOUD RUN" 
-
-Login to your google cloud account. 

-Go to Google Cloud Console --> "Cloud Run" --> "Connect Repo" --> Continously deploy from a Repository --> "Setup with cloud build."

        --> In "setup with cloud build" choose your github profile and click on authenticate further choose the repository you want to deploy and click on --> NEXT
        
        --> In Build Configurations: -->choose main branch (if there is only one branch in your github repo and main branch is a default branch) and choose -->Go, Nodejs, Python file.
        
             -->Entry point would be your "python main.py"  and click on "SAVE"
             
        --> Service name would be the same name as your repository and select region--> Mumbai(Asia)
        
        --> Enable "Allow unauthenticated invocations" as there's no confidential information as of now in this project
        
        --> Change the minimum instances to 1
        
        --> let the remaining options be the default chose itself. 
        
        --> click on "CREATE"
        
        --> Now the project will be succesfully deployed and a public url will be generated

        -->  THE FINAL PUBLIC URL GENERATED IN THIS PROJECT : "https://neela-clouddeploy-590809044493.asia-south1.run.app/"


PROJECT OUTPUT 
-
-https://neela-clouddeploy-590809044493.asia-south1.run.app/

        
