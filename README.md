# githubActionsKitten

## Overview

This repository demonstrates how to use environmental variables as input to control the execution of a GitHub Workflow. It is designed to help you understand how environment variables can be leveraged to make your CI/CD pipelines more flexible and dynamic.


## How to Use

To control whether the workflow runs the ASCII kitten script, simply change the value of the environmental variable `ASCII_KITTEN` in `.github/workflows/kitten_build.yml`:

```yaml
env:
	ASCII_KITTEN: "true"   # change to "true" or "false" to run or skip running kitten.sh
```

- Set `ASCII_KITTEN: "true"` to run the `kitten.sh` script when the workflow is triggered by a push to the `main` branch.
- Set `ASCII_KITTEN: "false"` to skip running the script.

Commit and push your change to the repository. The workflow will execute according to the value you set.

## Environmental Variables in GitHub Actions

- **Definition:** Environmental variables are key-value pairs that can be used to pass configuration, secrets, or control logic to your workflows.
- **Usage:**
	- Set at workflow, job, or step level.
	- Access with `$VAR_NAME` in shell scripts or `${{ env.VAR_NAME }}` in workflow YAML.
	- Useful for controlling build modes, toggling features, or passing secrets securely.

## Authorship

Created and maintained by [RZFeeser](https://github.com/RZFeeser).

## Contact

- Website: [rzfeeser.com](https://rzfeeser.com)
- Projects & Training: [iris7.com](https://iris7.com)
- GitHub: [RZFeeser](https://github.com/RZFeeser)

## Note

I train and teach on a wide range of technologies, including:

- GitHub Actions
- GitLab Pipelines
- Jenkins
- Terraform
- Ansible
- Docker
- Kubernetes
- Cloud platforms (AWS, Azure, Google Cloud)
- Python automation
- And other trending DevOps and cloud-native tools

If you have questions or want to learn more about any of these topics, feel free to reach out!