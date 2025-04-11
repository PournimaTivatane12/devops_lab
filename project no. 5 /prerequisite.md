# Prerequisites for Automated Infrastructure Provisioning with Terraform

Before you begin working on this project, ensure that you have the following prerequisites in place:

---

## 1. **Basic Knowledge Requirements**
- Familiarity with **Terraform** and its configuration language (HCL).
- Understanding of **infrastructure as code (IaC)** concepts.
- Knowledge of **cloud computing** platforms (e.g., AWS, Azure, or Google Cloud).
- Basic understanding of **networking**, **security groups**, and **virtual machines**.

---

## 2. **Software and Tools**
- **Terraform CLI**: Install the latest version of Terraform.
  - [Terraform Installation Guide](https://developer.hashicorp.com/terraform/downloads)
- **Cloud Provider CLI**: Install the CLI for your cloud provider (e.g., AWS CLI, Azure CLI, GCloud CLI).
  - AWS CLI: [Install Guide](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html)
  - Azure CLI: [Install Guide](https://learn.microsoft.com/en-us/cli/azure/install-azure-cli)
  - GCloud CLI: [Install Guide](https://cloud.google.com/sdk/docs/install)
- **Git**: Ensure Git is installed for version control.
  - [Git Installation Guide](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
- **Text Editor/IDE**: Use an editor such as VS Code, IntelliJ IDEA, or another IDE.
  - Install the **Terraform extension** in your IDE for syntax highlighting and formatting.

---

## 3. **Cloud Provider Account**
- Create an account with your preferred cloud provider (e.g., AWS, Azure, or Google Cloud).
- Set up billing and resource quotas to avoid deployment failures.
- Generate the necessary **API keys or credentials** for authentication:
  - AWS: Access Key ID and Secret Access Key.
  - Azure: Subscription ID, Tenant ID, Client ID, and Client Secret.
  - Google Cloud: Service Account Key (JSON).

---

## 4. **Environment Setup**
- Configure environment variables for cloud provider credentials.
  Example for AWS:
  ```bash
  export AWS_ACCESS_KEY_ID=<your-access-key-id>
  export AWS_SECRET_ACCESS_KEY=<your-secret-access-key>
  export AWS_DEFAULT_REGION=<your-region>

terraform init
