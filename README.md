AWS Tested OSes
============
This module returns for an given OS the AMI aswell as its default user and the prerequisits script


EXAMPLE
-------
```hcl
module "dcos-tested-oses" {
  source  = "terraform-dcos/tested-oses/aws"
  version = "~> 0.1"
}
```


## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|:----:|:-----:|:-----:|
| aws_ami | Map of system and region combinations to their AMI ID | map | `<map>` | no |
| aws_default_os_user | Map a system to its default users | map | `<map>` | no |
| os | Operating system to use | string | `centos_7.4` | no |
| provider | Provider to use | string | `aws` | no |
| region | Region to use. If not specify AWS current region is used. | string | `` | no |

## Outputs

| Name | Description |
|------|-------------|
| aws_ami |  |
| os-setup |  |
| user |  |

