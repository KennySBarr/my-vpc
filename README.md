<p align="center">
       
![AWS_logo_new](https://github.com/user-attachments/assets/a7a389ae-0c58-4096-afdf-d0586aaa44e3)

   

</p>

<h1>AWS Cloud </h1>
AWS (Amazon Web Services) is a comprehensive and widely adopted cloud platform that offers a variety of on-demand computing services, storage, networking, and analytics, enabling businesses to scale and innovate with flexibility and efficiency.

<h2>Requirements</h2>

- Computer with Internet Connection
- Credit Card (Required for free AWS credits)

<h2>Configuration Steps</h2>


<h3>Step 1: Create a VPC</h3>

- Search in the search bar "VPC" 
- Select VPC
  
![Screenshot 2024-12-07 054206](https://github.com/user-attachments/assets/e1d7a346-2feb-464e-b115-0f52d92aef40)


- Follow the prompt to the "Create VPC" 
     - You will notice there will be a defualt VPC already created!!
    
![Screenshot 2024-12-07 054223](https://github.com/user-attachments/assets/40f72bca-c397-4ea1-81b9-f4f5b3f94de1)



<h3>Step 2: Provision the VPC</h3>

 - AWS are so advanced, AMazon has a feature that creates the private and public subnets for you!
 - For the IPv4 CIDR Block you may want to change the number, you dont want multiple people on the same starting IP
 - You can also change the amount of availability zones, the zones are there incase you need to recover from a disaster
 - Every Subnet has their own route table, the public subnets are routed to the public internet gatweway
 - The private subnets are routed to the AWS S3 where all encrpyted data will be
 

![Screenshot 2024-12-07 054329](https://github.com/user-attachments/assets/fcc5bf46-d10d-42e3-94bf-c0e79055b1ed)






<h3>Step 2: Create an IAM User with Amazon S3 Access</h3>

- Go to the search bar at the top and search "IAM"
- Select Users tab to the left 
- You will need to name the user JohnDoe 
- Then click create passwordd
-  Create a Custom password and follow the rules and unclick "User has to reset password on next login" 

 
![Screenshot 2024-12-04 143727](https://github.com/user-attachments/assets/fe05ddf6-bafa-43a4-9ef8-0cad535fc875)





<h3>Step 3: Set Permissions to the IAM USer "JohnDoe" </h3>

- Click custom policy
- then click the Permissions Policy
- Select or Search Amazon S3 Access 
- You will need to select amazon S3 Access
- Then click Next 
 

![Screenshot 2024-12-04 143953](https://github.com/user-attachments/assets/d636cb79-6e74-4a8b-b859-0fb763253c10)

<h3>Step 4: Confirm IAM User</h3>
     
- Copy the sign in link provided for IAM User into another browser 

![Screenshot 2024-12-04 144025](https://github.com/user-attachments/assets/962700ee-03ea-4240-9961-83db19d8fb90)

- Log into the IAM user with the Username and Password created
    - The number you see attatched in the login screen is the number assocaited with your root account 

![Screenshot 2024-12-04 145254](https://github.com/user-attachments/assets/8589c3a8-f924-461d-a997-695276fa8a55)

- As seen in the third picture below the "JohnDoe" account has permission restrictions flagged on his/her dashboard upon launch

![Screenshot 2024-12-04 145335](https://github.com/user-attachments/assets/5bfff862-501b-48ce-b18a-97467e75497a)


