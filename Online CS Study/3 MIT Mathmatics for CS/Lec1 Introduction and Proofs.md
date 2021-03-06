# Lec1: Introduction and Proofs

# 증명이란?

가정들에서 결론들이 논리적으로 얻어질 수 있는 일련의 명제들?

> 증명은 진실을 **확증(진실을 설립하고 입증, ascertaining)**하는 방법론이다.
> 

## 확증의 예

관찰, 실험 

# **어떻게 진실이 설립되는가?**

어느것이 진실이 아닌지 안다면, 진실을 걸러낼 수 있다.

**그렇다면 어떻게 진실이 아님을 알 수 있는가?**

- 반례 찾기
- 샘플링 (예를 들기, 귀납적으로 실험해보기)
- 판사들의 판단(진실에 따라 판단을 내림)
- 종교, 신
- 사장님의 말
- 교수님의 말
- conviction(강한 신념)

# 수학적인 개념에서 증명이란?

> **수학적인 증명(mathmatic proof)**이란 일련의 **공리**(a set of **axioms**)로부터 **논리적 연역(추론)**(a chain of logical deduction)을 통해 **명제(proposition)**를 검증(verification)하는 것이다.
> 

# 명제란?

> **명제(proposition)**란 참(true)이거나 거짓(false)인 진술(statement)이다.
> 

예시 명제) 

- 2+3=5
- 모든 자연수(0,1,2,3,4, …)에 대해 **n^2+n+41은 소수(prime number)이다.**

→ 여기서 파란 부분을 **술어(predicate)**라고 한다. 그리고 그 앞부분을 수량자(quantifier)라고 한다.

> **술어**란 진리(truth)가 변수의 값(n)에 의존하는 명제이다.
> 

| n | n^2+n+41 | prime |
| --- | --- | --- |
| 0 | 41 | ✔️ |
| 1 | 43 | ✔️ |
| 2 | 47 | ✔️ |
| 3 | 53 | ✔️ |
| … | … | … |
| 20 | 461 | ✔️ |
| … | … | … |
| 39 | 1601 | ✔️ |

참인 명제처럼 보이지만

40^2+40+41=1681=41^2

으로 40에서 거짓이다.

또한 n=41에서 41의 배수가 되기 때문에 거짓이다.

# 첫번째 예시 명제

예시 명제) a^4+b^4+c^4=d^4는 양의 정수 해가 없다.

→ 양의 정수 a,b,c,d에 대해 다음을 성립하는 abcd가 존재한다, **a^4+b^4+c^4=d^4** 

- 1796년 오일러에 의해 참으로 드러남
- 2세기 넘게 풀리지 않음
- 추측된지 218년후 한 수학자에 의해 증명됨

a=95800

b=217519

c=414560

d=422481

# 두번째 예시 명제

예시 명제) 313*(x^3+y^3)=z^3은 양의 정수해가 없다.

- 거짓으로 판명됨
- 하지만 이를 성립하는 가장 작은 해는 1000자리가 넘는다.

### 근데 이걸 왜 알아야 하나?

수학자거나 수학 관련 대학원에 진학하여 수학 전문가가 되고 싶다면, 필요한 개념일지 모르겠으나 굳이 알 필요가 없는 것처럼 보인다. 그럼에도 이런 논리(인수분해)들은 RSA라는 암호학(cryptography)에도 사용된다. 다음주에 암호 시스템에 어떻게 적용되는지 더 살펴보자

# 세번째 예시 명제

예시 명제) **4색 정리:** 모든 지도의 영역은 4가지 색상으로 색칠할 수 있으므로 인접한 영역은 서로 다른 색상을 갖게 되어 구별할 수 있다. → 되게 유명함

- 사진을 통해 증명된 적이 있고, 이 증명이 오랫동안 믿어진 적 있음
- 설득력 있어 보이는 증명 이지만, 사진을 통해 증명한 것은 매우 잘못됨.
- 사진을 통한 증명은 일반적으로 좋지 못함 (왜냐하면 두뇌가 그 사진 안에 갇히기 때문)
- 1977년에 증명되었지만 수천가지 경우를 확인하려면 컴퓨터를 사용해야 했음

