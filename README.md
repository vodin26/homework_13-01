## Домашнее задание к занятию «Уязвимости и атаки на информационные системы» "Воронин Владислав"


### Задание 1


Разрешены протоколы: ftp, ssh, telnet, http, smtp Удаленный рабочий стол (vns), БД на PostgreSQL, Apache (Tomcat, Jserv), MySQL, rshd, rsh (удаленная консоль), Samba

ProFTPD 1.3.1 
[https://www.exploit-db.com/exploits/32798](https://www.exploit-db.com/exploits/32798) 
Использование этой проблемы может позволить злоумышленнику манипулировать SQL-запросами, изменять данные или использовать скрытые уязвимости в базовой базе данных. Это может привести к несанкционированному доступу и компрометации приложения; также возможны другие атаки.

Apache Tomcat/Coyote JSP engine 1.1 [https://charlesreid1.com/wiki/Metasploitable/Apache/Tomcat_and_Coyote](https://charlesreid1.com/wiki/Metasploitable/Apache/Tomcat_and_Coyote)
При применении эксплоита можно подключиться к оболочке tomcat. По ссылке пример взлома метасплоидетом.

Samba smbd 3.X 
[https://www.exploit-db.com/exploits/37834](https://www.exploit-db.com/exploits/37834) 
Samba подвержена неуказанной уязвимости удаленного выполнения кода. Злоумышленник может воспользоваться этой проблемой для выполнения произвольного кода с правами root.

### Задание 2
