# **Installation of AWS CLI**

**Link:** [AWS CLI Installation Guide](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html)

### Steps to Install AWS CLI

```bash
# Download the AWS CLI
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"

# Install unzip
sudo apt install unzip

# Unzip the AWS CLI package
unzip awscliv2.zip

# Run the AWS CLI installer
sudo ./aws/install

# Verify the AWS CLI installation
sudo aws --version
