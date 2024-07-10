### Secret-Scanning-Check
GitHub Actions Check - Secret Scanning; An added layer of visibility.

This GitHub Action checks for unresolved secret scanning alerts when a pull request is opened or reopened. If any unresolved alerts are found, the action will fail and report an error.

#### Usage

1. **Create a Secret**: Add a secret named `APP_TOKEN` in your GitHub repository settings with your GitHub token.

2. **Create Workflow**: Add the workflow [YAML file](secret-scanning-check.yml) to your repository at `.github/workflows/secret-scanning-check.yml`.

## Example Workflow File

Refer to the [`.github/workflows/secret-scanning-check.yml`](.github/workflows/secret-scanning-check.yml) file in your repository.

## Notes

- Ensure your `APP_TOKEN` has the necessary permissions to access secret scanning alerts.
- This action uses `jq` to process JSON data from the GitHub API.
- I love this check so much, I wanted to create a dedicated repository for it and recommend everyone use it.
