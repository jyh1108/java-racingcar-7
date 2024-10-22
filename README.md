초간단 자동차 경주 게임

기능 요구 사항

주어진 횟수 동안 n대의 자동차는 전진 또는 멈출 수 있다.
각 자동차에 이름을 부여할 수 있다. 전진하는 자동차를 출력할 때 자동차 이름을 같이 출력한다.
자동차 이름은 쉼표(,)를 기준으로 구분하며 이름은 5자 이하만 가능하다.
사용자는 몇 번의 이동을 할 것인지를 입력할 수 있어야 한다.
전진하는 조건은 0에서 9 사이에서 무작위 값을 구한 후 무작위 값이 4 이상일 경우이다.
자동차 경주 게임을 완료한 후 누가 우승했는지를 알려준다. 우승자는 한 명 이상일 수 있다.
우승자가 여러 명일 경우 쉼표(,)를 이용하여 구분한다.
사용자가 잘못된 값을 입력할 경우 IllegalArgumentException을 발생시킨 후 애플리케이션은 종료되어야 한다.

프로그래밍 요구 사항 - 
indent(인덴트, 들여쓰기) depth를 3이 넘지 않도록 구현한다. 2까지만 허용한다.
예를 들어 while문 안에 if문이 있으면 들여쓰기는 2이다.
힌트: indent(인덴트, 들여쓰기) depth를 줄이는 좋은 방법은 함수(또는 메서드)를 분리하면 된다.
3항 연산자를 쓰지 않는다.
함수(또는 메서드)가 한 가지 일만 하도록 최대한 작게 만들어라.



-- 구현할 기능 목록 --

1. 자동차 이름 입력 처리
    자동차 이름을 쉼표(,)로 구분하여 입력받는다.
    각 이름이 5자 이하인지 검증한다.
    잘못된 입력 시 IllegalArgumentException을 발생시키고 애플리케이션을 종료한다.

2. 이동 횟수 입력 처리
    사용자가 몇 번의 이동을 할 것인지 입력받는다.
    입력이 정수인지 검증하고 잘못된 입력 시 IllegalArgumentException을 발생시키고 애플리케이션을 종료한다.

3. 자동차 객체 생성
    입력받은 이름을 기반으로 자동차 객체를 생성한다.
    자동차 객체는 이름과 전진 거리를 저장할 수 있어야 한다.

4. 자동차 전진 로직
    0에서 9 사이의 무작위 값을 생성한다.
    값이 4 이상일 경우 해당 자동차는 한 칸 전진한다.
    각 자동차의 이동 상황을 기록한다.

5. 자동차 이동 결과 출력
    매 이동이 끝날 때마다 각 자동차의 이름과 현재 위치(전진 거리)를 출력한다.

6. 우승자 판별 및 출력
    모든 이동이 끝난 후, 가장 멀리 이동한 자동차를 우승자로 판별한다.
    우승자가 여러 명일 경우 쉼표(,)로 구분하여 출력한다.

7. 예외 처리
    력값에 대해 적절한 예외 처리를 구현한다.
    잘못된 자동차 이름, 잘못된 이동 횟수 입력 등 다양한 경우에 대해 IllegalArgumentException을 발생시킨다.


