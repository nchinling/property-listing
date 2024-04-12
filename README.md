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

```
- name: Check out repository code
        uses: actions/checkout@v4
```
1) Clones the repository to the runner so that steps in the pipeline can be executed. 

```
   run: ls ${{ github.workspace }}
      
```
2) List all files in the repository.

```
    - name: Install Angular CLI and dependencies
    run: |
        npm install -g @angular/cli
        npm install
      
```
3) - Enables use of Angular's use of 'ng' command in pipeline.
   - Installs dependencies (files) listed in package.json









