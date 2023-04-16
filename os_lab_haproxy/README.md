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
 ansible-playbook nginx.yml
 ~~~
 
 ## Проверка ##
работа балансировщика:

![изображение](https://user-images.githubusercontent.com/113581587/232329496-6e1ef7b8-6498-49d2-abf9-d8c62e67e5d8.png)

![изображение](https://user-images.githubusercontent.com/113581587/232329460-aeee7fc5-2a5e-403a-8901-dcd5d007bf89.png)
