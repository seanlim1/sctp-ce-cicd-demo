# sctp-ce-cicd-demo

## CI Workflow
1. Read the terraform files and attempt to draw the architecture diagram
2. Fill the values with the `to replace` comments
3. Get CI workflow to run. Fix if unsuccessful.

> Always check the plan before deployment

## Simple Deployment
1. Get Simple CD workflow to run

## Blue-Green
1. Uncomment all green deployment codeblocks
2. Get Blue-Green CD workflow to run

# Test
Use the the command to make a call to the service repeatedly
```bash
for i in `seq 1 10`; do curl $(terraform output -raw lb_dns_name); done
```

## references
- https://learn.hashicorp.com/tutorials/terraform/blue-green-canary-tests-deployments
