# Terraform
About Terraform

Structure explained
.
├── README.md
├── dev.tfvar
├── dev.tfvar.template
├── main.tf
├── modules
│   ├── resource_group
│   │   ├── main.tf
│   │   ├── outputs.tf
│   │   └── vars.tf
│   ├── storage_account
│   │   ├── main.tf
│   │   ├── outputs.tf
│   │   └── vars.tf
│   ├── virtual_machine
│   │   ├── main.tf
│   │   └── vars.tf
│   └── virtual_network
│       ├── main.tf
│       ├── outputs.tf
│       └── vars.tf
├── terraform.tfstate
├── terraform.tfstate.backup
└── variables.tf
main.tf modules instantiation.
variables.tf variables declaration.
dev.tfvar.template template for dev.tfvar with empty values.
dev.tfvar values for vars in variables.tf. Donot share this file as it can contain sensitive information.
modules/ each repo inside modules/ can be instantiated as a Terraform module.
main.tf module resources
vars.tf variables declaration
outputs.tf define outputs. Module outputs can be used in other resources.
