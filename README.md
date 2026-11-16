# CLOUD-DATA-STORAGE-SERVER
### CLOUD DATA STORAGE SERVER
### NAME: POOJA D
### REG NO: 212225040301
### Aim
To create and configure an Amazon Relational Database Service (Amazon RDS) instance as a cloud data storage server, configure the required security settings, connect it to a web application, and perform database operations using the application.

### Algorithm / Steps
Create a Security Group for the RDS database.
Add an inbound rule to allow MySQL (Port 3306) access from the Web Security Group.
Create a DB Subnet Group using two Availability Zones.
Launch an Amazon RDS MySQL database instance.
Configure the database with the required identifier, username, password, storage, and instance class.
Associate the database with the created Security Group and Subnet Group.
Wait until the database status becomes Available.
Copy the RDS endpoint.
Open the web application using the provided Web Server IP address.
Enter the RDS endpoint, database name, username, and password.
Connect the application to the database.
Verify the connection by adding, editing, and deleting records in the Address Book application.
### Program
### Security Group Configuration
Security Group Name: DB Security Group
Inbound Rule: MySQL/Aurora (3306)
Source: Web Security Group
### DB Subnet Group
Name: DB-Subnet-Group
VPC: Lab VPC
### Amazon RDS Configuration
Engine: MySQL
Template: Dev/Test
Availability: Multi-AZ
DB Instance Identifier: lab-db
Username: main
Password: lab-password
Instance Class: db.t3.micro
Storage: 20 GB (General Purpose SSD)
### Connect the Application
```
Endpoint : <RDS Endpoint>
Database : lab
Username : main
Password : lab-password
```
After submitting the above details, perform Add, Edit, and Delete operations on the Address Book application.


### Output
<img width="1920" height="1080" alt="Screenshot 2026-11-16 134018" src="https://github.com/user-attachments/assets/9c17736d-6279-4bb5-a494-baf9466faf3d" />
<img width="1920" height="1080" alt="Screenshot 2026-11-16 134102" src="https://github.com/user-attachments/assets/594b1f98-b0fd-454d-a014-1fd313a4fb9d" />
<img width="1920" height="1080" alt="Screenshot 2026-11-16 134201" src="https://github.com/user-attachments/assets/b9b8dd43-63f2-4225-8739-35769aa48cf0" />
<img width="1920" height="1080" alt="Screenshot 2026-11-16 134243" src="https://github.com/user-attachments/assets/1044f3a6-9f85-485c-8c31-bbad8e17f3e4" />
<img width="1920" height="1080" alt="Screenshot 2026-11-16 134531" src="https://github.com/user-attachments/assets/3f99dda8-2355-4ab1-9b3d-72479568f850" />
<img width="1920" height="1080" alt="Screenshot 2026-11-16 135115" src="https://github.com/user-attachments/assets/878e4c80-e7be-49a7-ac28-aab9f79dd884" />
<img width="1920" height="1080" alt="Screenshot 2026-11-16 135259" src="https://github.com/user-attachments/assets/30a22fd4-062d-40a5-92f8-dba030389b5a" />
<img width="1920" height="1080" alt="Screenshot 2026-11-16 135404" src="https://github.com/user-attachments/assets/9a873318-57ed-47b2-aad8-ca0724576ee2" />
<img width="1920" height="1080" alt="Screenshot 2026-11-16 135539" src="https://github.com/user-attachments/assets/37eef9bf-c0df-4bd4-a76e-d1e201b28638" />
<img width="1920" height="1080" alt="Screenshot 2026-11-16 135726" src="https://github.com/user-attachments/assets/78d95f13-050a-49da-ab94-95eb1154a4e4" />

### Result
Thus, an Amazon RDS database instance was successfully created and configured as a cloud data storage server. The database was securely connected to a web application, and data operations such as inserting, updating, and deleting records were successfully performed through the application.





