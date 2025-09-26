# GitHub Actions workflows with build
https://docs.github.com/en/actions/reference/workflows-and-actions/workflow-syntax

prebuild workflow can be created like the following way. In GitHub Actions, the permissions key within a workflow's YAML file controls the scope of the GITHUB_TOKEN for the entire workflow or for individual jobs. The permissions id-token: write, contents: write, and security-events: write grant specific access levels to different resources within your repository and GitHub's ecosystem.

**build.yml**

```
name : prebuild
permissions:
  id-token: write # Required for OIDC token requests
  contents: write # Required to modify repository contents
  security-events: write # Required to upload security scan results

on:
  push:
    branches:
      - main # Triggers on pushes to the 'main' branch
      - 'feature/*' # Triggers on pushes to any branch starting with 'feature/'
    paths:
      - 'src/**' # Triggers only if changes are within the 'src' directory or its subdirectories
      - 'config/*.yaml' # Triggers only if changes are made to .yaml files in the 'config' directory
jobs:
  build:
    uses: piyalidas10/Splunk-github-actions/blob/main/.github/workflows/{{main-artifcat}}.yml
```


**Here is a breakdown of these permissions:**
  -  id-token: write: This permission is required when your workflow needs to request an OpenID Connect (OIDC) JSON Web Token (JWT). OIDC is used for secure authentication and authorization with external cloud providers or services, allowing your GitHub Actions workflow to obtain temporary credentials to interact with those services without storing long-lived secrets in GitHub.
  -  contents: write: This grants write access to the repository's contents. This means the workflow can push commits, create branches, delete branches, and modify files within the repository. If you need to update files, create releases, or perform other write operations on the repository itself, this permission is necessary.
  -  security-events: write: This permission allows the workflow to upload security-related information to GitHub's security features, such as Dependabot alerts or CodeQL results. For example, if you are running a security scanning tool within your workflow and want to report the findings back to GitHub's security dashboard, this permission would be required.

**Explanation:**
  -  on: push:: This defines the event that triggers the workflow. In this case, it's a push event to the repository.
  -  branches:: This filter specifies which branches will trigger the workflow when a push event occurs. You can list specific branch names or use wildcard patterns (e.g., feature/* to match all branches starting with "feature/").
  -  paths:: This filter further refines the push trigger by specifying that the workflow should only run if changes are made to files within certain paths or directories in the repository. Wildcards can also be used here (e.g., src/** for any file or directory within src, or config/*.yaml for .yaml files directly within config).
  - 
