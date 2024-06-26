## 요구사항 분석
#### 특강 목록 조회, 등록, 삭제 API
1. 여러 개의 특강을 날짜 별로 등록할 수 있다. (수강 정원은 30명으로 고정하지 않았으나, 등록 시 제어한다.)
2. 같은 이름의 특강을 등록할 수 없다.
3. 종료되었거나, 수강 신청자가 없는 특강은 삭제할 수 있다.


#### 특강 신청 API
1. 특강을 선택하여 신청할 수 있다.
2. 각 유저는 동일한 특강을 중복으로 신청할 수 없다.
3. 동시적인 신청 요청에 대해 동시성을 제어하며, 순차적으로 처리
4. 수강 정원이 다 찬 특강은 신청할 수 없다.


#### 특강 신청 여부 조회 API
1. 각 유저에 대해 특강 신청 내역이 존재하는지의 메세지를 반환한다.


#### 특강 신청 취소 API
1. 특강 신청을 취소한다.
2. 이미 진행된 특강은 신청 취소할 수 없다.

- [x] TDD 기반으로 service 계층의 구현 객체와 명세 구현
- [x] 서비스 계층을 추상화, 각 기능 책임에 따라 서비스 컴포넌트를 분리
- [x] domain Entity와 Repository 계층 구현
- [x] controller 계층 구현
- [x] 특강 목록 조회, 등록, 삭제, 신청 취소 API 구현 


## [요구사항명세서](https://applebanana.atlassian.net/wiki/spaces/~6029c153c5a0430067bd79ce/pages/65961985)

## ERD 초기 설정

![image](https://github.com/K-J-HYEON/hhplus-tdd-lecture/assets/77037051/63736880-4735-463e-b869-24967f886218)
