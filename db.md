# Database

* MySQL 선택한 이유
  * 관계형 데이터베이스는...
  
* 프로젝트를 하면서 느낀 RDBMS와 DBMS의 차이점
  * 둘의 차이점은...
  
* ER diagram
 ![image](https://user-images.githubusercontent.com/77525358/110354439-7f4cbb80-807b-11eb-9b27-82df4c392b01.png)
    * **마름모**: 관계 타입
    * **동그라미**: 애트리뷰트 (엔티티를 기술하는 속성)  
           복합 애트리뷰트는 더 작은 구성요소로 나눌 수 있고 독립적인 의미를 가지는 애트리뷰트이고,  
           단순 애트리뷰트는 더 이상 나눌 수 없는 애트리뷰트  
    * **직사각형**: 엔티티 타입 (실세계에서 독립적으로 존재하는 실체)  
           엔티티 타입에 속하는 엔티티들에 대한 중요한 제약 조건은 애트리뷰트들에 대한 키 또는 유일함의 제약 조건이다. 키 제약 조건은 두 개 이상의 엔티티가 동시에 키 애트리뷰트에 대해 동일한            값을 가질 수 없도록 해주는 역할을 한다.
           
          - 일반적으로 데이터베이스의 요구사항들을 명시한 기술문에서 명사는 엔티티 타입 이름으로, 동사는 관계 타입 이름으로 되는 경향이 있다.
          - 애트리뷰트 이름은 엔티티 타입에 대응하는 명사를 설명하는 부가적인 명사들로부터 얻어진다.
           
    * **단일선과 이중선**: 참여 제약 조건  
                  이중선은 전체 참여(또는 존재 종속성)인 경우 엔터티 타입에 사용되고  
                  단일선은 부분 참여인 경우에 사용된다.  
    * **1,N,M**: 관계차수 1:1, 1:N, N:M (카디날리티)  
         예시)  
         1:1 관계 타입은 두 개의 엔티티는 서로 최대한 한 개의 관계 인스턴트에만 참여할 수 있는 관계이다. (한 사원(엔티티)이 한 부서(엔티티)만 관리할 수 있는 경우)  
         1:N 관계 타입은 두 개의 엔티티 중 하나의 엔티티만이 여러 개의 관계 인스턴트에 참여할 수 있는 관계이다. (한 사원만이 여러개의 프로젝트를 참여할 수 있는 경우)  
         M:N 관계 타입은 두 개의 엔티티 중 모두 여러 개의 관계 인스턴트에 참여할 수 있는 관계이다. (여러 명의 사원들이 여러 개의 프로젝트에 참여할 수 있는 경우)  
         
    * 참고문헌
 -[Designing an ER Diagram](https://www.youtube.com/watch?v=8JFaaD1vzSY&t=376s)
* Schema
  * schema
  ![image](https://user-images.githubusercontent.com/77525358/110330419-122c2c80-8061-11eb-8791-5c7829a582f3.png)
     **:heavy_check_mark: schema에서 카디날리티가 가장 핵심!!!:heavy_check_mark:**
         
         1:1 혹은 1:N 관계 타입은 참여하고 있는 엔티티 타입들 중의 하나로 통합될 수 있다. 다만 1:N 관계 타입에서는 관계 애트리뷰트가 관계의 N측 엔티티 타입으로만 이동할 수 있다는 점을  
         꼭 유의해야 한다. 
         위와 반대로 M:N 관계 타입에서는 관계 인스턴스에 참여하는 엔티티들의 조합에 의해서 결정되는 일부 애트리뷰들이 있어 반드시 관계 애트리뷰트로 명시되어야 한다.
    * 참고문헌
      -[How to convert an ER diagram to the Relational Data Model](https://www.youtube.com/watch?v=CZTkgMoqVss)
      
  * Schema diagram (spread sheet 사용)
  ![image](https://user-images.githubusercontent.com/77525358/110263144-17ee2780-7ff9-11eb-9379-db48519316f0.PNG)
  ![image](https://user-images.githubusercontent.com/77525358/110263106-fee57680-7ff8-11eb-9640-4b20e6cc30fb.PNG)
  ![image](https://user-images.githubusercontent.com/77525358/110263124-0b69cf00-7ff9-11eb-8ef3-6de22abc4f3f.PNG)
    * 참고문헌
 -[Converting ER Diagrams to Schemas](https://www.youtube.com/watch?v=xQRRf5fOAt8&t=557s)
* 새로 알게 된 SQL문
* 자주 쓰이는 SQL문 정리
  * 컬럼 관련
    * 1) 컬럼명 바꾸기
    * 2) 컬럼 순서 바

  * 데이터 관련
