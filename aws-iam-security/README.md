## Project: AWS IAM Security – Development vs Production Access

This project demonstrates using AWS Identity and Access Management (IAM)
to control access between development and production EC2 instances.

### What I Did
- Created separate EC2 instances for Development and Production
- Created an IAM policy to control EC2 permissions
- Used tags to separate Dev and Prod environments
- Tested permissions by logging in as an IAM user

### Steps

**Step 1: Created Development and Production EC2 instances**  
![Image](https://github.com/user-attachments/assets/f4f2a1a4-acd1-41a2-b65a-2d073f105068)

**Step 2: Created an IAM policy to control EC2 access**  
![Step 2](screenshots/step2.png)

**Step 3: Created an AWS account alias for easier sign-in**  
![Step 3](screenshots/step3.png)

**Step 4: Attached the IAM policy to a user group**  
![Step 4](screenshots/step4.png)

**Step 5: Created an IAM user for development access**  
![Step 5](screenshots/step5.png)

**Step 6: Logged in as the IAM user and verified restricted access**  
![Step 6](screenshots/step6.png)

**Step 7: Confirmed the user could NOT stop the Production EC2 instance**  
![Step 7](screenshots/step7.png)

**Step 8: Confirmed the user COULD stop the Development EC2 instance**  
![Step 8](screenshots/step8.png)

### Result
The IAM policy allows developers to manage development resources
while preventing changes to production resources.

*(EC2 instances may be stopped or removed to avoid AWS charges.)*
