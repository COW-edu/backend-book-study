# 1장 - 객체, 설계
- 스터디 중 삼색볼펜법으로 체크한 부분들을 팀원들과 공유한 내용입니다.
- 스터디원들이 2명 이상 겹치는 부분은 강조표시(BOLD)가 되어 있습니다.
- 문장은 페이지의 오름차순으로 정렬되어 있습니다.

## 🔴 빨강 (아주 중요하다고 생각한 내용!)
- 이 책은 훌륭한 객체지향 프로그램을 설계하고 유지보수하는 데 필요한 원칙과 기법을 설명하기 위해 쓰여진 책이다.(8p)
- 설계에 관해 설명할 때 가장 유용한 도구는 이론으로 덕지덕지 치장된 개념과 용어가 아니라 코드 그 자체다.(8p)
- 마틴에 따르면 모든 모듈은 제대로 실행돼야 하고, 변경이 용이해야 하며, 이해하기 쉬워야 한다.(14p)
- 의존성은 변경에 대한 영향을 암시한다.(16p)
- 의존성이라는 말 속에는 어떤 객체가 변경될 때 그 객체에게 의존하는 다른 객체도 함꼐 변경될수 있다는 사실이 내포돼 있다.(16p)
- 이처럼 개념적이나 물리적으로 객체 내부의 세부적인 사항을 감추는 것을 캡슐화라고 부른다.(20p)
- 캡슐화의 목적은 변경하기 쉬운 객체를 만드는 것이다.(20p)
- 핵심은 객체 내부의 상태를 캡슐화하고 객체 간에 오직 메세지를 통해서만 상호작용 하도록 만드는 것이다.(25p)
- 밀접하게 연관된 작업만을 수행하고 연관성 없는 작업은 다른 객체에게 위임하는 객체를 가리켜 응집도가 높다고 말한다.(26p)
- 객체는 자신의 데이터를 스스로 처리하는 자율적인 존재여야 한다.(26p)
- 이처럼 데이터와 프로세스가 동일한 모듈 내부에 위치하도록 프로그래밍하는 방식을 객체지향 프로그래밍이라고 부른다(27p)
- 불필요한 세부사항을 캡슐화하는 자율적인 객체들이 낮은 결합도와 높은 응집도를 가지고 협력하도록 최소한의 의존성만을 남기는 것이 훌륭한 객체지향 설계다.(29p)
- 어떤 경우에도 모든 사람들을 만족시킬 수 있는 설계를 만들 수는 없다.(33p)
- 진정한 객체지향 설계로 나아가는 길은 협력하는 객체들 사이의 의존성을 적절하게 조절함으로써, 변경에 용이한 설계를 만드는 것이다.(36p)

## 🔵 파랑 (중요하다고 생각한 내용!)
- 이해 가능한 코드란 그 동작이 우리의 예상에서 크게 벗어나지 않는 코드다(15p)
- 관람객의 입장에서 문제는 소극장이라는 제3자가 초대장을 확인하기 위해 관람객의 가방을 마음대로 열어 본다는 데 있다.(15p)
- **따라서 우리의 목표는 애플리케이션의 기능을 구현하는 데 필요한 최소한의 의존성만 유지하고 불필요한 의존성을 제거하는 것이다(16p)**
- 따라서 설계의 목표는 객체 사이의 결합도를 낮춰 변경이 용이한 설계를 만드는 것이어야 한다.(17p)
- 객체 사이의 의존성이 과한 경우를 가리켜 결합도가 높다고 말한다.(17p)
- 두 객체 사이의 결합도가 높으면 높을수록 함께 변경될 확률도 높아지기 떄문에 변경하기 어려워진다(17p)
- 객체를 인터페이스와 구현으로 나누고 인터페이스만을 공개하는 것은 객체 사이의 결합도를 낮추고 변경하기 쉬운 코드를 작성하기 위해 따라야 하는 가장 기본적인 설계 원칙이다.(21p)
- 객체의 응집도를 높이기 위해서는 객체 스스로 자신의 데이터를 책임져야 한다.(26p)
- 이 관점에서 Theater의 enter 메서드는 프로세스이며, Audience, TicketSeller, Bag, TicketOffice는 데이터이다.(26p)
- 사실 그림 1.2는 절차적 프로그래밍 방식으로 작성된 코드의 전형적인 의존성 구조를 보여준다.(26p)
- **이처럼 프로세스와 데이터를 별도의 모듈에 위치시키는 방식을 절차적 프로그래밍이라고 부른다.(26p)**
- **변경하기 쉬운 설계는 한번에 하나의 클래스만 변경할 수 있는 설계다.(27p)**
- **따라서 객체가 어떤 데이터를 가지느냐보다는 객체에 어떤 책임을 할당할 것이냐에 초점을 맞춰야 한다.(29p)**
- 설계를 어렵게 만드는 것은 의존성이라는 것을 기억하라.(29p)
- 첫째, 어떤 기능을 설계하는 방법은 한 가지 이상일 수 있다.(33p)
- 둘째, 동일한 기능을 한 가지 이상의 방법으로 설계할 수 있기 때문에 결국 설계는 트레이드오프의 산물이다.(33p)
- 비록 현실에서는 수동적인 존재라고 하더라도,일단 객체지향의 세계에 들어오면 모든 것이 능동적이고 자율적인 존재로 바뀐다.(33p)
- 객체지향은 여러분이 세상에 대해 예상하는 방식으로 객체가 행동하리라는 것을 보장함으로써 코드를 좀 더 쉽게 이해할 수 있게 한다.(36p)

## 🟢 초록 (흥미롭다고 생각한 내용!)
- 이론이 먼저일까, 실무가 먼저일까(7p)
- 결론적으로 소프트웨어 설계와 유지보수에 중점을 두려면 이론이 아닌 실무에 초점을 맞추는 것이 효과적이다.(8p)
- 개발자는 구체적이니 코드를 만지며 손을 더럽힐 때 가장 많은 것을 얻어가는 존재다.(8p)
- 사실 관람객이 가방을 가지고 있다는 사실과 판매원이 매표소에서 티켓을 판매한다는 사실을 Theater가 알아야 할 필요가 없다.(18p)
- 캡슐화를 개선한 후에 가장 크게 달라진 점은 Audience와 TicketSeller가 내부 구현을 외부에 노출하지 않고 자신의 문제를 스스로 책임지고 해결한다는 것이다.
- 그의 반해 그림 1.8에 객체지향 설계에서는 제어 흐름이 각 객체에 적절하게 분산되어 있음을 알 수 있다.(28p)