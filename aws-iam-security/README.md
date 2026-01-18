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
![Image](https://github.com/user-attachments/assets/d93f23d8-32cd-4fa7-833b-59c00e4568ac)

**Step 3: Created an AWS account alias for easier sign-in**  
![Image](https://github.com/user-attachments/assets/63417731-737b-4f7f-a3ce-9194ccf3b693)

**Step 4: Attached the IAM policy to a user group**  
![Image](https://github.com/user-attachments/assets/38f99098-e82b-4585-a9f2-d3bd16081dad)

**Step 5: Created an IAM user for development access**  
![Image](https://github.com/user-attachments/assets/70e728a9-d6fb-4cf2-af26-c65732c410b7)

**Step 6: Logged in as the IAM user and verified restricted access**  
![Image](https://github.com/user-attachments/assets/a2bad1e7-4408-4787-945e-e62219f58424)

**Step 7: Confirmed the user could NOT stop the Production EC2 instance**  
![Image](https://github.com/user-attachments/assets/a729c320-32b3-49bc-9a5c-493c2d8f6968)

**Step 8: Confirmed the user COULD stop the Development EC2 instance**  
![Image](https://github.com/user-attachments/assets/b7531145-e7a1-42a1-8a9f-6af831f7d530)

### Result
The IAM policy lets developers work with development resources but blocks them from changing production resources.