# 네번째 예시 명제

예시 명제) 2를 제외한 모든 짝수 양수 정수는 두 소수의 합이다.

- 골드 바흐의 추측(conjecture)이라고 불리며 1742년에 골드바흐에 의해 추측되었음
- ex) 24=11+13
- 아직도 사실인지 발견되지 않았음

# 유명한 명제들

- 리만 가설(1859), 아직 밝혀지지 않았음
- 푸앙카레 추측 (2003년 참인 것으로 증명됨→필즈상 수상함, 올해 초 100만달러(10억원)의 밀레니엄 상도 받음, 하지만 두 상 모두 거부함)

# Implication 이란?

예시 명제) 모든 정수에 대해 n≥2 ⇒(implies) n^2≥4

> 만약 p가 거짓이거나 q가 참이라면 **암시, 함축(implication)** p⇒q는 참이다
> 

진리표(truth table)

| p | q | p⇒q |
| --- | --- | --- |
| T | T | T |
| T | F | F |
| F | T | T |
| F | F | T |

**돼지는 날 수 있다 ⇒ 나는 왕이다**

는 참인 implication이다. 왜냐면 돼지는 날 수 없기 때문이다.

돼지가 날지 않기 때문에 내가 왕인지 아닌지는 중요하지 않다. 

예시 명제) 모든 정수에 대해 n≥2 <=>(iff, if and only if) n^2≥4

- 거짓이다. n=-3일 때.
- <=>는 <=이랑 ⇒ 모두 확인해야 한다.

진리표

| p | q | p⇒q | q⇒p | p<=>q |
| --- | --- | --- | --- | --- |
| T | T | T | T | T |
| T | F | F | T | F |
| F | T | T | F | F |
| F | F | T | T | T |

# 명제가 아닌 것들에 관하여

**“이것은 명제이다”**는 명제가 아니다

- **“이것은 명제이다"**가 참이라면 명제이므로 거짓이 될 것이고, 거짓이라면 명제가 아니므로 참이 될 것이기 때문이다. 이는 모순이다. 참도 아니고 거짓도 아니다.

좀 더 간단하게는 질문이나 인사는 명제가 아니다. 

# 공리(axiom)에 관하여

다음 시간에는 axioms 공리에 대해 배울 것이다. 공리는 실제로 명제와 같다. 유일한 차이점은 참이라고 가정하는 명제이다.

> **공리(axiom)**는 참이라고 가정하는 명제이다.
> 

→ 공리가 참이라는 증거는 없다. 그저 합리적인 명제라고 생각하기에 참이라고 가정한다.

ex) if a=b & b=c , then a=c

### 공리는 다른 관점에서 모순이 될 수도 있다.

→ 유클리드 기하학(평면 기하학, euclidean geometry)에서는 선 L과 L 위에 있지 않은 점 p가 주어지면 L에 평행한 p를 통해 정확히 하나의 선이 있다는 중심 공리가 있다.

→ 구형 기하학(sperical geometry)에서는 위 것과 모순되는 공리가 있다. 선 L과 L 위에 있지 않은 점 p가 주어지면 구에서 L에 평행한 p를 지나는 선은 없다.

→ 쌍곡 기하학(hyperbolic geometry)에서는 선 L과 L 위에 있지 않은 점 p가 주어지면, L과 평행한 p를 지나는 선이 무한히 많다는 공리가 있다.

 이러한 관점들이 서로 모순되기에 서로 다른 공리들을 가지고 있지만, 이들은 다양한 분야에서 의미가 있다.

공리에는 두가지 원칙이 있다.

1. 일관성(consistence)
2. 완전성(complete)

> 어떤 **명제(propositions)가 참과 거짓으로 증명될 수 없다면** 일련의 공리(a set of axioms)는 **일관성(consistence)**이 있다.
> 

> 공리의 집합은 **모든 명제가 참 또는 거짓임을 증명하는 데 사용할 수 있는** 경우 **완전(complete)**하다고 한다.
> 

cf) 노력으로도 안 되는 게 있다. 예를 들자면 공리를 증명하는 것(?)