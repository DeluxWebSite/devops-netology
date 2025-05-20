# devops-netology

# line 1

### Игнорирование файлов и каталогов в gitignore 👍

- Local .terraform directories

.terraform/

- .tfstate files

_.tfstate
_.tfstate.\*

- Crash log files

crash.log
crash.\*.log

- Exclude all .tfvars files, which are likely to contain sensitive data, such as password, private keys and other secrets. These should not be part of version control as they are data points which are potentially sensitive and subject to change depending on the environment.

_.tfvars
_.tfvars.json

- Ignore override files as they are usually used to override resources locally and so are not checked in

override.tf
override.tf.json
_\_override.tf
_\_override.tf.json

- Ignore transient lock info files created by terraform apply

.terraform.tfstate.lock.info

- Include override files you do wish to add to version control using negated pattern !example*override.tf Include tfplan files to ignore the plan output of command: terraform plan -out=tfplan example: \_tfplan*

- Ignore CLI configuration files

.terraformrc
terraform.rc

---

![alt text](https://github.com/DeluxWebSite/devops-netology/blob/main/Снимок-экрана-2025-05-20-в-09.58.45.png)
![alt text](https://github.com/DeluxWebSite/devops-netology/blob/main/Снимок-экрана-2025-05-20-в-10.00.37.png)
![alt text](https://github.com/DeluxWebSite/devops-netology/blob/main/Снимок-экрана-2025-05-20-в-10.09.28.png)
