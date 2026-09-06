---
name: proto-usage
description: Use when making or listing a throwaway web prototype that answers one design question, or when collecting play records from one — 웹 프로토타입을 새로 만들 때 · 목록을 갱신할 때 · 논 기록을 모을 때 ProtoTool 쓰는 법.
---

# 웹 프로토타입은 ProtoTool 로 만든다

**아직 뼈대다.** 코드가 없어서 여기 적을 명령도 없다. **1판이 나오면 채운다.**
지금 프로토타입을 만들어야 하면 아래 규약만 손으로 지키고, 부품 차례는 `Docs/Todo/할일.md` 를 본다.

## 어디서 부르나 — 명령 두 벌

| 어디서 쓰나 | 명령 앞자리 |
| --- | --- |
| 스튜디오(Officina) 저장소에서 | `ProtoTool/scripts/…` |
| 게임 저장소에서 (서브모듈) | `Tools/ProtoTool/scripts/…` |
| ProtoTool 저장소 단독에서 | `scripts/…` |

아래 표는 짧은 쪽으로 적는다. 실제로 칠 때는 위 앞자리를 붙인다.

## 지금도 지키는 규약

- **한 프로토타입은 한 파일이다** — `Prototypes/<날짜>-<이름>/index.html`, CSS·JS 인라인.
- 맨 위에 `proto-meta` JSON 덩이(물음 · 기준 · 만든날)를 둔다.
- **물음 하나에 프로토타입 하나.** 둘을 섞으면 불통일 때 뭐가 잘못인지 모른다.
- **버릴 코드다.** 그림·소리·UI 를 다듬지 않는다. 다듬으면 버리기 아까워진다.
- 논 뒤에는 같은 폴더 `결과.md` 에 기준 줄마다 통과/불통을 적는다.

자세한 규약과 폴더 모양은 `README.md` 의 「`Prototypes/` 규약」.

## 예정 명령 (1판이 나오면 여기 채운다)

| 이럴 때 | 이렇게 (예정) |
| --- | --- |
| 프로토타입을 새로 시작할 때 | 뼈대 한 장을 복사해 `Prototypes/<날짜>-<이름>/index.html` 로 둔다 |
| 시간이 흐르는 것을 시험할 때 | 뼈대의 틱 엔진을 켜고 빨리 감기(×1/×10/×60)를 쓴다 |
| 논 기록을 남길 때 | 화면의 「기록 내보내기」로 JSON 파일을 받아 같은 폴더에 둔다 |
| 목록을 갱신할 때 | 목록 생성기를 돌려 `Prototypes/index.html` 을 다시 만든다 |
| 판정 표가 필요할 때 | 기록 JSON 들을 모아 「물음 / 기준 / 통과·불통」 표를 뽑는다 (나중 부품) |
