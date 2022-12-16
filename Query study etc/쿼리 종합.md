## SQL 순서 

      1. from 
      1-1 join 
      2. where 
      3. group by 
      4. having 
      5. select 
      6. order by


**아이디 및 비밀번호 확인 쿼리**

      $sql = "select * from admin.tb_bizring where biz_corp='안녕' and biz_corpnumber='$pwd'";

**type은 간편이고 카테고리로부터 찾고자하는 사람의 변수와 같은사람을 찾을게 그리고 내림차순 ~ !**

      $sql = "select * from admin.tb_bizring where $catagory like '%$search_con%' and biz_type = '간편' 
                      order by biz_regtime desc";
                
**시간 개념**

      "select  * FROM admin.tb_bizring WHERE biz_regtime BETWEEN '$date_to 00:00:00' AND '$date_from 23:59:59' 
                      ORDER BY biz_regtime DESC";
