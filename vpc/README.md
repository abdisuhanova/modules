## Requirements

No requirements.

## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | n/a |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [aws_eip.main](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/eip) | resource |
| [aws_internet_gateway.main](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/internet_gateway) | resource |
| [aws_nat_gateway.main](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/nat_gateway) | resource |
| [aws_route.main](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route) | resource |
| [aws_route_table.main](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table) | resource |
| [aws_route_table_association.internet_access](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association) | resource |
| [aws_subnet.private](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet) | resource |
| [aws_subnet.public](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet) | resource |
| [aws_vpc.vpc](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/vpc) | resource |
| [aws_availability_zones.available](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/availability_zones) | data source |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_env"></a> [env](#input\_env) | Name to be used on all the resources as identifier. e.g. Environment name | `string` | `"env"` | no |
| <a name="input_private_subnets_count"></a> [private\_subnets\_count](#input\_private\_subnets\_count) | The number of private subnets. | `number` | `2` | no |
| <a name="input_public_subnets_count"></a> [public\_subnets\_count](#input\_public\_subnets\_count) | The number of public subnets. | `number` | `2` | no |
| <a name="input_subnet_cidr_bits"></a> [subnet\_cidr\_bits](#input\_subnet\_cidr\_bits) | The number of subnet bits for the CIDR. For example, specifying a value 8 for this parameter will create a CIDR with a mask of /24. | `number` | `8` | no |
| <a name="input_vpc_cidr"></a> [vpc\_cidr](#input\_vpc\_cidr) | The CIDR block for the VPC. Default value is a valid CIDR, but not acceptable by AWS and should be overridden | `string` | `"10.0.0.0/16"` | no |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_private_cidrs"></a> [private\_cidrs](#output\_private\_cidrs) | The IPv4 CIDR blocks for the private subnets. |
| <a name="output_private_ids"></a> [private\_ids](#output\_private\_ids) | The IDs of the private subnets |
| <a name="output_public_cidrs"></a> [public\_cidrs](#output\_public\_cidrs) | The IPv4 CIDR blocks for the public subnets. |
| <a name="output_public_ids"></a> [public\_ids](#output\_public\_ids) | The IDs of the public subnets |
| <a name="output_vpc_id"></a> [vpc\_id](#output\_vpc\_id) | The ID of the VPC |
