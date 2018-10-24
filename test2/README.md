# 实验2：用户管理 - 掌握管理角色、权根、用户的能力，并在用户之间共享对象。
## 第一步：以system登录到pdborcl，创建角色con_res_DMQ和用户new_DMQQ，并授权和分配空间
## 代码：
``` •	$ sqlplus system/123@pdborcl
•	SQL> CREATE ROLE con_res_DMQ;
•	Role created.
•	SQL> GRANT connect,resource,CREATE VIEW TO con_res_view;
•	Grant succeeded.
•	SQL> CREATE USER new_DMQQ IDENTIFIED BY 123 DEFAULT TABLESPACE users TEMPORARY TABLESPACE temp;
•	User created.
•	SQL> ALTER USER new_DMQQ QUOTA 50M ON users;
•	User altered.
•	SQL> GRANT con_res_DMQ TO new_DMQQ;
•	Grant succeeded.
•	SQL> exit
```
