# uds-infra
Foundational project for Unicorn Delivery Service's infrastructure layer, composed of reusable IaC modules and reusable prepackaged compliant environments. Nickname: edafos (greek for "foundation" or "ground")

## Vision

Edafos is the lowest layer of the Unicorn Delivery Service (UDS). It is the foundation of the UDS product and is responsible for providing the infrastructure layer that is required for UDS to function. Edafos is composed of two main sets of components:

* Reusable Infrastructure as Code modules powered by Terraform (the modules)
* Reusable prepackaged compliant environments that use the modules, powered by Zarf (the packages)

As UDS matures, Edafos will become a component of UDS such that the user is just deploying UDS as a single package. However, Edafos will always be versioned, released, and deployable independently if so desired. In addition, the IaC modules will also be maintained such that they are usable independently if desired.

The overall vision for Edafos can be described with the following user story:

As a software engineering team that needs to deploy Kubernetes-based applications in an environment that is required to meet certain compliance standards,  
I want the ability to deploy the infrastructure for that environment in a repeatable, auditable, and compliant manner,  
so that I can spend more time doing what really matters, which is delivering mission value to my users.

The first prepackaged environment that Edafos will target is one that must meet [United States of America Department of Defense Impact Level 5 (IL5) requirements](https://cic.gsa.gov/basics/cloud-security) plus the [I.T. Control Requirements for Unclassified Naval Unclear Propulsion Information (U-NNPI)](https://irp.fas.org/doddir/navy/opnavinst/n9210_3.pdf) in Amazon Web Services (AWS). Prepackaged environments that meet other compliance standards and in other Cloud Service Providers and On-Premise, will be added as the project matures.

## Reusable IaC Modules

* [terraform-aws-tfstate-backend](https://github.com/defenseunicorns/terraform-aws-tfstate-backend) - Reusable Terraform module that creates a Terraform Remote Backend via AWS S3 and AWS DynamoDB.
* More modules coming soon!

> Other modules we are working can be found [here](https://github.com/defenseunicorns/iac/tree/main/modules). As we transition to a more reusable approach to infrastructure, we will incrementally move those modules to their own repositories so that they can be versioned and consumed independently.


## Reusable Prepackaged Compliant Environments

* Coming soon!

> Initial work on reusable prepackaged compliant environments can be found [here](https://github.com/defenseunicorns/iac/tree/main/examples/zarf-complete-example). As we transition to a more reusable approach to infrastructure, we will incrementally move those packages to their own repositories so that they can be versioned and consumed independently.
