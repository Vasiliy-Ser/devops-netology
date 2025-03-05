# devops-netology  
Student Падеев Василий  
Fops-27  

Игнорироваться будут следующий файлы:  
1. Файлы в дирректории terraform расположенный в рабочем проекте  git   
**/.terraform/*  
2. Файлы содержащие информация о ресурсах развернутых облаке с люмым именем и расширением .tfstate или файлы с любым именем и двойным расширением в которых присутствует .tfstate.  
*.tfstate  
*.tfstate.*   
3. Конфиденциальные данные с любым именем и расширением tfvars и tfvars.json  
*.tfvars  
*.tfvars.json  
4. Файлы переопределения которые называются или заканчиваются на override.tf или override.tf.json  
override.tf  
override.tf.json  
*_override.tf  
*_override.tf.json  
5. Файлы журнала сбоев crash.log, в том числе имя которых начинаются на crash и заканчиваются расширением log   
crash.log  
crash.*.log  
6. Скрытый файл информации о временной блокировке  
.terraform.tfstate.lock.info  
7. Можно добавить Игнорировать вывод плана команды: terraform plan -out=tfplan содержащую в названии файла tfplan  
 # example: *tfplan*  
8. Файл конфигурации CLI terraform.rc и скрытый файл .terraformrc  
.terraformrc  
terraform.rc  
9. Можно добавить файл переопределения используя скрытый шаблон. Сейчас он отключен.  
 # !example_override.tf      
