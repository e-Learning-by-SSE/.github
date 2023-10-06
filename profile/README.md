## Developer Guide for E-Learning Projects by SSE

Hello there 👋,

Welcome to the repository for e-learning projects managed by [SSE](https://sse.uni-hildesheim.de/). If you're developing a service within our ecosystem, please read the following sections carefully.

## Resources for SSE Developers

- [Contributing Guidelines](https://github.com/e-Learning-by-SSE/.github/blob/main/CONTRIBUTING.md) (e.g., how to create commits and branches)

#### Internal Resources

- [Administrative Board](https://github.com/orgs/e-Learning-by-SSE/projects/1)
- [Board and Process Description](https://github.com/e-Learning-by-SSE/nm-concept/blob/main/doc/BOARD.md)
- [People, Responsibilites and Mails](TODO)

#### Important Repositories

- [Selflearn Repository (Digital Campus)](https://github.com/e-Learning-by-SSE/nm-self-learning)
- [nm-skill-lib Repository (Path Planner Library)](https://github.com/e-Learning-by-SSE/nm-skill-lib)
- [nm-skill-service Repository (Service for SEARCH)](https://github.com/e-Learning-by-SSE/nm-skill-service)

## Repository Naming Scheme

To maintain consistency, we use a specific repository naming scheme. Each repository name consists of three sections separated by hyphens: `<project-prefix>-<project-name>-<type>`.

|Prefixes in Use|Description|
|---|---|
|`infrastructure`|Cross-cutting concerns like authentication and infrastructure services like application gateways|
|`nm`|"Nano-Module": Projects for micro-learning|
|`exercise-submission`|Projects related to teaching and exercise submissions (in Java)|
|`stu`|Projects around the Student Management System (and older Q+ Projects)|

|Types|Description|
|---|---|
|`lib`|Libraries to be used in other projects|
|`service`|Applications that provide an API for clients (backends)|
|`client`|Applications that consume another API (frontends)|
|`app`|Monolithic apps that provide everything they need (frontend, backend, lib)|
|`common`|Shared resources or utilities|

### Infrastructure

We offer an infrastructure for cross-cutting concerns, which includes:

- Runtime Service Registry
- Application Gateway
- OIDC Authentication

Any service providing an API must at least register itself in the registry. For more details, refer to the [Developer Guide](https://github.com/e-Learning-by-SSE/infrastructure-common/blob/master/usage.md).
