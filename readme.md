# Demo for Spring Boot Extension Pack

## Spring Boot Extension Pack

The Spring Boot Extension Pack is a collection of extensions that provide support for developing Spring Boot applications in Visual Studio Code. The extensions included in the pack are:

- Extensions included in the pack

## Inner Loop Demo

The Inner Loop Demo is a demonstration of the end-to-end Spring development experience in Visual Studio Code. It includes the following steps:

- Getting Started
  - Spring Initializr integration
  - Use Spring Petclinic from Getting Started guide
- Spring Tooling
  - Run the application and access it through the code lenses
  - Refresh Live Process connection to update IDE with metrics
  - Code navigation, project symbols
  - Show live Hovers
- Debugging
  - Show debugging flow and hot code replace
- Spring Boot Dashboard
  - Show beans, mappings, memory views
  - Talk about Spring Boot auto-configuration insights
- Testing
  - JUnit Test runner to execute tests without leaving the IDE
- (Optional) Talk about Spring validations - best practices while coding
- Summarize the end-to-end Spring development experience

## Outer Loop Demo

The Outer Loop Demo is a demonstration of the end-to-end Spring development experience in Visual Studio Code, including the steps to monitor, migrate, build, deploy, and Q&A. It includes the following steps:

- MONITOR
  - EXPLAIN Codespaces
  - OPEN "Azure Spring Apps extension"
  - OPEN "Application Live View"
  - OPEN "View Live Information"
    - OPEN OwnerController.java
    - REFRESH ">Spring boot: manage live spring boot process connections"
    - DEMO
      - Beans
      - Endpoint mapping
  - DEBUG
- MIGRATE
  - OPEN ">Spring boot: upgrade spring boot version"
    - EXPLAIN openrewrite recipes from Spring Boot language server (3 levels down)
    - (Optional) Show validations for best practices using openrewrite
  - MIGRATE
  - COMMIT
  - Build
    - `mvn package -DskipTests`
- DEPLOY
  - OPEN springone.yml
    EXPLAIN
    - BUILD
    - Containerize
    - ROLL-OUT

- Q&A

## Appendix

To create an Azure User for the action:

- `az ad sp create-for-rbac --name springone --role contributor --scopes /subscriptions/<your sub>/resourceGroups/springoneent --sdk-auth`

Extension:

https://network.tanzu.vmware.com/products/tanzu-java-azure-buildpack