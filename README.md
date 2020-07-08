## Terraform-version-manage
# A way to manage Terraform version via docker-compose

Terraform version does not support each other completely. If you develop infrastructure with a number of developers and use version 2, then wrongly use version 3, Terraform Cloud will be directly upgraded the last version from 2 to 3. As a result of this upgrade, Terraform Cloud will be broken for the people who uses version 2. 

A way to manage Terraform Version is that running terraform image via docker-compose and docker. Check it out the script below! 

I got insprired from different Youtube videos and Open Source works on terraform to create this repo. There is no any license. You can just adopt this scrips if you would like to. 