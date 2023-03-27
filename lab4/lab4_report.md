University: ITMO University Faculty: FICT Course: IP-telephony Year: 2022/2023 Group: K34202 Author: Konstantinova Iuliia Vyacheslavovna Lab: Lab3 Date of create: 27.03.2023 Date of finished:

Цель: изучить построение сети IP-телефонии между удаленными филиалами с помощью маршрутизаторов Cisco 2811 и коммутаторов Cisco 2950Т.

Ход работы:
Часть 1

В начале работы собрана схема соединения, представленная в задании (Рис.1). Далее были настроены интерфейсы fa0/0 (Рис.2), s1/0 (Рис.3) на маршрутизаторах Cisco 2811. Настроены маршрутизатор Cisco 2811, коммутатор Cisco 2950Т (Рис.4), IP-телефоны аналогично лабораторной работе №1. Командой switchport mode access сконфигурированы выбранные порты коммутатора, как порты доступа (access порт). Командой switchport access vlan 1 указано, что данные порты являются портами доступа для vlan с номером 1.
 Также настроены DHCP сервера на маршрутизаторах для передачи голоса и данных между ними (Рис.5).
 
 ![image](https://user-images.githubusercontent.com/90499135/227979130-238d1f2c-1231-477d-aa78-c1cf8d63f8aa.png)

Рисунок 1 – Схема соединения
 
 ![image](https://user-images.githubusercontent.com/90499135/227979265-26c61309-9e28-46e1-ae4d-3ca393acf75b.png)

Рисунок 2 – Настройка интерфейса fa0/0
 
 ![image](https://user-images.githubusercontent.com/90499135/227979306-0eed9d99-9366-4fc6-9648-88fc024102a2.png)

Рисунок 3 – Настройка интерфейса s1/0
 
 ![image](https://user-images.githubusercontent.com/90499135/227979341-0d2274cd-c182-4eeb-8298-bfca64585d03.png)

Рисунок 4 – Настройка коммутатора 

 ![image](https://user-images.githubusercontent.com/90499135/227979374-d7ed694c-2ce0-4a69-8a28-5a5cd7215d21.png)

Рисунок 5 – Настройка DHCP серверов

После этого настроена динамическая маршрутизация RIP между маршрутизаторами для передачи информации друг другу (Рис.6). Настроены услуги телефонии Cisco CallManager Express на маршрутизаторах 2811 (Рис.7), заданы номера ip-телефонов (Рис.8).
 
 ![image](https://user-images.githubusercontent.com/90499135/227979445-c304cb55-f044-49e9-acd4-51f4c17bde3b.png)

Рисунок 6 – Настройка RIP
 
 ![image](https://user-images.githubusercontent.com/90499135/227979510-3eb804bf-4613-4c22-9ad5-bc7fe05fcd83.png)

Рисунок 7 – Настройка услуг телефонии
 
 ![image](https://user-images.githubusercontent.com/90499135/227979562-8bc1acb6-f6f5-4f2e-9205-1bdb0c2874b9.png)

Рисунок 8 – Настройка ip-телефонов

Затем настроены параметры dial-peer voice (Рис.9). Эта функция позволяет в конфигурации входящего dial-peer указать группу исходящих dial-peer как цель маршрутизации входящего звонка.
 
 ![image](https://user-images.githubusercontent.com/90499135/227979638-6e80656a-4b06-4711-8938-6d0dad69351a.png)

Рисунок 9 – Настройка dial-peer voice

В завершении работы проверены вызовы между удаленными IP-телефонами (Рис.10-13) и связь между компьютерами (Рис.14).
 
 ![image](https://user-images.githubusercontent.com/90499135/227979692-12037e38-ca2b-42a9-b4a3-975ef41cbfa7.png)

Рисунок 10 – Звонок внутри сети RouterA
 
 ![image](https://user-images.githubusercontent.com/90499135/227979735-059892ee-6b4f-490a-b2cc-c103c629053f.png)

Рисунок 11 – Звонок внутри сети RouterВ
 
 ![image](https://user-images.githubusercontent.com/90499135/227979767-6524c8b6-8082-411f-b74a-cfdfca8cd0aa.png)

Рисунок 12 – Исходящий вызов из одной сети в другую
 
 ![image](https://user-images.githubusercontent.com/90499135/227979822-9af2b6ca-d4a2-4a35-99c4-b7bc73ff6e45.png)

Рисунок 13 – Входящий вызов из другой сети

 ![image](https://user-images.githubusercontent.com/90499135/228002668-a34defe7-938e-4ac2-9695-d56348f7511c.png)

Рисунок 14 – Проверка связи ПК

Вывод: в результате выполнения работы все задачи выполнены. Изучено построение сети IP-телефонии между удаленными филиалами с помощью маршрутизаторов Cisco 2811 и коммутаторов Cisco 2950Т, а также смоделирована функционирующая VoIP-сеть.
