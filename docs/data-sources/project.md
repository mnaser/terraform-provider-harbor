# Data Source: harbor_project

## Example Usage
```hcl
data "haror_project" "main" {
    name    = "library" 
}

output "project_id" {
    value = data.harbor_project.main.id
}
```

## Argument Reference
The following arguments are supported:

* **name** - (Required) The of the project that will be created in harbor.

## Attributes Reference
In addition to all argument, the folloing attributes are exported:

* **project_id** - The id of the project within harbor.

* **public** - If the project will be public accessibility.

* **vulnerability_scanning** - If the images will be scanned for vulnerabilities when push to harbor.