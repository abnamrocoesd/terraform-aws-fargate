# Fargate with Terraform

Terraform module to deploy an ECS cluster with Fargate launch type.

```
module "fargate" {
  source                               = "github.com/abnamrocoesd/terraform-aws-fargate"
  cluster_name                         = "${local.cluster_name}"
  app_name                             = "${local.app_name}"
  app_image                            = "${local.app_image}"
  fargate_cpu                          = "${local.fargate_cpu}"
  fargate_memory                       = "${local.fargate_memory}"
}
```
