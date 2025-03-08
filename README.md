# ACIT-4640-Lab9

First install packer and terraform on your machine with:  
https://developer.hashicorp.com/packer/tutorials/docker-get-started/get-started-install-cli  

Then generate an ssh key to be uploaded and used with:  
`ssh-keygen -t ed25519 -f </name/of/key>`

Run the script provided with the ssh key to upload to AWS assuming you already have AWS CLI configured on your machine


## Packer  

CD into the packer directory and initialize it with `packer init .` this uses both files so we could use the variable  

Check validation of the files with `packer validate .`  
Build packer `packer build .`  

## Terraform  

CD into the terraform directory and initialize it with `terraform init`  
Validate it `terraform validate`  
Apply the changes `terraform apply`  
Terraform will then prompt you to confirm the changes if you are happy enter `yes` 
After everything is finished and you are no longer using the infastructure clean up and use `terraform destroy`
