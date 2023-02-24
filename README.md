# uds-infra
Foundational project for Unicorn Delivery Service's infrastructure layer, composed of reusable IaC modules and reusable prepackaged compliant environments. Nickname: edafos (greek for "foundation" or "ground")

## Reusable IaC Modules

* [terraform-aws-tfstate-backend](https://github.com/defenseunicorns/terraform-aws-tfstate-backend) - Reusable Terraform module that creates a Terraform Remote Backend via AWS S3 and AWS DynamoDB.
* More modules coming soon!

> Other modules we are working can be found [here](https://github.com/defenseunicorns/iac/tree/main/modules). As we transition to a more reusable approach to infrastructure, we will incrementally move those modules to their own repositories so that they can be versioned and consumed independently.


## Reusable Prepackaged Compliant Environments

* Coming soon!

> Initial work on reusable prepackaged compliant environments can be found [here](https://github.com/defenseunicorns/iac/tree/main/examples/zarf-complete-example). As we transition to a more reusable approach to infrastructure, we will incrementally move those packages to their own repositories so that they can be versioned and consumed independently.
