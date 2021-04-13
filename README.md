# Terraform provider npm

> **Note:** This is an experiment to replace the [NPM Download Terraform module](https://github.com/dealmore/terraform-npm-download) with an appropriate provider.

The goal of this project is to enable local downloads from [npm](https://www.npmjs.com/) like this:

```tf
data "npm_package_file" "this" {
  name    = "@dealmore/terraform-next-proxy"
  version = "0.5.0"
  file    = "dist.zip"
}
```
