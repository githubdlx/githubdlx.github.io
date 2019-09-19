# 1.主键与联合主键
主键非空
联合主键shift多选
# 2.外键
设置外键的前提：该外键是某个表的主键
![图片](https://uploader.shimo.im/f/Jq5zmSo438sVH8Cj.png!thumbnail)
现在需要将sno cno关联student和course两张表



![图片](https://uploader.shimo.im/f/nNe5Qeg1ObYxhXTk.png!thumbnail)
选择表和列规范

每一个外键单独设置：
![图片](https://uploader.shimo.im/f/6pWvckaV98Mkj9oV.png!thumbnail)


设置好的关系图：![图片](https://uploader.shimo.im/f/wynnH3gQfCMjPgC9.png!thumbnail)
# 2.增加操作
insert into  表名 values（字段1，字段2，...）
还可以excel导入，需要映射字段
# 3.删除操作
3.3.1使用DROP INDEX命令删除表格中的索引
DROP INDEX table_name.index_name
3.3.2使用DROP TABLE 语句用于删除表（表的结构、属性以及索引也会被删除）：
DROP TABLE 表名称
3.3.3使用DROP DATABASE 语句用于删除数据库：
DROP DATABASE 数据库名称
3.3.4如果我们仅仅需要除去表内的数据，但并不删除表本身，那么我们该使用TRUNCATE TABLE命令（仅仅删除表格中的数据）：
TRUNCATE TABLE 表名称
# 4.修改操作
修改单个值
UPDATE 表名称 SET 列名称 = 新值 WHERE 列名称 = 某值
修改多个值（用逗号隔开）
update student set ssex = '男', sdept = '文学院'
where sno = '0007'
# 5.查询操作
最基本的SQL查询语句语法如下：
SELECT <table fields list>
FROM <table names list>
WHERE <row constraints specification>
GROUP BY <grouping specification>
HAVING <grouping selection specification>
ORDER BY <order rules specification>
Tips & Tricks:
1、Select...From... 语句是必须的。
2、Where, group by 以及 order by 三个语句不是必须的。
3.[select...from...](https://www.cnblogs.com/PyLearn/p/7642236.html#jump3)
* 3.1 [“*”与“Top num *”](https://www.cnblogs.com/PyLearn/p/7642236.html#jump3.1)
* 3.2 [查询指定列](https://www.cnblogs.com/PyLearn/p/7642236.html#jump3.2)
* 3.3 [Isnull函数：判断空值](https://www.cnblogs.com/PyLearn/p/7642236.html#jump3.3)
* 3.4 [使用"+"将"列"与"字符串"连接起来（使用as重命名）](https://www.cnblogs.com/PyLearn/p/7642236.html#jump3.4)

4.[order by](https://www.cnblogs.com/PyLearn/p/7642236.html#jump4)
* 4.1 [asc（正序）](https://www.cnblogs.com/PyLearn/p/7642236.html#jump4.1)
* 4.2 [desc（倒序）](https://www.cnblogs.com/PyLearn/p/7642236.html#jump4.2)
* 4.3 [其他](https://www.cnblogs.com/PyLearn/p/7642236.html#jump4.3)

5.[where](https://www.cnblogs.com/PyLearn/p/7642236.html#jump5)
* 5.1 [比较运算符](https://www.cnblogs.com/PyLearn/p/7642236.html#jump5.1)
* 5.2 [or 或 and](https://www.cnblogs.com/PyLearn/p/7642236.html#jump5.2)
* 5.3 [Like "%" 或 "_" 通配符](https://www.cnblogs.com/PyLearn/p/7642236.html#jump5.3)
* 5.4 [in 或 not in](https://www.cnblogs.com/PyLearn/p/7642236.html#jump5.4)
* 5.5 [is null 或 is not null](https://www.cnblogs.com/PyLearn/p/7642236.html#jump5.5)
* 5.6 [between...and...](https://www.cnblogs.com/PyLearn/p/7642236.html#jump5.6)

6.[group by & having](https://www.cnblogs.com/PyLearn/p/7642236.html#jump6)
* 6.1 [常用的聚合函数&经典查询语句](https://www.cnblogs.com/PyLearn/p/7642236.html#jump6.1)
* 6.2 [count](https://www.cnblogs.com/PyLearn/p/7642236.html#jump6.2)
* 6.3 [Avg、Min、Max、Sum](https://www.cnblogs.com/PyLearn/p/7642236.html#jump6.3)
* 6.4 [group by & having 的作用](https://www.cnblogs.com/PyLearn/p/7642236.html#jump6.4)
# 6.JDBC连接sql server











