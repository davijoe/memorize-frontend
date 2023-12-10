# CI/CD Demonstration of group project
Related group project : [PlaceholderOrganization/memorize-frontend](https://github.com/PlaceholderOrganization/memorize-frontend)

## Resource Links
**Backend**

1) Repo: [davijoe/memorize-backend](https://github.com/davijoe/memorize-backend)
2) Live: [Deployed-Webapp-main](main-backend-memorize.azurewebsites.net)
3) Test: [Deployed-Webapp-staging](staging-backend-webapp.azurewebsites.net)
4) Dev : [Deployed-Webapp-dev](dev-backend-memorize.azurewebsites.net)
   

**Frontend**

1) Repo: [davijoe/memorize-frontend](https://github.com/davijoe/memorize-frontend)
2) Live: [www.danviktor.dk](https://www.danviktor.dk)
3) Test: [staging-test.danviktor.dk](https://staging-test.danviktor.dk)
4) Dev : [dev-test.danviktor.dk](https://dev-test.danviktor.dk)

### Database
Created as a MySQL database running in a docker container a Linux VM on Azure

### Branching Strategy
We use the 'main' branch as our released codebase. For new developments, we create feature branches from our development branch. Once a feature is complete, we initiate a pull request to merge it into the 'development' branch. This triggers automated builds and tests via GitHub Actions, and if successful, the changes are deployed to Azure Dev Web App service. When the sprint is complete, we deploy our successfully deployed development branch to our staging branch for further testing. When customer accepts the changes, we merge staging into main.

**Key elements in strategy**
 - Main Branch (live production)
 - Staging Branch (pre-production)
 - Development Branch (continous development)
 - Feature Branches
 - Pull Requests (Approval required from another team member)
 - Continuous Integration (CI) with GitHub Actions
 - Deployment with Azure Web App Service
 - Merging Staging into Master
