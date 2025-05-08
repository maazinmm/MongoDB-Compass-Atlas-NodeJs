# MongoDB-Compass-Atlas-NodeJs
A comprehensive guide on how to install and set up MongoDB (Compass), and connect it to Atlas, and VS Code


## Mongodb Installation and Setup
[My LinkedIn](www.linkedin.com/in/maazinmm)

1.	Download the mongodb server installer from https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-8.0.9-signed.msi

When it is done downloading, go ahead and open the file to start the installation


 
From here click “Next” 
 
Accept agreement and click Next
 
Choose complete
 
Leave everything as default and click Next
 
Make sure “Install MongoDB Compass is checked and click Next
 
Click “Install”
From here, there should be a windows prompt, accept it so installations can start.
 
Wait for installations to complete (takes a few minutes)
 
When the installation is done, you should see a window like this opened, even before the “Finish” window as below. MongoDB Compass is a visual tool that lets you see and interact with your MongoDB database.
 
When you see this, click “Finish”.
 
MongoDB is ready! If you click on “Add new connection” you will see your localhost connection string. 
 
Your localhost connection string.














CONNECT COMPASS TO MONGODB ATLAS
Login to Mongodb Atlas: 
https://www.mongodb.com/products/platform/cloud
Create an account if you don’t already have one
 
Create a cluster
Create a project and create a cluster under the project
 
Inside my project “maazinmm_1”. 
 
In creating the cluster, choose the Free tier
 
Set a name for your cluster
Select a cloud provider
Choose a region (us-east-1 is most preferred for free tier), and 
Click on “Create deployment” 
 
The system automatically adds your current ip address to enable local connectivity to your clusters.
You can change the database user credentials or leave it as is and copy them somewhere safe
Click “Create Database User”
 
Move to the next step to “Choose a connection method”
 
Choose how you want to interact with your MongoDB clusters
I prefer VS Code so I am going ahead with the VS Code environment setup
If you select any of those tools there is a guide to install them, like below
 
Turn on “Show Password” and copy the connection string


 
Find “MongoDB for VS Code” in VS Code Extensions and install it
 
Click “Connect” and paste your connection string copied from Atlas, as I showed earlier above.
 
VS Code connected to Atlas Cluster successfully!
 
Open MongoDB Compass, and paste your connection string here and click “Save & Connect”. Yes the same connection string. Make sure to add your password.
 
Atlas connected to Compass successfully!
These are our clusters created from Atlas!

Install nodejs
Click this link install nodejs:
https://nodejs.org/dist/v22.15.0/node-v22.15.0-x64.msi
 
 
Open the installer when the download is done and just follow the prompts. Try to leave everything as the default.
 
Installation completes in just a moment. Click “Finish”
 
Open your terminal (PowerShell or VS Code Terminal, etc) and run node -v and npm -v to confirm nodejs and npm installation. If your terminal is already opened, close the entire terminal window and reopen it and run the command. 
 
While in your project directory, run npm install mongodb to install the mongoDB driver. Navigate to your project directory is you are not there. Create a directory and navigate into the directory and run it, if you are not already in one. You should not be in your root or a public directory like Documents or Desktop.
You are all set now!
Now let’s insert a document into MongoDB Atlas and see it show up in Compass and Atlas from our terminal!
1.	Create a file named insert.js
  
2.	Paste this code inside the insert.js file
Make sure to replace 'your_connection_string_here' with your real connection string from Atlas (don't forget to fill in your password).
3.	In the terminal, run node insert.js
  
4.	Open Compass and reload to see new changes
In Compass, go to View > Reload
You might need to click on connect, which appear on top of the cluster address on the left side pane. If it does not appear to reconnect and you can see your new testDB then you are good.
 
Refresh compass to see new changes
 
Click on testDB to see the new document and collection you just created with the nodejs code.
What the nodejs code does:
It connects to your Atlas instance.
Creates a function that uses the connection and creates;
A database named testDB
A collection named users 
Inserts data (name, age, email) into the collection.
TRIAL
CREATE A DATABASE, A COLLECTION, AND INSERT DATA INTO THE COLLECTION USING COMPASS.
