## Requirements

No requirements.

## Providers

The following providers are used by this module:

- <a name="provider_aws"></a> [aws](#provider\_aws)

## Modules

No modules.

## Resources

The following resources are used by this module:

- [aws_instance.wordpress_os](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/instance) (resource)
- [aws_security_group.public_sg](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group) (resource)
- [aws_security_group_rule.sg_egress_public](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group_rule) (resource)
- [aws_security_group_rule.sg_ingress_public_22](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group_rule) (resource)

## Required Inputs

The following input variables are required:

### <a name="input_public_ids"></a> [public\_ids](#input\_public\_ids)

Description: The IDs of the public subnets

Type: `list(string)`

### <a name="input_vpc_id"></a> [vpc\_id](#input\_vpc\_id)

Description: The ID of the VPC

Type: `string`

## Optional Inputs

The following input variables are optional (have default values):

### <a name="input_env"></a> [env](#input\_env)

Description: Name to be used on all the resources as identifier. e.g. Environment name

Type: `string`

Default: `"env"`

## Outputs

No outputs.
