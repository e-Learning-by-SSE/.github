## Hi there 👋

This is the repository for e-learning projects by [SSE](https://sse.uni-hildesheim.de/). 

# Developer Guide
If you develope a service in our ecosystem please read the following sub-sections carefully. 

## Development Process
We provide a documentation of various aspects of our development progress here:
- [Commit Guideline](https://github.com/e-Learning-by-SSE/nm-self-learning/wiki/Commit-Guidelines)
- Branching Guideline
- [Project Board Description / Development Process](https://github.com/e-Learning-by-SSE/nm-self-learning/wiki/Project-Management)

## Infrastructure
We provide an infrastructure for cross-cutting concerns which includes:
- Runtime service registry
- Application gateway
- OIDC Authentication

Any service which provides an API must at least register themselfes in the registry. You can find a developer guide [here](https://github.com/e-Learning-by-SSE/infrastructure-common/blob/master/usage.md)

## Repository Naming Scheme
This group use a repository naming scheme to make it easier to find stuff. Please comply with this.

Each repository have three sections spereated with hyphen:
`<projectprefix>-<projectname>-<type>`

| prefix in use       | description                                                                                     |
|---------------------|-------------------------------------------------------------------------------------------------|
| infrastructure      | Cross Cutting Concerns like authentication and infrastructure service like application gateways |
| nm                  | "Nano-Module": Projects for micro learning                                                      |
| exercise-submission | Projects from teaching and exercise submitting (in java)                                        |
| stu                 | Project around the Student-Management System (and old Q+ Projects)

| types   | description |
|---------|-------------|
| lib     | Library to be used in other project                                       |
| service | Application which provides an API for clients (backends)                  |
| client  | Application which consumes another API (frontends)                        |
| app     | Monolithic app which provides everything it needs (frontend, backend lib) |
| common  |  | 

<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
