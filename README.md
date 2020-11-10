# 숫자 야구 게임
## 진행 방법
* 숫자 야구 게임 요구사항을 파악한다.
* 요구사항에 대한 구현을 완료한 후 자신의 github 아이디에 해당하는 브랜치에 Pull Request(이하 PR)를 통해 과제를 제출한다.

## 과제 제출 과정
* [과제 제출 방법](https://github.com/next-step/nextstep-docs/tree/master/precourse)

## 학습 테스트 Todo-list
- 모든 단위 테스트 메서드는 DisplayName 어노테이션으로 `의도`를 드러낸다.
- String 클래스
    - [X] "1,2"를 ,로 split 했을 때 분리 여부를 확인한다.
    - [X] "1"을 ,로 split 했을 때 1만을 포함하는 배열이 반환되는지 확인한다.
    - [X] "(1,2)" 값이 주어졌을 때 substring으로 "1,2"를 반환하는 학습을 진행한다.
    - [X] "abc" 값이 주어졌을 때 charAt 메서드를 활용해서 특정 위치의 문자를 가져오는 학습을 진행한다.
    - [X] charAt 메서드가 찾는 문자가 위치 값을 벗어나면 StringIndexOutOfBoundsException이 발생하는지 확인한다.
- Set Collection
    - [ ] Set의 사이즈 메소드를 활용해 Set의 크기를 확인하는 학습을 진행한다.
    - [ ] contains 메서드를 통해 Set 안에 1,2,3의 값이 존재하는지 확인하는 학습을 진행한다
        - 제약조건: 반복문 없이 진행한다.
    - [ ] contains 메서드를 통해 true인 경우와 false인 경우를 모두 확인하는 학습을 진행한다.

## 야구게임 Todo-list
- 도메인
    - [ ] 야구게임숫자 구현
        - [ ] 1 ~ 9 사이의 숫자를 입력받아서 객체를 생성할 수 있다.
        - [ ] 범위를 벗어난 숫자로 객체 생성 시도 시 에러가 발생한다.
        - [ ] 객체간 값 비교가 가능하다.
    - [ ] 야구게임숫자 생성기 구현
        - [ ] 랜덤으로 야구게임숫자 중 한개를 반환한다.
            - 제약조건: 한번 뽑은 숫자는 다시 뽑을 수 없다.
    - [ ] 야구게임 구현
        - [ ] 랜덤으로 야구게임숫자 세 개를 뽑아서 게임을 시작할 수 있다.
        - [ ] 야구게임숫자를 받아서 게임의 결과를 반환한다.
            - [ ] 스트라이크 여부를 판단할 수 있다.
            - [ ] 볼 여부를 판단할 수 있다.
            - [ ] 포볼(or낫싱) 여부를 판단할 수 있다. 
- UI
    - [ ] 사용자로부터 세자리의 숫자를 입력받는다.
        - [ ] 숫자가 아닌 값을 입력 시도 시 에러 메시지를 보여준다.
        - [ ] 숫자의 자릿수가 다를 경우 에러 메시지를 보여준다.
    - [ ] 사용자에게 야구게임의 1회분의 결과를 보여준다.
    - [ ] 3 스트라이크 시 추가 게임 진행 여부를 물어본다.
        - [ ] 추가 게임 진행 시 새로운 게임을 진행한다.
        - [ ] 게임 종료 시 프로그램이 종료된다.
