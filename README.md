# Terraform init

This init will create a basic VPC setup

- VPC
- 3 Private Subnets
- 3 Public Subnets
- 3 External IP
- Nat gateways for external traffic


# Docker
Please run terraform in docker and pin version no version is pinned at this point.

# Access
To access the AWS terraform need AWS access key and secret.
Add them into the docker-compose.yaml file.

```
    environment:
      AWS_ACCESS_KEY_ID:  your key id here
      AWS_SECRET_ACCESS_KEY:  your key secret here
    
```




# How to


## Build image
```
 docker compose build
```

## Start 


```
docker compose run terraform sh
```

## Init terraform

Change folder to /code and run terraform init


```
terraform init
```


## Plan 
This will show the changes that will be applied


```
terraform plan
```


## Apply and destroy 

```
terraform apply
```


```
terraform destroy
```



# Local dev
To dev local add and update files in the /code folder. then run terraform plan inside the docker to test your changes.


