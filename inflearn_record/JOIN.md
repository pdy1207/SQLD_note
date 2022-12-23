## 관계형 데이터베이스의 꽃 JOIN


      mysql> SELECT * FROM topic LEFT JOIN author ON topic.author_id = author.id;
      +----+---------+---------------+---------------------+-----------+------+---------+-----------+
      | id | title   | description   | created             | author_id | id   | name    | profile   |
      +----+---------+---------------+---------------------+-----------+------+---------+-----------+
      | 11 | Mysql   | Mysql is..    | 2022-12-21 14:04:17 |         1 |    1 | pdy1207 | developer |
      | 12 | Oracle  | Oracle is...  | 2022-12-21 14:04:32 |         1 |    1 | pdy1207 | developer |
      | 14 | MongoDB | MongoDB is... | 2022-12-21 14:04:55 |         3 | NULL | NULL    | NULL      |
      | 17 | test3   | test4         | 2022-12-22 14:15:52 |         1 |    1 | pdy1207 | developer |
      | 18 |         |               | 2022-12-22 14:17:43 |         1 |    1 | pdy1207 | developer |
      | 20 | ORACLE  | ORACLE is...  | 2022-12-23 10:54:08 |         5 | NULL | NULL    | NULL      |
      +----+---------+---------------+---------------------+-----------+------+---------+-----------+
      
###  LEFT / RIGHT ???   
