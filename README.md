# javascript-racingcar-precourse

# 구현 기능 목록

<aside>
💡
주어진 미션을 수행하기 위해 달성해야 할 기준과 목표가 담겨야 한다.
미션을 분석하면서 해결을 위해 필요하다고 생각되는 체크포인트를 작성한다.
</aside>

---

- [x] 구현할 기능 목록을 README.md에 추가
- [x] 사용자 입력 받기
  - [x] 자동차 이름 입력 받기
  - [x] 시도할 게임 횟수 입력 받기
- [x] 입력값 검증 로직 구현하기
  - [x] 자동차 이름 입력 테스트 케이스
    - 잘못된 값
      - `''` : 빈 문자열
      - `,,` : 구분자만 입력
      - `pobi,` : 사람 수 ≤ 구분자 수
      - `pobi jun` : 구분자 없는 경우
      - `pobi, jun` , `pobi, j un`, `pobi, ,jun` : 공백이 있는 경우
      - `pobipobi,jun` : 5자 초과인 이름이 있는 경우
    - 올바른 값
      - `pobi`
      - `pobi,jun`
      - `pobbi,junnn,hierk`
  - [x] 시도할 게임 횟수 입력 테스트 케이스
    - 잘못된 값
      - 음수
      - 0
      - 실수(소수점 포함), NaN, 숫자 타입을 제외한 모든 타입
    - 올바른 값
      - 양수
      - 숫자 타입
- [ ] 게임 기능 구현
  - [ ] 주어진 횟수 동안 진행
    - [x] 1회 진행할 때마다, 각 자동차의 무작위 값 구하기
    - [x] n대의 자동차 조건에 따라 움직이기
      - [x] 무작위 값 4이상
        - 자동차 전진
      - [x] 무작위 값 3이하
        - 자동차 멈춤
    - [x] 전진하는 자동차 출력
      - [x] 이름 출력 (멈춘 자동차도 같이 출력)
      - [x] 전진한 길이 출력
- [ ] 결과 출력
  - [ ] 최종 우승자 출력
    - [ ] 최종 우승자 1명
      - `최종 우승자 : ${name}`
    - [ ] 최종 우승자 n명
      - `최종 우승자 : ${name1}, ${name2}`
- [ ] 예외 처리
  - `[ERROR]${에러메시지}`
  - Error 발생 후 애플리케이션 종료
