# Github Actions (CI/CD)
Description: Setting up a Continuous Integration / Continuous Deployment pipeline with Github Actions

## Web App 
A property listing site developed with Angular (WIP...)

![](src/assets/images/app.png)

## Why CI/CD Pipeline?

- **Facilitates Continuous Integration and Deployment**: Streamlines the process of integrating code changes into the main codebase and deploying them to production. 

- **Upholds Code Standards**: Enforces rigorous code standards such as testing, linting, security checks, and vulnerability scanning. This ensures code quality and integrity across the development pipeline compared to local development environments.


## Implementation
- Workflow is triggered on 'push' to any branch. 
- There is only job: 'Explore Github Actions'
- Runs on latest version of Ubuntu

1) actions/checkout@v4 -> Clones the repository to the runner so that pipeline steps can be performed. 
2) ls ${{ github.workspace }} -> list all files in the repository
3) 

