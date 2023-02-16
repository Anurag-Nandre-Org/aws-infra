AWS Infrastructure Setup using Terraform
Prerequisites Before you can create the infrastructure using Terraform, you need to have the following:

An AWS account with administrative privileges Terraform installed on your local machine AWS CLI installed on your local machine AWS IAM user with necessary permissions and access keys

Steps to Setup Infrastructure 1. Clone the repository to your local machine git clone https://github.com/your-username/aws-terraform-infrastructure.git

Navigate to the cloned directory cd aws-terraform-infrastructure

Initialize Terraform terraform init

Create a terraform.tfvars file with your AWS access and secret keys: access_key = "your_aws_access_key" secret_key = "your_aws_secret_key"

Plan the infrastructure to see what changes Terraform will make: terraform plan

Apply the infrastructure to create the resources: terraform apply

Verify that the infrastructure was created successfully: aws ec2 describe-instances

This command should return information about the EC2 instance that Terraform created.

Destroy the infrastructure when it is no longer needed: terraform destroy
