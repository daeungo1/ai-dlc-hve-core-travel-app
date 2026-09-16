# AI-DLC with HVE core - Travel app

2박3일 여행 일정을 자동 설계하는 앱을 주제로, HVE Core의 Design Thinking 코칭 프레임워크(9 메서드)를 따라 진행한 기록입니다. 코드가 아니라 **의사결정 과정**이 산출물입니다.

## 프로젝트 한 줄 요약

> 단기 여행자는 추천 정보가 부족해서가 아니라, 흩어진 후보를 동선과 시간 제약에 맞춰 실행 가능한 시간표로 조립하는 데 2~3시간을 쓴다.

## 진행 현황

| 메서드 | 이름 | 상태 |
|--------|------|------|
| 1 | Scope Conversations | 완료 |
| 2 | Design Research | 완료 |
| 3 | Input Synthesis | 완료 |
| 4 | Brainstorming | 완료 |
| 5 | User Concepts | 진행 중 (5c 평가) |
| 6-9 | Prototypes / Testing / Iteration | 미착수 |

Problem Space(1-3)를 통과해 Solution Space(4-6)에 들어와 있습니다.

## 이 기록에서 실제로 바뀐 것들

요청은 frozen으로 도착했지만, 과정을 거치며 여러 판단이 뒤집혔습니다.

| 시점 | 무엇이 바뀌었나 |
|------|-----------------|
| Method 1 | 제약 10개를 전부 Frozen으로 분류 |
| Method 2 | Frozen 제약 2개가 근거에 반증됨. 계획은 PC에서 일어나고, 동행자는 합의 주체가 아니라 조건 제시자였음 |
| Method 3 | 핵심 가설(조립 노동) 검증됨. 단일 출처 테마 1개는 규율에 따라 기각 |
| Method 3 | 수정 루프를 HMW2에 흡수하고 스코프에서 제외 |
| Method 4 | 제외한 수정 루프가 발산에서 아이디어 5개짜리 테마로 재등장 |
| Method 5 | 재등장의 근거가 실제로 더 강했음이 확인됨. Method 3 종합이 놓친 패턴 |

## 근거

모든 판단은 인터뷰 4건과 화면 관찰 1건에 연결되어 있습니다. 참여자는 P1부터 P4까지 익명 라벨로만 기록했고, 녹음은 하지 않았습니다.

대표 인용:

> "추천은 널렸는데, 몇 시에 뭘 할지는 아무도 안 알려줘요." (P2)

> "막상 가보면 동선이 꼬여서 두 군데는 그냥 포기해요." (P1)

> "저는 정해주면 따라가는 편이에요. 대신 이동 오래 걸리는 건 싫어요." (P4)

## 아티팩트 구조

```text
.copilot-tracking/dt/travel-agent-p/
├── coaching-state.md              # 세션 상태, 전환 로그, 의사결정 이력
├── method-01-scope/               # 스테이크홀더 맵, 스코프 경계, 가정 로그
├── method-02-research/            # 리서치 계획, 인터뷰 원자료, 관찰, 결과 요약
├── method-03-synthesis/           # 어피니티 클러스터, 인사이트, 문제 정의, HMW
├── method-04-brainstorming/       # 발산 18개, 철학 기반 해법 테마 5개
├── method-05-concepts/            # 테마 선정, concepts.yml, 스테이크홀더 정렬
└── canonical/                     # Method 1 시점 스냅샷 (현재 stale)
```

## 알려진 한계

* 표본이 작습니다. Tier1 3명, Tier2 1명이며 전원 지인 접촉이라 선택 편향이 있습니다.
* Hidden 스테이크홀더(개인정보 담당)와 한 번도 접촉하지 않았습니다.
* `canonical/` 스냅샷은 Method 1 시점이라 Method 2 근거와 어긋납니다.
* Method 5c 평가는 실제 스테이크홀더 없이 역할극으로 수행됩니다.

## 참고

Design Thinking 프레임워크는 [microsoft/hve-core](https://github.com/microsoft/hve-core)의 HVE Design Thinking 확장을 사용했습니다.
