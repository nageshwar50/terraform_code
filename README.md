# Initialize Terraform
Initialize Terraform to download the necessary providers and modules:

``` terraform init ```
# Plan the Infrastructure:
Run the terraform plan command to preview the changes Terraform will make based on the configuration files. You can specify the dev.tfvars file to use the variable values from that file:

``` terraform plan -var-file="dev.tfvars" ```
# Apply the Configuration:
To apply the changes and create the infrastructure, run:
``` terraform apply -var-file="dev.tfvars" ```
# Verify the Infrastructure:
After the apply completes, you can verify the resources created by checking your AWS Management Console or by running:
``` terraform output ```

# Manage the Infrastructure:

Update: If you need to make changes, modify the .tf files and then run terraform plan and terraform apply again.
Destroy: To destroy the infrastructure created, run
``` terraform destroy -var-file="dev.tfvars" ```

This will tear down all the resources created by your Terraform configuration.
