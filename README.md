# Diplom-netology
Дипломная работа по профессии «Системный администратор» - Aleksandr Mihajlov SYS34

## Задача

Ключевая задача — разработать отказоустойчивую инфраструктуру для сайта, включающую мониторинг, сбор логов и резервное копирование основных данных. 
Инфраструктура должна размещаться в [Yandex Cloud](https://cloud.yandex.com/) и отвечать минимальным стандартам безопасности: запрещается выкладывать токен от облака в git. 
Используйте [инструкцию](https://cloud.yandex.ru/docs/tutorials/infrastructure-management/terraform-quickstart#get-credentials).



# Начало работы.  



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
![alt text](https://github.com/Roman-Teterevlev/SYS-19_diploma/blob/main/README.md)  
Карта сети  
![alt text](https://github.com/AleksandrMihajlov/Diplom-netology/blob/main/Screen/6.png)  
Создан балансировщик  
![alt text](https://github.com/AleksandrMihajlov/Diplom-netology/blob/main/Screen/7.png)  
![alt text](https://github.com/AleksandrMihajlov/Diplom-netology/blob/main/Screen/8.png)
