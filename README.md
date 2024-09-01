# **Домашнее задание к занятию «Disaster recovery и Keepalived» SYS-32 - Кумышев Аслан**

# * Задание 1 *
Что нужно сделать:

* Дана схема для Cisco Packet Tracer, рассматриваемая в лекции.
* На данной схеме уже настроено отслеживание интерфейсов маршрутизаторов Gi0/1 (для нулевой группы)
* Необходимо аналогично настроить отслеживание состояния интерфейсов Gi0/0 (для первой группы).
* Для проверки корректности настройки, разорвите один из кабелей между одним из маршрутизаторов и Switch0 и запустите ping между PC0 и Server0.
* На проверку отправьте получившуюся схему в формате pkt и скриншот, где виден процесс настройки маршрутизатора..

  [🛠️Файл Схемы pkt](https://github.com/sAslank/Disas-ter-recovery-Keepalived/blob/main/file/hsrp_advanced.pkt)



1. ![alt text](https://github.com/sAslank/Disas-ter-recovery-Keepalived/blob/main/img/11.jpg)
2. ![alt text](https://github.com/sAslank/Disas-ter-recovery-Keepalived/blob/main/img/22.jpg)
3. ![alt text](https://github.com/sAslank/Disas-ter-recovery-Keepalived/blob/main/img/33.jpg)

 **************************************************************************

# * Задание 2 *
Что нужно сделать:
* Запустите две виртуальные машины Linux, установите и настройте сервис Keepalived как в лекции, используя пример конфигурационного файла.
* Настройте любой веб-сервер (например, nginx или simple python server) на двух виртуальных машинах
* Напишите Bash-скрипт, который будет проверять доступность порта данного веб-сервера и существование файла index.html в root-директории данного веб-сервера.
* Настройте Keepalived так, чтобы он запускал данный скрипт каждые 3 секунды и переносил виртуальный IP на другой сервер, если bash-скрипт завершался с кодом, отличным от нуля (то есть порт веб-сервера был недоступен или отсутствовал index.html). Используйте для этого 
  секцию vrrp_script
* На проверку отправьте получившейся bash-скрипт и конфигурационный файл keepalived, а также скриншот с демонстрацией переезда плавающего ip на другой сервер в случае недоступности порта или файла index.html

[🛠️Файл Keepalived.conf](https://github.com/sAslank/Disas-ter-recovery-Keepalived/blob/main/file/Keepalived.conf.txt)

[🛠️Файл bash-script.sh](https://github.com/sAslank/Disas-ter-recovery-Keepalived/blob/main/file/script.txt)

1. ![alt text](https://github.com/sAslank/Disas-ter-recovery-Keepalived/blob/main/img/2.jpg)
2. ![alt text](https://github.com/sAslank/Disas-ter-recovery-Keepalived/blob/main/img/3.jpg)
3. ![alt text](https://github.com/sAslank/Disas-ter-recovery-Keepalived/blob/main/img/4.jpg)
4. ![alt text](https://github.com/sAslank/Disas-ter-recovery-Keepalived/blob/main/img/5.jpg)
5. ![alt text](https://github.com/sAslank/Disas-ter-recovery-Keepalived/blob/main/img/6.jpg)
