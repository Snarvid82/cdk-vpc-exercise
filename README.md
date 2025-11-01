# cdk-vpc-exercise

## Project Overview

This repository contains the code for a CDK (Cloud Development Kit) project focused on creating and managing VPC (Virtual Private Cloud) resources in AWS. The primary goal is to provide a foundational infrastructure component that can be easily deployed and customized for various application needs.

## Key Features & Benefits

*   **Infrastructure as Code:** Define and manage VPC resources using the CDK, enabling version control, repeatability, and automated deployments.
*   **Customizable VPC Configuration:** Easily configure the number of Availability Zones, CIDR blocks, subnets, and other VPC parameters to meet specific requirements.
*   **Simplified Deployment:** Leverage the CDK's abstraction to simplify the complexity of AWS infrastructure provisioning.
*   **Scalable Architecture:** Design a scalable VPC architecture that can accommodate future growth and increased traffic.

## Prerequisites & Dependencies

Before you begin, ensure you have the following installed and configured:

*   **AWS Account:** An active AWS account with appropriate permissions to create and manage VPC resources.
*   **AWS CLI:** The AWS Command Line Interface installed and configured with your AWS credentials.
    *   Installation instructions can be found [here](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html).
*   **Node.js and npm:** Node.js and npm (Node Package Manager) are required for running the CDK.
    *   Download and install Node.js from [https://nodejs.org/](https://nodejs.org/).  npm is included with Node.js.
*   **AWS CDK Toolkit:** The AWS CDK Toolkit must be installed globally.
    ```bash
    npm install -g aws-cdk
    ```
*   **TypeScript:**  Install TypeScript globally using npm.
    ```bash
    npm install -g typescript
    ```

## Installation & Setup Instructions

1.  **Clone the Repository:**

    ```bash
    git clone <repository_url>
    cd cdk-vpc-exercise
    ```

2.  **Install Dependencies:**

    ```bash
    npm install
    ```

3.  **Bootstrap CDK (if necessary):**

    If this is your first time using CDK in this AWS account and region, you may need to bootstrap the CDK:

    ```bash
    cdk bootstrap aws://<your-aws-account-id>/<your-aws-region>
    ```

    Replace `<your-aws-account-id>` with your AWS account ID and `<your-aws-region>` with the AWS region you are deploying to (e.g., `us-east-1`).

## Usage Examples

### Deploying the VPC

To deploy the VPC, use the following command:

```bash
cdk deploy
```

This command will synthesize the CDK code into CloudFormation templates and deploy the VPC to your AWS account.

### Destroying the VPC

To remove the deployed VPC, use the following command:

```bash
cdk destroy
```

## Configuration Options

The CDK project is configured using TypeScript code. You can modify the following parameters:

*   **VPC CIDR Block:**  The CIDR block for the VPC (e.g., `10.0.0.0/16`).
*   **Number of Availability Zones:** The number of Availability Zones to use for the VPC.
*   **Subnet Configuration:**  Customize the subnet configuration including CIDR blocks and subnet types (public, private, isolated).

These parameters can be modified directly within the CDK stack definition file.

## Contributing Guidelines

We welcome contributions to this project! If you'd like to contribute, please follow these guidelines:

1.  Fork the repository.
2.  Create a new branch for your feature or bug fix.
3.  Make your changes and commit them with clear, concise commit messages.
4.  Submit a pull request to the `main` branch.

Please ensure that your code adheres to the project's coding standards and includes appropriate tests.

## License Information

This project does not specify a license. All rights are reserved.

## Acknowledgments

This project utilizes the AWS Cloud Development Kit (CDK).


