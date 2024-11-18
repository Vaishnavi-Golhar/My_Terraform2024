# **Configure AWS CLI Using IAM User from AWS Management Console**

To configure AWS CLI with an IAM user, follow these step-by-step instructions:

## **Step 1: Create an IAM User in AWS Management Console**

1. **Log in** to the [AWS Management Console](https://aws.amazon.com/console/).
2. Navigate to the **IAM (Identity and Access Management)** service.
3. In the IAM Dashboard, click on **Users** from the left navigation pane, then click **Add users**.

### **Add User Details:**
- Enter a **User name** (e.g., `cli-user`).
- Select the **Access type** as **Programmatic access** (this provides an **Access Key ID** and **Secret Access Key**).

### **Set Permissions:**
- Choose **Attach policies directly**.
- Select a policy like **AdministratorAccess** for full access, or **AmazonS3FullAccess** based on your requirements.

### **Review and Create User:**
- Click **Next** until you reach the review page.
- Click **Create user**.

### **Download the Credentials:**
- After the user is created, you will see the **Access Key ID** and **Secret Access Key**.
- **Download the .csv file** or **copy** the credentials securely because the secret access key will not be shown again.

## **Step 2: Configure AWS CLI with IAM User Credentials**

Now that you have the Access Key ID and Secret Access Key, configure them using AWS CLI on your machine:

1. Open your terminal and run the following command:
   ```bash
   aws configure
