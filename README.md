**## Hosting a Website on AWS EC2 with a CICD Setup Using Github Actions**

- This project involves the following steps:

- *Step 1: Create an EC2 instance, allow the neccessary ports in your sg, and download your keypair*

- *Stept 2: Create secrets in GitHub for the Repository*

   The secrets settings are as follows:
   . EC2_SSH_KEY: This carries your .pem file to be used to log into your EC2 instance
   . HOST_DNS: It's the public DNS ID of the EC2 instance,e.g. ec2-xx-xxx-xxx-xxx.us.west-1.compute.anazonaws.com
   . USER_NAME: This will be the username of the EC2 to host your application, e.g. AmazonLinux2, Ubuntu.
   . TARGET_DIR: A target directory is where you want your code to be deployed.

- *Step 3: Create your workflow by following gitHub practices*
   #To create a workflow in your repository that will be recognized by GitHub, the directory must be .github/workflows/<name-of-your-workflow.yml-file> 

- *Step 4; Testing*
