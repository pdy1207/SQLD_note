## SQL 순서 

      1. from 
      1-1 join 
      2. where 
      3. group by 
      4. having 
      5. select 
      6. order by


**아이디 및 비밀번호 확인 쿼리**

      $sql = "select * from 테이블명 where biz_corp='안녕' and biz_corpnumber='$pwd'";
      

**type은 간편이고 카테고리로부터 찾고자하는 사람의 변수와 같은사람을 찾을게 그리고 내림차순**


      $sql = "select * from 테이블명 where $catagory like '%$search_con%' and biz_type = '간편' 
                      order by 기준 desc";
                
**시간 개념**

      "select  * FROM 테이블명 WHERE biz_regtime BETWEEN '$date_to 00:00:00' AND '$date_from 23:59:59' 
                      ORDER BY 기준 DESC";
**시간으로서 간단한 삭제**

      delete  
                
                FROM 테이블명 
                WHERE time BETWEEN '2022-12-19 10:41:49' AND '2022-12-19 23:59:59' 
                ORDER BY  DESC;
                
**업데이트 문**
      
      UPDATE [테이블] SET [열] = '변경할값' WHERE [조건]
      
      
**DB 삭제**

      drop database 데이터베이스명
      
      
**기본 PK삭제 후 새롭게 PK 설정**

      ALTER TABLE study DROP id; 
      ALTER TABLE study ADD PRIMARY KEY (login_id);
