## 관계형 데이터베이스의 꽃 JOIN <br> -[JOIN 강의](https://opentutorials.org/course/3884/25179)

### 예시 (JOIN에 의미부여 해봅시다.)

      mysql> SELECT * FROM topic LEFT JOIN author ON topic.author_id = author.id; //전체 다 뽑기
      
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
      
      mysql> SELECT topic.id,title,description,created,name,profile FROM topic LEFT JOIN author ON topic.author_id = author.id; //topic.id and join
      
      +----+---------+---------------+---------------------+---------+-----------+
      | id | title   | description   | created             | name    | profile   |
      +----+---------+---------------+---------------------+---------+-----------+
      | 11 | Mysql   | Mysql is..    | 2022-12-21 14:04:17 | pdy1207 | developer |
      | 12 | Oracle  | Oracle is...  | 2022-12-21 14:04:32 | pdy1207 | developer |
      | 14 | MongoDB | MongoDB is... | 2022-12-21 14:04:55 | NULL    | NULL      |
      | 17 | test3   | test4         | 2022-12-22 14:15:52 | pdy1207 | developer |
      | 18 |         |               | 2022-12-22 14:17:43 | pdy1207 | developer |
      | 20 | ORACLE  | ORACLE is...  | 2022-12-23 10:54:08 | NULL    | NULL      |
      +----+---------+---------------+---------------------+---------+-----------+
      6 rows in set (0.00 sec)

      mysql> SELECT topic.id AS topic_id ,title,description,created,name,profile FROM topic LEFT JOIN author ON topic.author_id = author.id; // AS 사용
      
      +----------+---------+---------------+---------------------+---------+-----------+
      | topic_id | title   | description   | created             | name    | profile   |
      +----------+---------+---------------+---------------------+---------+-----------+
      |       11 | Mysql   | Mysql is..    | 2022-12-21 14:04:17 | pdy1207 | developer |
      |       12 | Oracle  | Oracle is...  | 2022-12-21 14:04:32 | pdy1207 | developer |
      |       14 | MongoDB | MongoDB is... | 2022-12-21 14:04:55 | NULL    | NULL      |
      |       17 | test3   | test4         | 2022-12-22 14:15:52 | pdy1207 | developer |
      |       18 |         |               | 2022-12-22 14:17:43 | pdy1207 | developer |
      |       20 | ORACLE  | ORACLE is...  | 2022-12-23 10:54:08 | NULL    | NULL      |
      +----------+---------+---------------+---------------------+---------+-----------+
      6 rows in set (0.00 sec)


###  LEFT / RIGHT / inner ???   

<p align="center">
  <img src="https://user-images.githubusercontent.com/110442250/209277645-5e91c84d-38c6-4955-90d5-b948dd7ef6d2.jpg" height="400">

</p>
