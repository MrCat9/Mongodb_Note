# Mongodb_Note

1_复制数据库

```
mongodb 复制集合与数据库的方式
https://blog.csdn.net/yisun123456/article/details/78646774
```

```
示例：
192.168.11.51 mongod实例mydb库，
复制到本地newmydb库：
db.copyDatabase("mydb", "newmydb", "192.168.11.52");
```

2_mongoDB删除表中一个字段

```
https://www.cnblogs.com/zdfjf/p/6179691.html
```

例如要把User表中address字段删除
```
db.User.update({},{$unset:{'address':''}},false, true)
```

