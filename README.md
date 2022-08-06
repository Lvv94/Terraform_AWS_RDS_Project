envs:
virginia.tfvars: 
region                  = "us-east-1"
allocated_storage       = 20
engine                  = "mysql"
engine_version          = "8.0.28"
instance_class          = "db.r6gd.large"
db_name                 = "mydb"
name                    = "mydb"
username                = "foo"
publicly_accessible     = true
instance_tenancy        = "default"
enable_dns_host_names   = true
enable_dns_support      = true
#allowed_cidr_blocks     = "0.0.0.0/0"
allowed_security_groups = "default"
subnet_ids = [
  "subnet-0188b6c64bdf8af92", "subnet-0aab9c166f58508a8", "subnet-06fa1e22079eae502"
]
aws_db_subnet_group_name = "project_sg"
vpc_id                   = "vpc-08638f9ad2603d412"
vpc_security_group_id    = "sg-0e09bb4c415e17c65"