# AWS API Event Terraform module

Terraform module which creates a Lambda with a ready-to-use NodeJS source code to handle
event receiving on AWS.

## Usage

```hcl
module "lambda-api-event" {
  source = "genstackio/layer-api-event/aws//modules/lambda"

  name   = "my-lambda-api-event"
}
```
