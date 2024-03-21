# demo-repository-defaults

demo repository to document and demonstrate default settings for any natureOffice development repository.
> Please note: This is a **template repository**, please use it if you create a new repository for development purposes. Further details can be found in the official `GitHub` [docs](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template).

- [Introduction](#introduction)
- [Features](#features)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation--usage)
- [Documentation](#documentation)
- [FAQ](#faq)
- [TODO](#todo)
- [Contact](#contact)

## Introduction

This demo repo should provide a **template for all natureOffice repositories** and also document the repository **standards** and **defaults** we use.
Whenever a new repository is created **this repository should be used as a blueprint** to save setup time by reusing all the pre-configurations.

## Features

As explained above this repository provides common **settings** as well as the following **files**:

### Provided Settings

| setting | description | remark  |
| -------- | ----------- | --------- |
| `branches` | all default branches are configured | The current default branches are `main` and `develop`
| the default branch is `develop` | use `develop` branch as repo default that devs do not have to switch branches after checkout | already set in template |
| the `main` branch is protected | protected `main` branch to secure a versioned state against direct manipulations *(if `release` or `stating` branches will be used this might be needed there as well)* | manipulation example: `push -f` (force push) |
| `common PR setting`| All changes must be added to the default branches by using a `PR`, every `PR` must be reviewed and approved by **two team members** | four-eyes principle |


### Provided Files

| default | description | example | reference |
| -------- | ----------- | ------- | --------- |
| `.gitignore` | default `.gitignore` file that is added to any repository | exclude `.DS_Store` files on mac | the included `.gitignore` was generated using [toptal.com](https://www.toptal.com/developers/gitignore/api/macos,linux,windows,visualstudiocode,vue,vuejs,node,nuxtjs), but additional modifications were added   |
| `README.md` | file that provide the description you are currently reading  | the default scheme of the readme can be found in `README.blueprint.md` |
| `README.blueprint.md` | `README.blueprint.md` [markdown](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax) template you should use to create the `README.md` of your repository  |  | `README.md` [markdown](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax) file should provide a comprehensive introduction to the project, including its purpose, features, and usage instructions |
| `CODEOWNERS` | `CODEOWNERS` file for managing a collaborative and secure development process, ensuring that all changes are reviewed by individuals with the appropriate expertise and responsibility. |  | [About code owners](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-code-owners) (official `GitHub` Documentation) |

## Getting Started

### Prerequisites

- you need the permission to create repositories within the **natureOffice** `organization` in order to create repositories based on this template. 

### Installation & Usage

For using this template for your repository, please follow the official [`GitHub` guide](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template).

> Please Note: if you use this Template all these setting will be cloned by default.

## Documentation

### 1. **Use a Clear and Descriptive Names for your repository**
The repository name should reflect the purpose or functionality of the project it contains.

Please refer to the following guideline:

- **Scheme:** `[application-name]-[type]:-[version]`
- **Version**: the version tag: `-[version]` is optional and should be added, if needed, at the end of the name
- **Example:** application-names: `ecozoom-pro` or `ecozoom-direct`
- **Example:** types: `frontend`, `backend`, or `loadbalancing-service`
- **Result:** `ecozoom-pro-frontend`, `ecozoom-direct-backend-V1`, `ecozoom-pro-loadbalancing-service-V2`

### 2. **Transparency & Communication**

Please keep all communication **close to the code**! This means that you should add all discussions and decisions into MR/PR comments **to documented decisions and processes** in order to improve **transparency** for all (future-) team-members.
- **Example:** add comment on MR/PR, even if you had a call about something 

### 3. **Code of Conduct**
   - All participants must ensure a welcoming and respectful community and communication (no silos, no single fighters).
   > Please find more information in our [team notion](https://www.notion.so/Team-Workflow-4b67094125a64a8c9af57f32a4ad88f3)

### 4. **Use Branches and Pull Requests**
   - Feature branches and pull requests are essential for managing contributions and reviewing code changes effectively.
   - A common commit convention and branching strategy will be discussed ASAP!

### 5. **Keep a Clean Commit History**
   - Squash related commits and write meaningful commit messages to maintain a readable history.

   > Please Note: The option to squash commits from the UI within the PR interface is already enabled within the repo settings

### 6. **Document the Code**
- Good in-code comments and documentation make the code more understandable and accessible.

## FAQ

- **Does this template repository include default `CI/CD workflows`?** Currently, this is not the case but will be added soon (please check the **TODO Section**)

## TODO
- discuss branch naming convention (could be checked by [GitHub
Rulesets](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-rulesets/about-rulesets))?
- discuss branching strategy should be used (e.g., gitflow,
trunk-based)?
- discuss release versions + tags (conventional commits + semantic versioning)
- discuss security (e.g., dependency management)
- discuss signed commits
- discuss `Badges`: [internal ci badges](https://docs.github.com/en/actions/monitoring-and-troubleshooting-workflows/adding-a-workflow-status-badge), [external universal badges 1](https://github.com/badges/shields), [external universal badges 2](https://github.com/dwyl/repo-badges)

### **(CI/CD workflows) Automate Testing and Integration**
   - Use continuous integration tools to automate testing and ensure that changes do not break existing functionality.

The default `ci workflow` (not established yet) will be added to any new repository. The majority of coding standards will be enforced out of the box (e.g., all files will be linted).

## Contact

natureOffice GmbH - [website](natureoffice.com) | [e-Mail](mailto:it@natureoffice.com)

