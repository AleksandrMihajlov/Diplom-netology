# Diplom-netology
Дипломная работа по профессии «Системный администратор» - Aleksandr Mihajlov SYS34

## Задача

Ключевая задача — разработать отказоустойчивую инфраструктуру для сайта, включающую мониторинг, сбор логов и резервное копирование основных данных. 
Инфраструктура должна размещаться в [Yandex Cloud](https://cloud.yandex.com/) и отвечать минимальным стандартам безопасности: запрещается выкладывать токен от облака в git. 
Используйте [инструкцию](https://cloud.yandex.ru/docs/tutorials/infrastructure-management/terraform-quickstart#get-credentials).



# Начало работы  



## Инфраструктура  

Для развертки использовался Terraform  
![alt text](https://github.com/AleksandrMihajlov/Diplom-netology/blob/main/Screen/1.png)  
Созданы 6 виртуальных машин
![alt text](https://github.com/AleksandrMihajlov/Diplom-netology/blob/main/Screen/2.png)  
Созданы снимки дисков и расписание  
![alt text](https://github.com/AleksandrMihajlov/Diplom-netology/blob/main/Screen/3.png)  
Создана главная сеть и 4 подсети  
![alt text](https://github.com/AleksandrMihajlov/Diplom-netology/blob/main/Screen/4.png)  
Создана группа безопасности  
![alt text](https://github.com/AleksandrMihajlov/Diplom-netology/blob/main/Screen/5.png)  
Карта сети  
![alt text](https://github.com/AleksandrMihajlov/Diplom-netology/blob/main/Screen/6.png)  
Создан балансировщик  
![alt text](https://github.com/AleksandrMihajlov/Diplom-netology/blob/main/Screen/7.png)  
![alt text](https://github.com/AleksandrMihajlov/Diplom-netology/blob/main/Screen/8.png)  
  
Время развертывания занимает около 10 минут  
  
## Сервисы  
  
  
### Сайт  

Запуск Nginx "заглушка" с адресом http://158.160.148.69
![alt text](https://github.com/AleksandrMihajlov/Diplom-netology/blob/main/Screen/2.2.png)  
Выполняем curl -v 158.160.148.69:80
![alt text](https://github.com/AleksandrMihajlov/Diplom-netology/blob/main/Screen/2.1.png)  
  
### Мониторинг  
  
Запуск Zabbix c адресом http://89.169.145.182  
Добавлены дашборты для VM WEB  
![alt text]()  
  
### Логи

Запуск Elasticsearch c адресом http://158.160.54.232:5601  
![alt text]()