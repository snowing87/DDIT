# nibang-naebang
SVN으로 형상관리를 진행하였습니다.
Github에서는 완성 소스코드만 조회할 수 있습니다.

# 설명
사용 기술 : <b>Java Fx, MariaDB, iBatis, PHP7, kakao Map, Geocoding</b>\
2019.06.10 2019.06.30\n

- 방 추천 알고리즘
사용자의
위치와 검색기록 조회 기록을 통해 맞춤 방 추천 기능을 구현하였습니다 주소 좌표 변환 API 를 활용하여
사용자 위치에서 가까운 방을 우선 조회한 후 사용자가 검색한 키워드가 포함되어 있거나 비슷한 조건을 가지고 있는
경우 방 추천 점수를 높여 일반 방보다 상단에 노출되도록 하였습니다
- 객관적인 방 점수 제공
주관적인
추천 점수가 있다면 사용자에게 객관적으로 이 방이 얼마나 좋은 조건을 가지고 있는지 보여줄 수 있는 객
관적인 점수가 필요할 것입니다 공공데이터를 활용하여 방 주변 상권을 파악하고 주위 방들과 조건을 비교하여 방의
점수를 분석한 후 사용자에게 다양한 차트를 이용하여 참고할 수 있는 점수를 제공하였습니다
- 효과적인 UX 구현
자신의 주소를 처음부터 끝까지 모두 입력하는 것은 사용자에게 불편한 경험을 줄 수 있다고 생각했습니다. 조금이라도 입력하는 주소의 양을 줄여서 사용자에게 좀 더 편안한 검색 환경을 제공해 주고 싶어서 방법을 찾아보았고 사용자가 시, 구 등을 입력하지 않아도 주소를 특정할 수 있는 일정 정보(**동) 만으로 완성된 주소를 제공할 수 있게 구현하였습니다.

# ERD
![image](https://user-images.githubusercontent.com/46917538/65937773-d8aec500-e45b-11e9-9c74-997696e9004b.png)

# 실행 화면
![image](https://user-images.githubusercontent.com/46917538/65937789-e3695a00-e45b-11e9-9aac-adc917a73217.png)
![image](https://user-images.githubusercontent.com/46917538/65937804-f11edf80-e45b-11e9-9769-1a3b60b4b201.png)

# 방 스코어 계산
![image](https://user-images.githubusercontent.com/46917538/65937822-ff6cfb80-e45b-11e9-829b-ea9437f9da7f.png)
![image](https://user-images.githubusercontent.com/46917538/65937834-08f66380-e45c-11e9-876a-49e6272a8983.png)

# 방 위치 표시
![image](https://user-images.githubusercontent.com/46917538/65937852-1875ac80-e45c-11e9-8770-dabda0cb915e.png)
