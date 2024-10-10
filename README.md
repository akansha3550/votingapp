# votingapp
## Overview
This repository contains the setup and deployment instructions for a Voting App running on AWS EKS (Elastic Kubernetes Service). The application leverages Kubernetes to manage containerized services, providing scalability and high availability.

## Setup Instructions

### Prerequisites
Ensure you have the following installed on your EC2 instance:
- **AWS CLI**: For AWS service management.
- **kubectl**: Kubernetes command-line tool.
- **eksctl**: A command-line tool for creating EKS clusters.

##Application Stack
This application is built using the following technologies:

1. Frontend: Python-based web application for user interactions.
2. Backend:
 - .NET service for processing votes.
 - Node.js service to display real-time voting results.
3. Messaging: Redis is used to manage message queues.
4. Database: PostgreSQL serves as the primary storage solution.#
