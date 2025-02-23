# Terraform-work

### Introduction
Terraform is a popular Infrastructure as Code (IaC) tool developed by HashiCorp, and it’s widely used for provisioning, managing, and automating infrastructure across various cloud providers
(e.g., AWS, Azure, Google Cloud) and on-premises environments.


## Installation  (Linux)

### 1. Update the System:
```
sudo apt update && sudo apt upgrade -y
```

### 2. Install Dependencies:
```
sudo apt install -y gnupg software-properties-common curl
```

### 3. Add the HashiCorp GPG Key:
```
curl -fsSL https://apt.releases.hashicorp.com/gpg | sudo gpg --dearmor -o /usr/share/keyrings/hashicorp-archive-keyring.gpg
```

### 4. Add the HashiCorp Repository:
```
echo "deb [signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] https://apt.releases.hashicorp.com $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/hashicorp.list
```

### 5. Install Terraform:
```
sudo apt update
sudo apt install terraform -y
```
-> Verify Terraform
```
terraform -version
```

![Screenshot from 2025-02-22 23-31-35](https://github.com/user-attachments/assets/8c69e374-5ac3-4f59-876a-5bb91735f32c)

------------------------------------------------------------------------------------------------------

## AWS setup

### 1. IAM (Identify and Access management)
** -> Go to user groups in IAM -> Create a User Group

![Screenshot from 2025-02-23 21-09-51](https://github.com/user-attachments/assets/ec1a65ce-0d9e-45e1-b300-bf09938111a4)

== Give it Above permissions ==

** -> Create User

![Screenshot from 2025-02-23 21-13-52](https://github.com/user-attachments/assets/4067742d-24b5-4a48-a4d2-96689c740592)

** -> Attach it with user Group of step 1

![Screenshot from 2025-02-23 21-16-19](https://github.com/user-attachments/assets/d754ef20-24cd-4138-a9ea-d3c9ec03419e)

** -> Create Access key

![Screenshot from 2025-02-23 21-18-51](https://github.com/user-attachments/assets/7aef27c1-8dd7-4685-8035-df9ca84868aa)

** -> Select AWS CLI

![Screenshot from 2025-02-23 21-20-46](https://github.com/user-attachments/assets/f816a6e3-7da8-47d7-858d-b5b517205d18)

