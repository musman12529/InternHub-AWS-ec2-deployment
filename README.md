# Deployment on AWS EC2

### 1. Set Up  AWS EC2 Instance
   - `Launch Instance`.
**Choose an Operating System**:
   - Select a lightweight Ubuntu OS 
**Configure Instance Settings**:
   - Choose the instance type `t2.micro` (Free Tier eligible).

**Launch the Instance**:
   - Keep the remaining settings as default and click `Launch Instance`.

**Allocate and Associate an Elastic IP**

**Connect to  Instance**:

   - Opend terminal, navigate to  Downloads folder (where `.pem` file is located), and paste the SSH command.


**Update and Install Necessary Software**

**Install NVM and Update Node.js**:
   - Install NVM:
     ```bash
     curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
     ```
   - Load NVM:
     ```bash
     source ~/.bashrc
     ```
   - Install the desired Node.js version:
     ```bash
     nvm install 20.11.0
     ```
   - Use the installed Node.js version:
     ```bash
     nvm use 20.11.0
     ```

### 3. Deploy  MERN App

1. **Clone  GitHub Repository**:
   - Copy  repository URL from GitHub.
   - In the terminal connected to  EC2 instance, run:
     ```bash
     git clone <repo-url>
     ```
   - Navigate into your project directory:
     ```bash

 **Install Dependencies and Start the Backend**

2. **Build  Frontend**

### 4. Configure Security Groups and Final Steps

1. **Set Up Security Groups**:
   - Go back to the AWS EC2 dashboard.
   - Allow inbound traffic for HTTP (port 80), HTTPS (port 443), and any other necessary ports (like 3000 or 4000 for  app).





![backend-pic](https://github.com/user-attachments/assets/e3cf254c-a10b-41ab-88e1-08e59ecdc5ee)
