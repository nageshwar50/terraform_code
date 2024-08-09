# Initialize Terraform
Initialize Terraform to download the necessary providers and modules:

``` terraform init ```

![image](https://github.com/user-attachments/assets/1d655151-b038-4736-bdbf-a34054346947)

# Plan the Infrastructure:
Run the terraform plan command to preview the changes Terraform will make based on the configuration files. You can specify the dev.tfvars file to use the variable values from that file:

``` terraform plan -var-file="dev.tfvars" ```

![image](https://github.com/user-attachments/assets/a9024158-c468-4697-9218-cd3c31550d72)

# Apply the Configuration:
To apply the changes and create the infrastructure, run:

``` terraform apply -var-file="dev.tfvars" ```
![image](https://github.com/user-attachments/assets/fdf15ad9-4857-4601-ad83-115448575432)
![image](https://github.com/user-attachments/assets/e31bb873-c31d-46a7-8aae-0c879d8fdfc1)
![image](https://github.com/user-attachments/assets/078dbb96-be96-4608-b6bd-4f1dd066fd28)
![image](https://github.com/user-attachments/assets/9a63eadc-7856-4227-9b4c-2fb4ebdf478e)
![image](https://github.com/user-attachments/assets/2db5fe79-08e0-405d-88cd-53b7ebe2fd14)


# Verify the Infrastructure:
After the apply completes, you can verify the resources created by checking your AWS Management Console or by running:

``` terraform output ```
![image](https://github.com/user-attachments/assets/16736f60-b4df-4dd3-abbc-7baed876a972)

# Manage the Infrastructure:

Update: If you need to make changes, modify the .tf files and then run terraform plan and terraform apply again.
Destroy: To destroy the infrastructure created, run

``` terraform destroy -var-file="dev.tfvars" ```
![image](https://github.com/user-attachments/assets/84bef216-3a0a-4df4-944c-441908b94fc3)
![image](https://github.com/user-attachments/assets/72ba8db7-cfaf-4435-865f-34775703d959)

![image](https://github.com/user-attachments/assets/fa96db50-3614-46af-87f3-8ae40cff2288)

This will tear down all the resources created by your Terraform configuration.
