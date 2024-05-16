### 요구사항 분석
- 회원은 상품을 주문할 수 있다.
- 주문 시 여러 종류의 상품을 선택할 수 있다.

### 기능 목록
- 회원 기능
  - 회원 등록
  - 회원 조회
- 상품 기능
  - 상품 등록
  - 상품 수정
  - 상품 조회
- 주문 기능
  - 상품 주문
  - 주문 내역 조회
  - 주문 취소

### 도메인 모델 분석
- 회원과 주문의 관계: 회원은 여러 번 주문할 수 있다(일대다).
- 주문과 상품의 관계: 주문할 때 여러 상품을 선택할 수 있다. 반대로 같은 상품도 여러 번 주문될 수 있다. 주문 상품이라는 모델을 만들어 다대다 관계를 일대다, 다대일 관계로 풀어냄.

### 요구사항 추가
- 상품의 종류는 음반, 도서, 영화가 있고 이후 확장 가능성이 있다.
- 모든 데이터는 등록일, 수정일이 필수다.
