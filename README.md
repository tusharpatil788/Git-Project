
banking-microservices/
├── account-service/        # Spring Boot, built by GitHub Actions
│   ├── src/
│   ├── Dockerfile
│   └── .github/workflows/ci.yml
├── payment-service/        # Spring Boot, built by Jenkins
│   ├── src/
│   ├── Dockerfile
│   └── Jenkinsfile
├── helm/
│   └── banking-service/    # One reusable chart for all services
│       ├── Chart.yaml
│       ├── values.yaml
│       ├── values-dev.yaml
│       ├── values-uat.yaml
│       ├── values-prod.yaml
│       └── templates/
├── infra/                  # Terraform for ACR and AKS
└── azure-pipelines/
    └── release.yml         # CD pipeline
