---
name: Project Setup
about: Prepare for development with basic project setup.
title: Project Setup
labels: ''
assignees: ''

---
<!-- ### PORT THIS INTO A K8S DEPLOYED SERVICE ### -->

<!-- Please check off line-items as they are completed and leave notes if necessary. -->
<!-- If an item is not relevant to this project, [strike it out](https://docs.github.com/en/github/writing-on-github/basic-writing-and-formatting-syntax#styling-text) -->
<!-- (e.g. `~~Not relevant item~~`) or remove it. If child tickets are created for -->
<!-- any line-item, please update this description to include references to them. -->

- [ ] Create a README.
- [ ] Set up [Tugboat](https://dashboard.tugboat.qa/).
- [ ] Create an AWS user and S3 bucket with an access policy and bucket lifecycle rule for database backups ([documentation](https://github.com/jucr-io/engineering-handbook/blob/main/technical/database-backup-aws-s3.md)).
- [ ] Set up Dependabot ([example](https://github.com/jucr-io/jucr.de/blob/master/.github/dependabot.yml)).
- [ ] Set up PHP code style checks.
- [ ] Set up GitHub Actions [example] (<https://github.com/jucr-io/.github/workflows>) to run code style checks on YML, shell scripts, and execute PHP checks/front-end linting tools.
- [ ] Set up `settings.php` file infrastructure.
- [ ] Set up a `composer.json` file.
- [ ] Create a theme at `web/themes/custom/THEME_NAME`.
- [ ] Set up front-end tooling with [Calliope](https://github.com/jucr-io/calliope).
  - [ ] A task to build the theme's static assets.
  - [ ] Development workflow tasks to build assets automatically, watch for changes, refresh the browser automatically, etc.
  - [ ] CSS and JS linting tasks, as well as any other testing tasks that relevant to the project.
- [ ] Document system-level requirements and step(s) to build theme assets in remote environments in the theme's README.
- [ ] Update build scripts (used in Tugboat, production, and elsewhere) to install front-end dependencies and build theme assets.
- [ ] Update GitHub Actions to run any front-end linting and/or testing tasks.
- [ ] Set up a production environment.
- [ ] Set up nightly database backups to S3.
- [ ] Set up automated deployments.
