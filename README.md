                                            ⚙️  Be a Man 1 Assignment
                               Jenkins EC2 Startup Script Enhancement + Version Verification
          ✅ Java upgraded to 21  •  🐍 Python installed  •  🧱 Terraform installed  •  ☁️ AWS CLI verified
                                Environment used: Amazon Linux 2023 on AWS EC2
🎯 Objective
Modify the startup script and verify all required versions from the server command line.	

🛠️ Tools
Jenkins, Java 21, Terraform, Python 3, AWS CLI, Git, Jenkins plugins.	

📸 Evidence
Terminal output was captured from the EC2 instance; add the four screenshots for final submission.

1. Assignment Overview
This assignment required the EC2/Jenkins startup script to be updated so the instance could support Terraform automation, AWS access, Python, and an updated Java runtime. The completed implementation uses Amazon Corretto 21, installs Python 3, installs Terraform from the HashiCorp repository, and confirms the AWS CLI from the command line.

•	✅ Updated the Java runtime to Java 21.

•	✅ Installed Python 3 for scripting and command-line verification.

•	✅ Installed Terraform so infrastructure code can be initialized, planned, and applied from Jenkins.

•	✅ Verified the AWS CLI from the EC2 terminal to confirm cloud access tools were available.

•	✅ Kept Jenkins, Git, and the required Jenkins plugins in the startup workflow.


2. Updated EC2 Startup Script
The script is the updated startup script used to prepare the Jenkins EC2 instance. It updates the server, installs the required packages, adds the Terraform repository, and loads the requested Jenkins plugins at startup.


⚠️ Note: AWS CLI was verified on the EC2 instance from the terminal output. On this Amazon Linux 2023 environment, it was already available and reported a valid version.

3. Verification Commands Used on the EC2 Instance
After connecting to the instance, the following commands were used to verify the installed toolchain:
aws --version
java --version
terraform --version
python3 --version

4. Verified Version Results
   
Tool	Verified Version	Status	Evidence Source

☁️ AWS CLI	2.33.15	PASS ✅	EC2 terminal output

☕ Java	21.0.10	PASS ✅	EC2 terminal output

🧱 Terraform	1.14.8	PASS ✅	EC2 terminal output

🐍 Python	3.9.25	PASS ✅	EC2 terminal output

5. EC2 Evidence Summary
The following version evidence was captured from the live EC2 terminal session and confirms that the required software was available on the instance:
[ec2-user@ip-172-31-86-17 ~]$ aws --version
aws-cli/2.33.15 Python/3.9.25 Linux/6.1.163-186.299.amzn2023.x86_64 source/x86_64.amzn.2023

[ec2-user@ip-172-31-86-17 ~]$ java --version
openjdk 21.0.10 2026-01-20 LTS

[ec2-user@ip-172-31-86-17 ~]$ terraform --version
Terraform v1.14.8
on linux_amd64

[ec2-user@ip-172-31-86-17 ~]$ python3 --version
Python 3.9.25

6. Screenshot Evidence Checklist
📸 Final submission note: The terminal text above confirms the versions, but the assignment specifically asks for screenshots. Insert the actual EC2 terminal screenshots in the four boxes below before turning in the final assignment.

☁️ AWS CLI Screenshot
Run: aws --version

Paste screenshot here	
☕ Java Screenshot
Run: java --version

Paste screenshot here
🧱 Terraform Screenshot
Run: terraform --version

Paste screenshot here	
🐍 Python Screenshot
Run: python3 --version

Paste screenshot here

7. Conclusion
In summary, the EC2 startup process was successfully enhanced to support Jenkins and infrastructure automation requirements. Java 21, Terraform 1.14.8, Python 3.9.25, and AWS CLI 2.33.15 were all confirmed from the server command line, demonstrating that the instance was prepared for Terraform-based CI/CD work.

✅ Result: The environment is ready for Jenkins-driven infrastructure deployment, with only the four terminal screenshots needing to be pasted into the final submission package.

