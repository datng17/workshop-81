# AWS Application Load Balancer Advanced Features Workshop

A comprehensive hands-on workshop for implementing and managing advanced capabilities of AWS Application Load Balancer (ALB).

## Overview

This workshop provides practical guidance for configuring a highly available, performant, and intelligent application delivery solution using AWS ALB. Participants will learn to leverage advanced features critical for modern, scalable, and resilient applications.

## Architecture

The workshop implements a multi-tier architecture with:
- **VPC**: Isolated network environment with public/private subnets across 2 AZs
- **ALB**: Internet-facing load balancer with SSL termination and content-based routing
- **Auto Scaling Groups**: Three microservices (Web, API, WebSocket) with automatic scaling
- **Monitoring**: CloudWatch alarms, dashboards, and SNS notifications
- **Security**: Layered security groups and IAM roles

## Prerequisites

- AWS Account with appropriate permissions
- Domain name for SSL certificate
- Basic understanding of AWS services (VPC, EC2, ALB, Route 53)

## Workshop Modules

1. **Introduction** - Workshop overview and objectives
2. **Preparation** - Domain registration, IAM setup
3. **Network Infrastructure** - VPC, subnets, security groups
4. **SSL Certificate** - ACM certificate request and validation
5. **S3 Bucket** - Access logs storage setup
6. **Target Groups** - Health checks and routing configuration
7. **Application Load Balancer** - ALB creation and listener rules
8. **Launch Templates** - EC2 instance templates for microservices
9. **Auto Scaling Groups** - Automatic scaling configuration
10. **SNS Topic** - Notification setup
11. **CloudWatch** - Monitoring and alerting
12. **Cost Monitoring** - Budget and cost alerts
13. **DNS Configuration** - Route 53 setup
14. **Testing** - Validation and verification
15. **Performance Testing** - Load testing scenarios
16. **Cleanup** - Resource cleanup procedures

## Getting Started

### Local Development

1. **Install Hugo**:
   ```bash
   # Windows (using Chocolatey)
   choco install hugo-extended
   
   # macOS (using Homebrew)
   brew install hugo
   ```

2. **Clone and run**:
   ```bash
   git clone <repository-url>
   cd workshop-81
   hugo server -D
   ```

3. **Access locally**: http://localhost:1313

### Deployment

The workshop includes GitHub Actions workflow for automated deployment to GitHub Pages.

## Languages

- **English**: Primary language
- **Vietnamese**: Secondary language support

## Project Structure

```
workshop-81/
├── content/           # Workshop content in markdown
├── static/           # Images, CSS, JS assets
├── layouts/          # Hugo templates
├── themes/           # Hugo theme (hugo-theme-learn)
├── i18n/            # Internationalization files
├── config.toml      # Hugo configuration
└── .github/         # GitHub Actions workflows
```

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test locally with `hugo server`
5. Submit a pull request

## How this workshop was built

This workshop was developed using a documentation-as-code approach:

- **Hugo static site generator**: Chosen for fast builds, markdown support, and multilingual capabilities
- **Hugo learn Theme**: Provides structured navigation, search functionality, and mobile-responsive design
- **GitHub Actions CI/CD**: Automated deployment pipeline for seamless updates
- **Modular content structure**: Each workshop module is self-contained with step-by-step instructions and screenshots
- **Bilingual support**: English and Vietnamese content to serve diverse audiences

## Why this workshop was created

The motivation behind this workshop stems from real-world challenges:

- **Knowledge gap**: Many developers understand basic load balancing but struggle with advanced ALB features
- **Production readiness**: Moving beyond simple setups to enterprise-grade configurations
- **Hands-on learning**: Bridging the gap between theory and practical implementation
- **Cost optimization**: Teaching efficient resource management and monitoring practices
- **Community need**: Providing accessible, comprehensive AWS training in multiple languages

## Lessons learned

Key insights gained during workshop development:

### Technical insights
- **ALB complexity**: Advanced routing rules require careful planning and testing
- **Security layers**: Proper security group configuration is critical for microservices architecture
- **Monitoring strategy**: Proactive alerting prevents costly downtime
- **Auto scaling tuning**: Balancing responsiveness with cost efficiency requires iteration

### Educational approach
- **Progressive complexity**: Starting simple and building complexity prevents overwhelm
- **Visual learning**: Screenshots and diagrams significantly improve comprehension
- **Real-world scenarios**: Practical examples resonate better than theoretical concepts
- **Cleanup importance**: Teaching resource cleanup prevents unexpected AWS charges

## License

This project is licensed under the terms specified in LICENSE.md.
