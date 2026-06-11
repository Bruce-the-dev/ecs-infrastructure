# helloapp Infrastructure

CloudFormation templates for deploying the helloapp Spring Boot application
on AWS ECS Fargate with blue/green deployments.

## Stacks

| Stack | Template | Purpose |
|---|---|---|
| Network | `templates/network-stack.yaml` | VPC, subnets, IGW, route tables |
| Compute | `templates/compute-stack.yaml` | ALB, ECS cluster, service, auto scaling |
| Pipeline | `templates/pipeline-stack.yaml` | CodeDeploy, CodePipeline, EventBridge |

All stacks are deployed via CloudFormation GitSync.

## Companion Repo

Application code: https://github.com/Bruce-the-dev/ecs_ci-cd_lab 