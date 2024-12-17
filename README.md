# setup-terraform-action

Set up your GitHub Actions workflow with a specific version of Terraform.

<!-- actdocs start -->

## Description

This action sets up [Terraform CLI](https://www.terraform.io/) and
[tfcmt](https://github.com/suzuki-shunsuke/tfcmt) in your GitHub Actions workflow by:

- Installing a specified version of Terraform CLI and tfcmt
- Verifying the authenticity and integrity of the downloaded binaries to prevent tampering
- Setting the `TF_PLUGIN_CACHE_DIR` environment variable to enable the plugin cache

This enables Terraform CLI commands to execute just like they do on your local environment.
Additionally, tfcmt simplifies commenting on the results of Terraform CLI commands in pull requests.

## Usage

```yaml
  steps:
    - name: Setup Terraform
      uses: tmknom/setup-terraform-action@v0
      with:
        terraform-version: 1.2.3
        tfcmt-version: 4.14.0
```

## Inputs

| Name | Description | Default | Required |
| :--- | :---------- | :------ | :------: |
| terraform-version | The version of Terraform CLI to install. | `latest` | no |
| tfcmt-version | The version of tfcmt to install. | `latest` | no |

## Outputs

N/A

<!-- actdocs end -->

## Permissions

N/A

## FAQ

N/A

## Related projects

N/A

## Release notes

See [GitHub Releases][releases].

[releases]: https://github.com/tmknom/setup-terraform-action/releases
