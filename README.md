## Домашнее задание к занятию «Уязвимости и атаки на информационные системы» "Воронин Владислав"


### Задание 1


Разрешены протоколы: ftp, ssh, telnet, http, smtp Удаленный рабочий стол (vns), БД на PostgreSQL, Apache (Tomcat, Jserv), MySQL, rshd, rsh (удаленная консоль), Samba

#### ProFTPD 1.3.1 
https://www.exploit-db.com/exploits/32798

Использование этой проблемы может позволить злоумышленнику манипулировать SQL-запросами, изменять данные или использовать скрытые уязвимости в базовой базе данных. Это может привести к несанкционированному доступу и компрометации приложения; также возможны другие атаки.

#### Apache Tomcat/Coyote JSP engine 1.1 
https://charlesreid1.com/wiki/Metasploitable/Apache/Tomcat_and_Coyote

При применении эксплоита можно подключиться к оболочке tomcat. По ссылке пример взлома метасплоидетом.

#### Samba smbd 3.X 
https://www.exploit-db.com/exploits/37834

Samba подвержена неуказанной уязвимости удаленного выполнения кода. Злоумышленник может воспользоваться этой проблемой для выполнения произвольного кода с правами root.


### Задание 2

**Режимы сканирования в Metasploitable**

1.  **SYN (Synchronize):**  
    *   В SYN-пакете нет данных, а только синхронизирующий флаг. 
    *   Сетевой трафик: SYN-пакет -> SYN-ACK.
    *   Metasploitable отвечает: SYN-ACK
2.  **FIN (Finish):**  
    *   FIN-пакет - это конечный пакет TCP, который указывает на завершение соединения. 
    *   Сетевой трафик: FIN-пакет -> ACK (сервисом может ответить RST или ACK).
    *   Metasploitable отвечает: ACK
3.  **Xmas (Christmas):**  
    *   Xmas-режим включает в себя несколько флагов, что делает его более заметным для некоторых IDS и IPS систем. 
    *   Сетевой трафик: SYN+URG+ACK-FIN-пакеты -> RST.
    *   Metasploitable отвечает: RST
4.  **UDP (User Datagram Protocol):**  
    *   UDP - это соединение-less протокол, который не требует установления соединения. 
    *   Сетевой трафик: UDP-датаграмма -> ICMP-"destination unreachable".
    *   Metasploitable отвечает: ICMP-"destination unreachable"
