# gcp-cloud-infra
terraform-gcp-infra/
├── modules/
│   ├── networking/
│   │   ├── main.tf  # Define VPC, Subnets, Firewall Rules
│   │   ├── variables.tf
│   │   ├── outputs.tf
│   ├── iam/
│   │   ├── main.tf  # Define IAM Roles & Policies
│   │   ├── variables.tf
│   │   ├── outputs.tf
│   ├── compute/
│   │   ├── main.tf  # Define GKE, VM Instances, Load Balancers
│   │   ├── variables.tf
│   │   ├── outputs.tf
│   ├── storage/
│   │   ├── main.tf  # Define GCS Buckets, Object Lifecycle
│   │   ├── variables.tf
│   │   ├── outputs.tf
│   ├── monitoring/
│   │   ├── main.tf  # Define Logging, Monitoring Alerts
│   │   ├── variables.tf
│   │   ├── outputs.tf
├── envs/
│   ├── dev/
│   │   ├── main.tf  # Call modules with dev-specific variables
│   │   ├── variables.tf
│   │   ├── backend.tf  # Configure remote state backend
│   ├── prod/
│   │   ├── main.tf  # Call modules with prod-specific variables
│   │   ├── variables.tf
│   │   ├── backend.tf
├── terraform.tfvars  # Common variables
├── backend.tf  # GCS Backend Configuration
├── providers.tf  # Provider Config (Google Cloud)
├── versions.tf  # Define Terraform version
└── README.md  # Documentation
