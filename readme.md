# SIT753 7.3C Task

## Part 1, Task 1: Jenkins Integration via Poll SCM

- Jenkins job: Pipeline (Pipeline script from SCM) pointing to this repo, branch `main`.
- Trigger: Poll SCM (hash-spread every 2 minutes). New commits start a build.
- Stages (task, tool):
  - Build: npm, 
  - Tests: Jest,
  -  Code Analysis: ESLint, 
  -  Security: OWASP Dependency-Check, 
  -  Deploy Staging: Ansible, 
  -  Staging Tests: Newman CLI, 
  -  Deploy Prod: Ansible/Terraform.