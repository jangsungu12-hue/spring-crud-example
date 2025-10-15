# Spring Boot 게시판 CRUD

## 개요
Spring Boot와 H2 DB를 이용해 게시글 CRUD 기능을 구현한 간단한 REST API 프로젝트입니다.

## 기술 스택
- Java 21, Spring Boot 3.5.6
- Spring Data JPA, H2 Database
- Maven, Eclipse

## 실행 방법
1. 프로젝트 클론 후 Eclipse에서 열기  
2. `BoardApplication` 실행  
3. H2 콘솔 접속 (선택): http://localhost:9090/h2-console  
   - JDBC URL: `jdbc:h2:mem:testdb`  
   - 사용자명: `sa`, 비밀번호 없음

## API 요약

| 메서드 | URL            | 설명           |
|--------|----------------|----------------|
| POST   | /posts         | 게시글 생성    |
| GET    | /posts         | 전체 게시글 조회 |
| GET    | /posts/{id}    | 게시글 상세 조회 |
| PUT    | /posts/{id}    | 게시글 수정    |
| DELETE | /posts/{id}    | 게시글 삭제    |

## 테스트
Postman 등으로 JSON 형태 요청 보내면 됩니다.

---

작성자: 장성우 
