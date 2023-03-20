University: ITMO University
Faculty: FICT
Course: IP-telephony
Year: 2022/2023
Group: K34202
Author: Konstantinova Iuliia Vyacheslavovna
Lab: Lab2
Date of create: 16.03.2023
Date of finished:
Цель: изучить построение сети IP-телефонии с помощью маршрутизатора Cisco 2811, коммутатора Cisco 3560 и IP телефонов Cisco 7960.

Ход работы:

Часть 1

В начале работы собрана схема соединения, представленная в задании (Рис.1). Затем в конфигурационном режиме изменено название маршрутизатора на CMERouter. Также отключен синтаксис ввода слов от DNS серверов (Рис.2).
 
![image](https://user-images.githubusercontent.com/90499135/226295793-bd6d473b-bd78-45a9-afe7-977950ee45aa.png)

Рисунок 1 – Схема соединения
 
![image](https://user-images.githubusercontent.com/90499135/226295845-8cfce242-95d3-41b8-a954-c6c5cbf8c64e.png)

Рисунок 2 – Отключение поиска в системе DNS

Затем заданы пароли для защиты маршрутизатора как в удаленном режиме, так и в режиме консоли (Рис.3, 3.1). Настроен интерфейс fa0/0 на маршрутизаторе Cisco 2811 (CMERouter) (Рис.4). Также настроены DHCP сервера для передачи голоса и данных на маршрутизаторе Cisco 2811 (Рис.5). Настроены услуги телефонии Cisco CallManager Express на маршрутизаторе 2811 (Рис.6).
 
![image](https://user-images.githubusercontent.com/90499135/226295955-589ca457-a66a-4291-a82d-fd57aa549e33.png)

Рисунок 3 – Задание паролей для маршрутизатора

![image](https://user-images.githubusercontent.com/90499135/226296462-c72f9991-04f5-4886-893f-1a172e349a35.png)

Рисунок 3.1 – Ввод пароля
 
![image](https://user-images.githubusercontent.com/90499135/226296505-ce8ec520-f61c-4a3e-abc6-6f2c46d5eb37.png)

Рисунок 4 – Настройка интерфейса роутера
 
![image](https://user-images.githubusercontent.com/90499135/226296577-9bbba76a-496d-42bb-9b03-9bc5358f6ddd.png)

Рисунок 5 – Настройка DHCP серверов
 
![image](https://user-images.githubusercontent.com/90499135/226296612-e56ea139-9775-4c07-b0be-dd4179972350.png)

Рисунок 6 – Настройка услуг телефонии

После были созданы VLAN порты на коммутаторе Cisco Catalyst 3560 для взаимодействия коммутатора с маршрутизатором (Рис.7) и подключены IP телефоны (Рис.8). Настроены IP-телефоны и после они были соединены с коммутатором Cisco Catalyst 3560.
 
![image](https://user-images.githubusercontent.com/90499135/226296671-5de9bde7-ffec-433d-92f8-69059edb14cb.png)

Рисунок 7 – Создание VLAN портов
 
![image](https://user-images.githubusercontent.com/90499135/226296709-4bde5ff4-652c-44b0-9229-7f8f8fa9c60a.png)

Рисунок 8 – Подключение телефонов

В завершении были проверены звонки между телефонами (Рис.9,10).
 
![image](https://user-images.githubusercontent.com/90499135/226296769-d91ae38b-f601-4225-8cf7-d3866b0a0297.png)

Рисунок 9 – Исходящий звонок
 
![image](https://user-images.githubusercontent.com/90499135/226296797-d854e8e9-fb2f-4e48-92b4-23d0f3aa81a0.png)

Рисунок 10 – Принятый звонок

Часть 2

В начале работы собрана схема соединения, представленная в задании (Рис.11). Затем созданы VLAN порты на коммутаторе для взаимодействия коммутатора с маршрутизатором (Рис.12, 13) и подключены IP телефоны.
 
![image](https://user-images.githubusercontent.com/90499135/226296887-b28e3dcc-6cc5-4bab-a0d9-131d1cffc32f.png)

Рисунок 11 – Схема соединения
 
![image](https://user-images.githubusercontent.com/90499135/226296941-408177a5-67cd-4a39-874f-d531ff34c6eb.png)

Рисунок 12 – Создание VLAN портов
 
![image](https://user-images.githubusercontent.com/90499135/226296999-f753ebac-e595-4b84-8918-84c6816ecfcd.png)

Рисунок 13 – Настройка VLAN 99

Далее задан маршрут по умолчанию командой ip default-gateway (Рис.14). Настроен порт как канал типа trunk (Рис.15).
 
![image](https://user-images.githubusercontent.com/90499135/226297052-c048faf2-0bcc-41a5-9b33-7471f3170376.png)

Рисунок 14 – Задание маршрута по умолчанию
 
![image](https://user-images.githubusercontent.com/90499135/226297086-f47f5725-6528-4724-bd18-9c5befb4fdc3.png)

Рисунок 15 – Настройка порта

Затем настроены DHCP сервера для передачи голоса и данных на маршрутизаторе Cisco 2811 (Рис.16). Также настроены услуги телефонии Cisco CallManager Express на маршрутизаторе (Рис.17). Настроены и соединены с коммутатором IP-телефоны.
 
![image](https://user-images.githubusercontent.com/90499135/226297145-53c47273-c9a6-496b-895c-f09eef1c7003.png)

Рисунок 16 – Настройка DHCP серверов
 
![image](https://user-images.githubusercontent.com/90499135/226297180-84fe1768-6fc5-4e64-bfa2-476b88ba1f99.png)

Рисунок 17 – Настройка телефонии
Подключены конечные узлы устройств. В завершении работы проверены звонки между телефонами (Рис.18) и связь между компьютерами при помощи  пингования (Рис.19,20).
 
![image](https://user-images.githubusercontent.com/90499135/226297226-84dfe5a7-eb4b-4564-a903-6d61cc1b9e3c.png)

Рисунок 18 – И сходящий звонок
 
![image](https://user-images.githubusercontent.com/90499135/226297258-10c1a61f-b496-4f28-9467-160514c4c323.png)

Рисунок 19 – Принятый звонок
 
![image](https://user-images.githubusercontent.com/90499135/226297312-b0c6d935-d91c-446a-8e40-71eedcf74aec.png)

Рисунок 20 – Пинг с PC5 на PC3

![image](https://user-images.githubusercontent.com/90499135/226297365-0146f9d7-6dcc-4593-9ccf-ccd615041f70.png)

Рисунок 21 – Пинг с PC4 на PC5

Вывод: в ходе выполнения работы все задачи выполнены. Изучено построение сети IP-телефонии с помощью маршрутизатора Cisco 2811, коммутатора Cisco 3560 и IP телефонов Cisco 7960, а также смоделирована функционирующая VoIP-сеть.
