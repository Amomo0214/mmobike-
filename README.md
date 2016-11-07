# mmobike-

-- 最近,魔拜单车火遍了微信朋友圈，也火遍了帝都街头。假如你是「魔拜单车」公司的
-- 架构师，请设计 MySQL 风格的数据表结构，满足以下场景：
-- 1. 用户的基本信息；
 create table Users(
uid varchar(20),
uname varchar(30),
usex  varchar(30),
uaddress varchar(20)
)

-- 2. 用户使用微信登录；
 create table weixin(
wphone varchar(20),
wuname varchar(30),
wusex  varchar(30),
wuaddress varchar(20)
)

-- 3. 用户使用邮箱登录；
 create table mail(
mphone varchar(20),
muname varchar(30),
musex  varchar(30),
muaddress varchar(20)
)
-- 4. 用户使用手机号登录；
 create table Tphone(
phone varchar(20),
name varchar(30),
sex  varchar(30),
address varchar(20)
)
-- 5. 单车的基本信息；
 create table mobike(
mid varchar(20),
mlocation varchar(30),
mstate  varchar(30)
)
-- 6. 用户充值记录；
 create table recharge(
uid varchar(20),
rje varchar(30),--充值金额
rtime  varchar(30),--充值时间
rye varchar(20) --余额
)
-- 7. 用户骑行记录；
 create table cycling(
ctime varchar(20),
clength varchar(30),  --骑行距离
)
-- 8. 单车每天的 GPS 位置记录。
 create table Gps(
uid varchar(20),
mlocation varchar(30),
)
