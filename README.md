# setup-terraform-action

Set up your GitHub Actions workflow with a specific version of Terraform.

<!-- actdocs start -->

## Description

This action sets up [Terraform CLI](https://www.terraform.io/) in your GitHub Actions workflow by:

- Downloading a specified version of Terraform CLI and adding it to the `PATH`
- Verifying that the downloaded binary is created and signed by HashiCorp before installation
- Setting the `TF_PLUGIN_CACHE_DIR` environment variable to enable the plugin cache

This enables Terraform CLI commands to execute just like they do on your local environment.

## Usage

```yaml
  steps:
    - name: Setup Terraform
      uses: tmknom/setup-terraform-action@v0
      with:
        terraform-version: 1.2.3
```

## Inputs

| Name | Description | Default | Required |
| :--- | :---------- | :------ | :------: |
| terraform-version | The version of Terraform CLI to install. | `latest` | no |

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

## License

Apache 2 Licensed. See [LICENSE](LICENSE) for full details.

[releases]: https://github.com/tmknom/setup-terraform-action/releases
