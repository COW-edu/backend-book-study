# 8장 - 유연한 설계
- 스터디 중 삼색볼펜법으로 체크한 부분들을 팀원들과 공유한 내용입니다.
- 스터디원들이 2명 이상 겹치는 부분은 강조표시(BOLD)가 되어 있습니다.
- 문장은 페이지의 오름차순으로 정렬되어 있습니다.

## 🔴 빨강 (아주 중요하다고 생각한 내용!)
- 동일한 클래스 안에서 객체 생성과 사용이라는 두 가지 이질적인 목적을 가진 코드가 공존하는 것이 문제인 것이다. (287)
- 상위 수준의 모듈은 하위 수준의 모듈에 의존해서는 안 된다. 둘 모두 추상화에 의존해야 한다. (302)
- 추상화는 구체적인 사항에 의존해서는 안 된다. 구체적인 사항은 추상화에 의존해야 한다. (302)
- 유연성은 코드를 읽는 사람들이 복잡함을 수용할 수 있을 때만 가치가 있다. (305)

## 🔵 파랑 (중요하다고 생각한 내용!)
- 추상화 과정을 거치면 문맥이 바뀌더라도 변하지 않는 부분만 남게 되고 문맥에 따라 변하는 부분은 생략된다. (284)
- **의존성 관점에서 개방-폐쇄 원칙을 따르는 설계란 컴파일 타임 의존성은 유지하면서 런타임 의존성의 가능성을 확장하고 수정할 수 있는 구조라고 할 수 있다.** (284)
- 개방-폐쇄 원칙에서 폐쇄를 가능하게 하는 것은 의존성의 방향이다. (285)
- **변경에 위한 파급효과를 최대한 피하기 위해서는 변하는 것과 변하지 않는 것이 무엇인지를 이해하고 이를 추상화 목적으로 삼아야만 한다.** (286)
- 결합도가 높아질수록 개발-폐쇄 원칙을 따르는 구조를 설계하기가 어려워진다. (287)
- 유연하고 재사용 가능한 설계를 원한다면 객체와 관련된 두가지 책임을 서로 다른 객체로 분리해야 한다. 하나는 객체를 생성하는 것이고, 다른 하나는 객체를 사용하는 것이다. (288)
- 이처럼 생성과 사용을 분리하기 위해 객체 생성에 특화된 객체를 FACTORY라고 부른다. (289)
- 크레이그 라만은 이처럼 책임을 할당하기 위해 창조되는 도메인과 무관한 인공적인 객체를 PURE FABRICATION(순수한 가공물)이라고 부른다. (291)
- 만약 도메인 개념이 만족스럽지 못하다면 주저하지 말고 인공적인 객체를 창조하라. (292)
- SERVICE LOCATOR 패턴의 가장 큰 단점은 의존성을 감춘다는 것이다. (297)
- **숨겨진 의존성이 이해하기 어렵고 디버깅하기 어려운 이유는 문제점을 발견할 수 있는 시점을 코드 작성 시점이 아니라 실행 시점으로 미루기 때문이다.** (298)
- 클래스의 사용법을 익히기 위해 구현 내부를 샅샅이 뒤져야 한다면 그 클래스의 캡슐화는 무너진 것이다. (298)
- **유연하고 재사용 가능한 설계를 원한다면 모든 의존성의 방향이 추상 클래스나 인터페이스와 같은 추상화를 따라야 한다.** (301)
- 의존성을 역전시켜야만 유연하고 재사용 가능한 설계를 얻을 수 있다. (304)
- 추상화를 별도의 독립적인 패키지가 아니라 클라이언트가 속한 패키지에 포함시켜야 한다. (304)
- **핵심은 객체를 생성하는 방법에 대한 결정은 모든 책임이 자리를 잡은 후 가장 마지막 시점에 내리는 것이 적절하다는 것이다.** (307)

## 🟢 초록 (흥미롭다고 생각한 내용!)
- 이제 Client는 Factory를 사용해서 생성된 Movie의 인스턴스를 반환받아 사용하기만 하면 된다. (290)
- 객체지향이 실세계를 모방해야 한다는 헛된 주장에 현혹될 필요가 없다. (292)
