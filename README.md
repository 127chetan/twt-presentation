# twt-presentation
Test GitHub repository to demo docs-as-code workflows with OpenAPI documentation updates.

## Prerequisites:
- VSCode
- NPM
- GitHub account
- GitHub repository
- Setup GitHub Actions
  1. Click **Settings** (at the top-right) in your created repository.
  2. Under **Code and automation** on the left, click **Pages**.
  3. Under **Build and deployment** for **GitHub Pages**, set the source as GitHub Actions.
  4. Click **Configure** for Static HTML. At preset static.yml file is created.
  5. Click **Commit changes**. Each time the OpenAPI file is updated and the repository is updated, GitHub Actions automatically builds the website.
- Installing redoc-cli: https://redocly.com/docs/cli/installation/#install-globally
- Using the redocly command: https://redocly.com/docs/cli/commands/build-docs/#usage
- Test petstore.yaml file: https://github.com/OAI/OpenAPI-Specification/blob/main/examples/v3.0/petstore.yaml

## Steps to build your docs-as-code workflow
1. Create a new GitHub repository.
2. Create a test-petstore.yaml file.
3. Clone the repository in VSCode.
4. Build HTML output from the YAML file: redocly build-docs test-petstore.yaml
5. Rename the HTML output to index.html: mv redoc-static.html index.html
6. Comment and push your changes to the repository. GitHub Actions automatically builds a website.
