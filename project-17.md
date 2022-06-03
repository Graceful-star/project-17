# Doocumentation of Project 17

1. I continued from where I stopped at project 16 by creating private subnets
   
   ![Project17](images/image1.PNG)

2. I added tags to my private and public subnets

   ![Project17](images/image2.PNG)

3. I added the variable for my private subnet and tags in my 'variable.tf' file

   ![Project17](images/image3.PNG)
   ![Project17](images/image4.PNG)
   ![Project17](images/image5.PNG)

4. I ran the `terraform plan` command and it was successful
    
    ![Project17](images/image6.PNG)
    ![Project17](images/image7.PNG)
    ![Project17](images/image8.PNG)
    ![Project17](images/image9.PNG)
    ![Project17](images/image10.PNG)
    ![Project17](images/image11.PNG)

5. I created two new files namely 'internet-gateway.tf' and 'nat-gateway.tf' and I inserted the required commands for me to create internet gateway, nat gateway and elastic ip address

    ![Project17](images/image12.PNG)
    ![Project17](images/image13.PNG)
    ![Project17](images/image14.PNG)


6. I ran the `terraform plan` command as usual and it worked

    ![Project17](images/image15.PNG)
    ![Project17](images/image16.PNG)
    ![Project17](images/image17.PNG)
    ![Project17](images/image18.PNG)
    ![Project17](images/image19.PNG)
    ![Project17](images/image20.PNG)
    ![Project17](images/image21.PNG)

7. I created another file; 'routes.tf' and inserted the required commands for creating route table, routes and route-table association. Then I ran the `terraform plan` command and it worked.

    ![Project17](images/image22.PNG)
    ![Project17](images/image23.PNG)
    ![Project17](images/image24.PNG)
    ![Project17](images/image25.PNG)
    ![Project17](images/image26.PNG)
    ![Project17](images/image27.PNG)

8. I ran the `terraform apply` command and it worked
   
   ![Project17](images/image31.PNG)
   ![Project17](images/image32.PNG)

9. I confirmed everything that was created on my aws console
   
   ![Project17](images/image33.PNG)
   ![Project17](images/image34.PNG)
   ![Project17](images/image35.PNG)
   ![Project17](images/image36.PNG)
   ![Project17](images/image37.PNG)
   ![Project17](images/image38.PNG)
   ![Project17](images/image39.PNG)
   ![Project17](images/image40.PNG)

10. I created three files;

a. "cert.tf"- for creating and validating a certificate and for also creating records in Route53 on aws console

b. "security.tf"- for creating security groups and editing the rules

c. "alb.tf"- for creating load balancers, target groups

   ![Project17](images/image43.PNG)
   ![Project17](images/image44.PNG)
   ![Project17](images/image45.PNG)

11. I ran the `terrraform plan` and `terraform apply` commands and it worked
    
    ![Project17](images/image46.PNG)

12. I confirmed the things I just created on my aws console

    ![Project17](images/image47.PNG)
    ![Project17](images/image48.PNG)
    ![Project17](images/image49.PNG)
    ![Project17](images/image50.PNG)
    ![Project17](images/image51.PNG)

13. I created another file; "routes.tf" for creating Iam role policy. Then I  ran `terraform plan` command as usual
    
    ![Project17](images/image52.PNG)
    ![Project17](images/image53.PNG)

14. I created new files;

a. "asg-webserver.tf"- for creating launch templates
  
b. "asg-bastion.tf"- for creating auto-scaling groups

c. "bastion.sh"- a shell script for bastion

d. "nginx.sh"- a shell script for nginx

e. "tooling.sh"- a shell script for tooling

f. "wordpress.sh"- a shell script for wordpress

g. "outputs.tf"- for the output

then I ran `terraform plan` and `terraform apply` and it worked

     ![Project17](images/image54.PNG)
     ![Project17](images/image55.PNG)
     ![Project17](images/image56.PNG)
     ![Project17](images/image57.PNG)
     ![Project17](images/image58.PNG)
     ![Project17](images/image59.PNG)
     ![Project17](images/image60.PNG)
     ![Project17](images/image61.PNG)

15. I checked my aws console to confirm if what I created is showing

     ![Project17](images/image62.PNG)

16. I created new files;

a. "efs.tf"- for creating a file system and a key

b. "rds.tf"- for creating a subnet group and a database

Then I applied the code and it worked
    

    ![Project17](images/image63.PNG)
    ![Project17](images/image64.PNG)
    ![Project17](images/image65.PNG)

17. I confirmed what I've created on my aws console

    
    ![Project17](images/image66.PNG)
    ![Project17](images/image67.PNG)
    ![Project17](images/image68.PNG)
    ![Project17](images/image69.PNG)
    ![Project17](images/image70.PNG)
    ![Project17](images/image71.PNG)