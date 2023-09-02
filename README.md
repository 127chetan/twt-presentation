# twt-presentation
Test GitHub repository to demo docs-as-code workflows with OpenAPI documentation updates.

## Prerequisites:
- VSCode
- NPM
- Create a GitHub account
- Create a GitHub repository
- Set up GitHub Actions in the repository
- Starter OpenAPI spec for testing: https://github.com/OAI/OpenAPI-Specification/blob/main/examples/v3.0/petstore.yaml

## Steps to set up your own repository and GitHub Actions
1. Create a new GitHub repository.
2. Create a test-petstore.yaml file in the repository. Copy the contents from https://github.com/OAI/OpenAPI-Specification/blob/main/examples/v3.0/petstore.yaml as an example.
3. Set up GitHub Actions in the repository.
    1. Click **Settings** (at the top-right) in your created repository.
    2. Under **Code and automation** on the left, click **Pages**.
    3. Under **Build and deployment** for **GitHub Pages**, set the source as GitHub Actions.
    4. Click **Configure** for Static HTML. A preset static.yml file is created.
    5. Click **Commit changes**.
    6. Copy the static.yml contents from this twt-presentation repository to your repository and commit your changes.
4. Clone the repository in VSCode. Each time you save changes to your OpenAPI yaml file and push your changes to GitHub, GitHub Actions automatically builds API documentation output.
