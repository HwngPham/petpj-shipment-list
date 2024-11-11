# PJ🐶: Shipment list

An application which deals with CRUD operations a person can execute on a bunch of shipments that they're allowed to view - think of it like the Post app. The demo consists of a backend and a frontend implementation, using React to display the information. The AWS services involved are:

- S3 for storing pictures.
- DynamoDB for the entities.
- Lambda function that will validate the pictures, apply a watermark and replace non-compliant files.
- SNS that receives update notifications.
- SQS that subscribes to a topic and delivers the messages.

## Architecture Overview

![Diagram](assets/app_diagram.png)

## Prerequisites

- [Localstack](https://www.localstack.cloud/)
- [Docker](https://www.docker.com/)
- [Terraform](https://developer.hashicorp.com/terraform)
- [Pnpm](https://pnpm.io/)
