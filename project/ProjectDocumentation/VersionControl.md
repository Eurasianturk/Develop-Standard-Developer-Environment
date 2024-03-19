# Version Control Tools

## Introduction

Version control is an essential tool in the software development process. It allows developers to track and manage changes to the project codebase over time. By maintaining a detailed history of modifications, version control systems (VCS) facilitate collaboration among team members, ensure the integrity of the project, and allow for the safe experimentation of new features. In the context of Continuous Integration/Continuous Deployment (CI/CD) pipelines, version control plays a pivotal role in automating the build, test, and deployment processes.

## Version Control System Used

For this project, **Git** has been chosen as the version control system. Git is widely recognized for its robustness, flexibility, and support for distributed development workflows. It surpasses other VCS in terms of speed, data integrity, and support for non-linear development. Git's branching capabilities make it ideal for managing the project's lifecycle, from development through testing to production.

## Repository Setup

### Structure

The project repository follows a feature-branch workflow, where new features are developed in separate branches off the main branch. This strategy ensures the main branch always maintains a stable and deployable state. The repository's directory layout is organized into several key areas:

- `.devcontainer/`: Contains configurations for the Development Container.
- `src/`: The source code of the application.
- `tests/`: Automated tests for the application.
- `docs/`: Documentation related to the project.

### Integration

The repository is tightly integrated with the DevContainer environment and the CI/CD pipeline, facilitated by GitHub Actions. Upon each push to the repository, GitHub Actions triggers the CI/CD pipeline that runs tests, builds the application, and deploys it to the staging environment.

### Standards and Conventions

- **Commit Messages**: Follow the "Conventional Commits" format to enhance readability and automation.
  ```text
  git commit -m "feat(login): implement user authentication"
