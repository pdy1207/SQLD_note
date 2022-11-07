### SQL? 

  Structutred Query Language 구조화된 쿼리 언어  Data를 쉽게 다루기(추가,수정,삭제 등) 위해 고안된 언어
  
### DB는 뭐임?

  DB는 데이터 저장 창고다. 유튜브 영상, 인스타그램 사진, 댓글, 좋아요, 등등.. 디지털 정보를 저장 및 관리한다. <br>
  DB는 SQL 명령에 따라 움직인다. SQL로 작성된 명령, 이를 쿼리(qurey)라 한다.<br>
  데이터를 생성(Create), 조회(Read), 수정(Update), 삭제(Delete) 할 수 있다. 간단히 줄여 CRUD 할 수 있다.<br>
  
  <hr>
  
###   SQL 분류
  
   1. `DDL (Data Definition Language)` : 데이터 정의어로서, Data나 Schema를 정의하기 위해 사용한다.<br>
    CREATE, ALTER, DROP, TRUNCATE 등이 여기에 속한다.

  2. `DML (Data Manipulation Language)` : 데이터 조작어로서, Data를 조작하기 위해 사용한다.<br>
  SELECT, INSERT, UPDATE, DELETE 등이 여기에 속한다.

  3. `DCL (Data Control Language)` : 데이터 제어어로서, Data의 무결성 및 보안, 권한 등을 제어하기 위해 사용한다.<br>
  GRANT, REVOKE, COMMIT, ROLLBACK 등이 여기에 속한다.

  4. `TCL (Transaction Control Language)` : 보통 DCL로 취급하지만, transaction에 초점을 맞춰 구지 별개로 본다면,<br>
   이렇게 나눌 수 있다. COMMIT, ROLLBACK이 여기에 속한다.
