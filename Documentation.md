# MongoDB-Compass-Atlas-NodeJs
A comprehensive guide on how to install and set up MongoDB (Compass), and connect it to Atlas, and VS Code

## Mongodb Installation and Setup
[My LinkedIn](www.linkedin.com/in/maazinmm)

### Download the MongoDB Server installer from:
https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-8.0.9-signed.msi

When it is done downloading, go ahead and open the file to start the installation

![Screenshot 2025-05-07 140603](https://github.com/user-attachments/assets/ffff65b5-c1d7-4c19-92f6-44f44d5edcef)

From here click “Next” 

![image](https://github.com/user-attachments/assets/24423314-026f-426a-afed-e3a6db63415f)

Accept Agreement and click Next

![image](https://github.com/user-attachments/assets/89f71803-afbf-43ac-a341-2ca08e8120e2)

Choose Complete

![image](https://github.com/user-attachments/assets/7b8898cd-ffb4-4a03-b966-46792d6ec55a)

Leave everything as default and click Next

![image](https://github.com/user-attachments/assets/92b02cd6-97db-4995-9454-a11356a5db80)

Make sure “Install MongoDB Compass" is checked and click Next

![image](https://github.com/user-attachments/assets/e6eeb1d7-3b0e-41a8-9ff7-9834410e0a0e)

Click “Install”
From here, there should be a Windows prompt, accept it so installations can start.

![image](https://github.com/user-attachments/assets/c4849935-758b-4c56-b2c9-ea69f614313f)

Wait for installations to complete (takes a few minutes)

![image](https://github.com/user-attachments/assets/d4ab1e3d-9949-45e8-bb33-3fdb525a2633)

When the installation is done, you should see a window like this opened, even before the “Finish” window as below. MongoDB Compass is a visual tool that lets you see and interact with your MongoDB database.

![image](https://github.com/user-attachments/assets/0602c2d0-5e93-4ec2-b036-6aed1bc12716)

When you see this, click “Finish”.

![image](https://github.com/user-attachments/assets/e0df03e8-fb2b-4757-b131-2261d9258de4)

MongoDB is ready! If you click on “Add new connection” you will see your localhost connection string. 

![image](https://github.com/user-attachments/assets/32d1f66b-e418-4d12-a1d8-34007045ee77)

Your localhost connection string. (In **URI**)

## CONNECT COMPASS TO MONGODB ATLAS
Login to Mongodb Atlas:
https://www.mongodb.com/products/platform/cloud

![image](https://github.com/user-attachments/assets/431c9ad3-60a5-4f1d-93c3-ab622552e212)

Create an account if you don’t already have one

![image](https://github.com/user-attachments/assets/51e6863a-75e3-45b2-9dcd-19bf1d07a899)
<sub>Inside my project “maazinmm_1”</sub>
Create a cluster
Create a project and create a cluster under the project 

![image](https://github.com/user-attachments/assets/11f4fc1d-10a7-4050-b2c3-a9579d2c5b91)

In creating the cluster, choose the Free tier

![image](https://github.com/user-attachments/assets/a7c213b0-a5b2-447a-a1dd-626b0c4d72d7)

Set a name for your cluster
Select a cloud provider
Choose a region (us-east-1 is most preferred for free tier), and 
Click on “Create deployment” 

![image](https://github.com/user-attachments/assets/4556a72e-c5f7-44a4-8c45-62efcaa31933)

The system automatically adds your current IP address to enable local connectivity to your clusters.
You can change the database user credentials or leave it as is and copy them somewhere safe
Click “Create Database User”

![image](https://github.com/user-attachments/assets/7633ce24-d5ef-4e5d-8cce-09dc42d284d0)

Move to the next step to “Choose a connection method”

![image](https://github.com/user-attachments/assets/d1082551-2195-48a0-9812-e1b3ea56745c)

Choose how you want to interact with your MongoDB clusters
I prefer VS Code so I am going ahead with the VS Code environment setup
If you select any of those tools there is a guide to install them, like below.

![image](https://github.com/user-attachments/assets/2ba38202-5244-4cfa-9e84-b2d1f7254aa2)

Turn on “Show Password” and copy the connection string. We will use this later.

![image](https://github.com/user-attachments/assets/77bb3e97-0b63-429c-9be2-ca9019476995)
 
Find “MongoDB for VS Code” in VS Code Extensions and install it.

![image](https://github.com/user-attachments/assets/78735fab-d0d9-4ca2-b41b-aa69e3a9fde0)

Click “Connect” and paste your connection string copied from Atlas, as I showed earlier above.

![image](https://github.com/user-attachments/assets/af14a35c-d741-4ec4-afe3-7790d3d32dbc)

VS Code connected to Atlas Cluster successfully!

![image](https://github.com/user-attachments/assets/dbef2c3c-35cd-4e85-bb29-67cc0602a9fe)

Open MongoDB Compass, and paste your connection string here and click “Save & Connect”. Yes the same connection string. Make sure to add your password.

![image](https://github.com/user-attachments/assets/c6622729-db03-487d-8d3c-42af4a2b532f)

Atlas connected to Compass successfully!
These are our clusters created from Atlas!

## INSTALL NODEJS
Click this link install nodejs:
https://nodejs.org/dist/v22.15.0/node-v22.15.0-x64.msi

![image](https://github.com/user-attachments/assets/eaa4eff9-c5a0-41f2-a530-beb2bd80fd62)

![image](https://github.com/user-attachments/assets/98426245-070b-4da0-a73f-740746210e97)

Open the installer when the download is done and just follow the prompts. Try to leave everything as the default.

![image](https://github.com/user-attachments/assets/d0750d08-d6b1-434b-9fd2-3e619d850754)

Installation completes in just a moment. Click “Finish”

![image](https://github.com/user-attachments/assets/0b285c0c-02d0-4757-8eb5-3ffa77441389)

Open your terminal (PowerShell or VS Code Terminal, etc) and run node -v and npm -v to confirm nodejs and npm installation. If your terminal is already opened, close the entire terminal window and reopen it and run the command. 
 
 ![image](https://github.com/user-attachments/assets/350b848d-88af-4d07-89a5-c72a64d4f5b7)

While in your project directory, run npm install mongodb to install the mongoDB driver. Navigate to your project directory is you are not there. Create a directory and navigate into the directory and run it, if you are not already in one. You should not be in your root or a public directory like Documents or Desktop.
### You are all set now!

### Now let’s insert a document into MongoDB Atlas and see it show up in Compass and Atlas from our terminal!
1.	Create a file named insert.js

![image](https://github.com/user-attachments/assets/de7d6205-33e9-4394-a41d-c1e0e293bae8)

2.	Paste this code inside the insert.js file

<pre> const { MongoClient } = require('mongodb'); // Replace with your actual Atlas connection string including your password const uri = 'your_connection_string_here'; async function run() { const client = new MongoClient(uri); try { await client.connect(); const db = client.db('testDB'); // Will be created if it doesn't exist const users = db.collection('users'); // Same for this collection const result = await users.insertOne({ name: 'Jane Doe', age: 29, email: 'jane@example.com' }); console.log('Inserted with _id:', result.insertedId); } catch (err) { console.error('Error:', err); } finally { await client.close(); } } run(); </pre>

Looks like this:

![image](https://github.com/user-attachments/assets/b5b11564-4bc9-4131-a875-d4406117bef7)

Make sure to replace 'your_connection_string_here' with your real connection string from Atlas (don't forget to fill in your password).
3.	In the terminal, run node insert.js

![image](https://github.com/user-attachments/assets/13237df0-8373-4e74-9ec9-e2805b13febd)

4.	Open Compass and reload to see new changes
In Compass, go to View > Reload
You might need to click on connect, which appear on top of the cluster address on the left side pane. If it does not appear to reconnect and you can see your new testDB then you are good.

![image](https://github.com/user-attachments/assets/20e65239-b3ae-4386-a845-81b7393f8b54)

Refresh compass to see new changes

![image](https://github.com/user-attachments/assets/e0db08b6-e862-4ec2-a732-cf5a188a0087)

Click on testDB to see the new document and collection you just created with the nodejs code.
What the nodejs code does:
It connects to your Atlas instance.
Creates a function that uses the connection and creates;
A database named testDB
A collection named users 
Inserts data (name, age, email) into the collection.
## TRIAL
### CREATE A DATABASE, A COLLECTION, AND INSERT DATA INTO THE COLLECTION USING COMPASS.
