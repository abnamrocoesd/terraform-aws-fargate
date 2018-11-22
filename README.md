# Fargate with Terraform

Terraform module to deploy an ECS cluster with Fargate launch type.

```
module "fargate" {
  source                               = "github.com/abnamrocoesd/terraform-aws-fargate"
  cluster_name                         = "${var.cluster_name}"
  app_name                             = "${var.app_name}"
  app_image                            = "${var.app_image}"
  fargate_cpu                          = "${var.fargate_cpu}"
  fargate_memory                       = "${var.fargate_memory}"
}
```
