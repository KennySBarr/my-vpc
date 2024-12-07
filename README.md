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


<h3>Step 3: Create VC </h3>

- Click Create 

![Screenshot 2024-12-07 055108](https://github.com/user-attachments/assets/7525b740-786e-4014-8e72-07758daf64e3)

<h3>Step 3: Check Private and Public Subnets for proper routing </h3>

- The public subnet has a Target to the internet gateway (Public)

![Screenshot 2024-12-07 055842](https://github.com/user-attachments/assets/8b064ab0-2d1d-4b59-9ef6-3ddab79e4ab5)

- The private subnet has a Target to AWS S3 only 
  
![Screenshot 2024-12-07 055929](https://github.com/user-attachments/assets/e0c59a06-fcb5-401a-90fd-ade7df40d1ce)


![Screenshot 2024-12-07 055946](https://github.com/user-attachments/assets/a0e570d6-a047-40e3-abb6-1b6c91c087d3)



