## Terraform-version-manage

A way to manage Terraform version via docker-compose

Terraform version does not support each other completely. If you develop infrastructure with a number of developers and use version 2, then wrongly use version 3, Terraform Cloud will be directly upgraded the last version from 2 to 3. As a result of this upgrade, Terraform Cloud will be broken for the people who uses version 2. 

A way to manage Terraform Version is that running terraform image via docker-compose and docker.  

# Running docker-compose

1. docker-compose run --rm tf init
2. docker-compose run --rm tf fmt
3. docker-compose run --rm tf validate 
// Note: If you get the result is => Success! You configured everything successfully.
4. docker-compose run --tm tf plan 
// Warning! Do not commit anything /terraform folder to Github!
5. docker-compose run --tm tf apply  
// Then, you would get a confirmation message from terraform 
// Say; yes
6. The resources you described on main.tf would be provision on AWS.


I got insprired from different Youtube videos and Open Source works on terraform to create this repo. There is no any license. You can just adopt this scrips if you would like to. 