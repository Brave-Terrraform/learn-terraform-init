# Initialize a Terraform Working Directory

01-Initialize-Terraform

The core Terraform workflow consists of three main steps after you have written your Terraform configuration:

Initialize prepares your workspace so Terraform can apply your configuration.
Plan allows you to preview the changes Terraform will make before you apply them.
Apply makes the changes defined by your plan to create, update, or destroy resources.
When you initialize a Terraform workspace, Terraform configures the backend, installs all providers and modules referred to in your configuration, and creates a version lock file if one doesn't already exist. In addition, you can use the terraform init command to change your workspace's backend and upgrade your workspace's providers and modules.

In this tutorial, you will initialize a Terraform workspace that uses both local and remote modules, explore the .terraform directory that Terraform uses to store your providers and modules, and update your provider and module versions. In the process, you will learn more about the terraform init command's integral role in the Terraform workflow.


This is a companion repository to the ["Initialize a Terraform Working Directory"](https://developer.hashicorp.com/terraform/tutorials/cli/init) tutorial.
