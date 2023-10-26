# Demo2024
##1.
**Цель задания:**
1. Выполните базовую настройку всех устройств:  
	a. Соберите топологию согласно рисунку. Все устройства работают на OC Linux - Debian  
  b. Присвоить имена в соответствии с топологией  
  c. Рассчитайте IP-адресацию IPv4 и IPv6. Необходимо заполнить таблицу №1. При необходимости отредактируйте таблицу.  
  d. Пул адресов для сети офиса BRANCH - не более 16. Для IPv6 пропустите этот пункт.  
  e. Пул адресов для сети офиса HQ - не более 64. Для IPv6 пропустите этот пункт.  

![image](https://github.com/MurzabaevSSA39/Demo2024--1/assets/148869306/a7346d78-d13c-4cf2-8e87-4939f1a03497)



| Имя устройства |    Интерфейс   |  Pv4/IPv6      |  Маска/Префикс     |   Шлюз         |
| -----------    | -----------    |-------------   | -----------        | -------------- |
| ISP            |      ens192    |  10.12.24.10   |/24                 |10.12.24.254    |
|                |      ens224    |192.168.0.162   |/30                 |                |
|                |      ens256    |192.168.0.166   |/30                 |                |
| HQ-R           |      ens192    |192.168.0.161   | /30                |192.168.0.162   |
|                |      ens224    | 192.168.0.1    | /25                |                |  
| BR-R           |      ens192    |192.168.0.165   | /30                |192.168.0.166   |
|                |      ens224    |192.168.0.129   | /27                |                |
| HQ-SRV         |      ens192    |192.168.0.126   | /25                |   192.168.0.1  |
| BR-SRV         |     	ens192    |192.168.0.158   | /27                |  192.168.0.129 |
