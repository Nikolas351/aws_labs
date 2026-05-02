# Lab 01: User Lifecycle Management (Provisioning and Deprovisioning) 
## Objective
This lab focuses on managing the full user lifecycle in Microsoft Entra ID, including user and group creation, transferring users between departments, and deprovisioning accounts. 

The goal is to simulate real-world IAM operations such as joiner, mover, and leaver workflows while applying access control and least privilege principles throughout. This lab was conducted in a personal Microsoft Entra ID tenant using simulated users and groups to represent a company with multiple departments.

## Step 1: Create Roles and Users CSV
Created two CSV files to represent simulated company data. Roles CSV mapped each department, Users CSV includes user's name, department, job title, and status.

![Users CSV](Screenshots/created/users-csv.png)

![Roles CSV](Screenshots/created/roles-csv.png)

## Step 2: Create User Accounts
Click New User → Create New User → 
Fill in: 
- User principal name
- User display name
- User properties (User type, Job Title, Department)

Set or auto generate password

<img src="Screenshots/created/user-create.png" width="450" height="350">

List of all created users:

<img src="Screenshots/created/users-list.png" width="800">

## Step 3: Create Security Groups 
Click New Group 

Enter group name and description

Select:
- Group Type: Security
- Group Owners (My admin account)

<img src="Screenshots/created/group-create.png" width="450" height="350">

List of all created groups:

<img src="Screenshots/created/group-list.png" width="800">

## Step 4: Add user to groups
Click on All Groups → Choose specific group

Go to Members tab

Click Add Members

Select the appropriate user

<img src="Screenshots/created/eng-team.png" width="800">

# Part 2: User Changing Departments

## Step 1: Change Users Properties

Click on Users → Choose Appropriate User

Click Edit Properties → All

Change corresponding properties to appropriate department (Job Title, Department, etc)

<img src="Screenshots/mover/dan-before-swap.png" width="500">  <img src="Screenshots/mover/dan-after-swap.png" width="500">

## Step 2: Mover — Remove User From Original Department and Assign to New Department

Click Groups → All Groups → Choose Users Old Department Group

Click Members → Checkbox Users → Remove
