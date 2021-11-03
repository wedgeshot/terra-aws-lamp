### Usage Instructions

1. Clone repository.
2. Install the AWS CLI for your respective operating system: https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html .
3. Install Terraform for your respective operating system: https://learn.hashicorp.com/tutorials/terraform/install-cli .
4. Move into the repository ``` cd <repository-name> ```.
5. Make sure your AWS account has IAM programmatic access: https://docs.aws.amazon.com/IAM/latest/UserGuide/id_users_change-permissions.html.
6. Edit main.tf and enter your AWS access key ID and secret access key in the top two variables.
7. While still editing main.tf, name your private keypair on line 212 and point to your local copy of the private key on line 426.
8. Run ``` terraform init ```
9. Run ``` terraform apply ```
10. The IP's for the web and database servers will be displayed after terraform apply is complete.
11. Point your browser to http://<public_ip> .
12. Run ``` terrafom destroy ``` so you don't get billed.
