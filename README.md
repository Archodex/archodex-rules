# Archodex Rules

This repository contains the sources for the [Archodex Rules](https://archodex.com/docs/rulesets) repository.

## Deployment

The infrastructure is deployed using GitHub Actions. Rules are published for development agent releases on each merge to
the `main` branch. Rules are published for production agent releases on each tag push.

### Initial Deployment Setup

If you are not an Archodex developer you do not need to worry about deployments. If you are an Archodex developer and
want to set up deployments, ensure you have the following prerequisites:

1. **Fork Repository**: Create a personal fork of this repository.
2. **GitHub Repository Secrets**: Store the AWS IAM Role ARN for your environment's `ArchodexRulesGithubActionsRole` in
   the GitHub repository secrets as `ARCHODEX_RULES_AWS_ROLE_ARN`.
3. **Enable GitHub Actions**: Ensure that GitHub Actions are enabled for your forked repository.
4. **Manually Trigger Workflow**: Manually trigger the deploy workflow from the Actions tab in your forked repository.
