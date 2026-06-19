# IaC Examples

This is my collection of Infrastructure as Code (IaC) examples. IaC is the management and provisioning of IT infrastructure—such as servers, networks, and databases—using machine-readable definition files rather than manual click-through configuration. By treating infrastructure setup as software code, I automate, version-control, and replicate environments, eliminating manual, error-prone, and slow processes.

I also illustrate keeping IaC DRY (Don't Repeat Yourself) using tools like [OpenTofu](https://opentofu.org) and [Terragrunt](https://terragrunt.gruntwork.io).

## Structure

Each example lives in its own subdirectory under the relevant tool folder (e.g. `opentofu/`, `ansible/`). Every example is minimal and focused on a single concept or pattern, with its own README explaining what it does, what it creates, and any prerequisites.

## CI

This repo uses [Woodpecker CI](https://woodpecker-ci.kevininscoe.com) for automated pipeline runs.

## Prerequisites

- [OpenTofu](https://opentofu.org/docs/intro/install/) — `tofu` CLI
- [Terragrunt](https://terragrunt.gruntwork.io/docs/getting-started/install/) — `terragrunt` CLI (for DRY examples)

## Usage

Each example directory is standalone. Navigate into one and follow its README:

```sh
cd opentofu/some-example
tofu init
tofu plan
tofu apply
```

## License

Licensed under the [Apache License 2.0](LICENSE).
