

# Terraform AWS ECS Fargate Deployment

This Terraform script deploys a containerized application on AWS ECS Fargate with an Application Load Balancer, VPC, security groups, and autoscaling policies.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Usage](#usage)
- [Configuration](#configuration)
- [Terraform Commands](#terraform-commands)
- [Outputs](#outputs)
- [Contributing](#contributing)
- [License](#license)

## Prerequisites

Before you begin, ensure you have the following in place:

- [Terraform](https://www.terraform.io/) installed.
- AWS credentials configured with the necessary permissions.

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/utrains/deploy-ecs-farget-with-terraform.git
   cd terraform-aws-ecs-fargate
   ```

2. Update the `terraform.tfvars` file with your configuration.

3. Run Terraform commands to deploy the infrastructure:

   ```bash
   terraform init
   terraform apply
   ```

## Configuration

The main configuration parameters are defined in the `terraform.tfvars` file:

- `region`: AWS region for deployment.
- `image`: Docker image for the application.
- `container_name`: Name of the ECS container.
- `container_port`: Port to which the Docker image is exposed.

Update these variables based on your application requirements.

## Terraform Commands

- `terraform init`: Initializes the working directory.
- `terraform apply`: Applies the Terraform configuration and deploys the infrastructure.
- `terraform destroy`: Destroys the deployed infrastructure.

## Outputs

- `lb_url`: URL of the deployed Application Load Balancer.

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

## License

