# spring boot api, bo 분리 기본 셋팅 

- spring boot를 이용해 demo-api(로직,쿼리), demo-bo(화면)로 분리하였습니다.
- demo-bo(화면)에서 demo-api로 요청을 보내고 결과값을 demo-bo(화면)로 반환합니다.
- 현재 api는 1개이지만 확장하여 api를 여러개로 나누어 관리할 수 있습니다.
  - (member-api, product-api, display-api, common-api ...)
- bo또한  확장하여 여러개로 나누어 관리할 수 있습니다.
  - (member-bo, product-bo, display-bo, common-bo ...)
- 한 화면에 필요한 여러개의 api를 각각 다르게 호출하여 데이터를 받을 수 있습니다.
- 프로젝트 별로 분리함으로써 오류나 장애가 발생했을 경우 해당부분만 신속히 대처가 가능합니다. 
- 화면을 통해 테스트 시 bo, api 서버 모두 실행해야 하며 현재 bo는 localhost로 api는 aws rds로 연결하였습니다.
- api는 REST api로 postman, swagger 등으로 테스트 가능합니다.

