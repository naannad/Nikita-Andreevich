## Описание работы :point_down: ## 
+ установка и настройка ПО обеспечивается ansible, 
+ установка nginx на виртуальные машины web1 и web2,
+ на серверах haproxy1, haproxy2 установить и настроить отказоустойчивую связку HAProxy+Keepalived,
+ настроить VIP,
+ на серверах с HAProxy ПО должно обеспечить балансировку нагрузки серверов web1 и web2 в режиме round-robin,
+ кастомные страницы помогают понять, на каком сервере мы находимся.
 
 ## Установка ##
 + запуск виртуальных машин с вагрантом
 ~~~ 
 vagrant up 
 ~~~
 + запуск playbook
 ~~~
 ansible-playbook sirius.yml
 ~~~
 + для вывода результата
 ~~~
 patronictl -c /opt/app/patroni/etc/postgresql.yml list
 ~~~
 
 ## Результат ##

![изображение](https://user-images.githubusercontent.com/113581587/232332188-a534b4d6-8398-4dd4-93bf-75eede06476f.png)
