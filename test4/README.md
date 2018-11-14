# 实验4：对象管理
## 一、表的创建
## （1）CREATE TABLE DEPARTMENTS
![](./1.png)
![](./2.png)
## （2）CREATE TABLE EMPLOYEES
![](./3.png)
![](./4.png)
## 创建索引
![](./5.png)
## 创建外键
![](./6.png)
![](./7.png)
## CREATE TABLE PRODUCTS
![](./12.png)
![](./13.png)
## CREATE GLOBAL TEMPORARY TABLE "ORDER_ID_TEMP"
![](./15.png)
## CREATE TABLE ORDERS
![](./17.png)
![](./18.png)
## 创建索引
![](./18-1.png)
## 创建主键和外键
```
ALTER TABLE ORDERS
ADD CONSTRAINT ORDERS_PK PRIMARY KEY
(
  ORDER_ID
)
USING INDEX ORDERS_PK
ENABLE;
```
```
ALTER TABLE ORDERS
ADD CONSTRAINT ORDERS_FK1 FOREIGN KEY
(
  EMPLOYEE_ID
)
REFERENCES EMPLOYEES
(
  EMPLOYEE_ID
)
ENABLE;
```
![](./23.png)
![](./24.png)
## CREATE TABLE ORDER_DETAILS
![](./25.png)
![](./26.png)
## 二、创建触发器
![](./31.png)
![](./32.png)

## 三、录入数据
## 插入DEPARTMENTS，EMPLOYEES数据
![](./41.png)
![](./42.png)
![](./43.png)
![](./44.png)
![](./45.png)
![](./46.png)
![](./47.png)
![](./48.png)
![](./49.png)
![](./50.png)
![](./51.png)
![](./52.png)
## 四、查询数据
## 递归查询某个员工及其所有下属，子下属员工
![](./56.png)
![](./57.png)
## 查询一个分区中的数据
![](./58.png)


