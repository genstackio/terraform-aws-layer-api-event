# AWS API Event Layer Terraform module

Terraform module which creates an entire layer (i.e. module to be contained in its own tfstate).
It manage an API Gateway v2 linked to a Lambda with a ready-to-use NodeJS source code to handle
event receiving on AWS.

## Usage

```hcl
module "main" {
  source     = "genstackio/layer-api-event/aws"

  env        = "prod"
  dns        = "event.mydomain.com"
  dns_zone   = "id-of-the-route53-zone"
}
```
