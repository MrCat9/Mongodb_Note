# Mongodb_Note

## 复制数据库

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
