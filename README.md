# Terraform Beginner Bootcamp 2023

## Semantic Versioning  :mage:
This project is going to utilize semantic versioning for its tagging
[semver.org](https://semver.org/)

The general format:

**MAJOR.MINOR.PATCH**, eg. `1.0.1`

- MAJOR version when you make incompatible API changes
- MINOR version when you add functionality in a backward compatible manner
- PATCH version when you make backward compatible bug fixes
Additional labels for pre-release and build metadata are available as extensions to the MAJOR.MINOR.PATCH format.

## Install the Terraform CLI

### Considerations with the Terraform CLI changes
The Terraform CLI installation instructions have changed due to gpg keyring changes.  So we needed to refer to the latest in CLI installation instructions via Terraform documentation and chagne the scripting for install.

[Install Terraform CLI](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli)

### Refactoring into Bash Scripts

While fixing the Terraform CLI gpg deprecation issues we noticed that the bash scripts steps were a considerable amount more code.  We decided to create a bash script to isntall the Terraform CLI. 

This bash script is located here: 

- This will keep the Gitpod Task File ([.gitpod.yml](.gitpod.yml)) tidy.
- This will allow us an easier time to debug and execute manual Terraform CLI install
- This will allow better portability for other projects that need to install Terrform CLI.
