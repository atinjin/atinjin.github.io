---
layout: page
title: Seraph2
permalink: /seraph2/
---

## Seraph2 — 개인용 AI 비서

Seraph2 는 **개발자 본인 한 사람이 쓰기 위해 만든 개인용 AI 비서**입니다.
Telegram 메신저로 대화하면, 일정·메일·할 일·메모를 대신 확인하고 정리해
줍니다.

운영자의 개인 컴퓨터(macOS)에서 직접 실행되며, 별도의 서버나 회원 가입이
없습니다. 공개 서비스가 아니고, 다른 사용자를 받지 않습니다.

---

### 무엇을 하나요

- **일정** — Google 캘린더의 일정을 읽고, 요청하면 새 일정을 만들거나
  수정합니다.
- **메일** — Gmail 의 최근 메일과 본문을 읽어 요약하고, 읽음 표시나
  보관(Archive) 처리를 합니다. **메일을 보내거나 삭제하지는 않습니다.**
- **할 일 · 메모** — macOS 미리알림과 개인 노트를 읽고 씁니다.
- **정기 브리핑** — 정해둔 시각에 그날 필요한 내용을 먼저 알려 줍니다.

### Google 계정 권한을 왜 요청하나요

위 기능 중 일정과 메일은 Google 계정의 데이터가 없으면 동작할 수 없습니다.
그래서 다음 두 가지 권한을 요청합니다.

| 권한 | 쓰는 이유 |
| --- | --- |
| Google Calendar | 일정 조회·생성·수정 |
| Gmail (읽기 및 라벨 변경) | 메일 조회·요약, 읽음/보관 처리 |

권한은 **운영자 본인의 Google 계정 하나**에만 연결됩니다. 부여한 권한은
언제든 [Google 계정 설정](https://myaccount.google.com/permissions)에서
회수할 수 있습니다.

데이터를 어떻게 다루는지는 [개인정보처리방침]({{ site.url }}/seraph2/privacy/)에
자세히 적어 두었습니다. 이용 조건은 [서비스 약관]({{ site.url }}/seraph2/terms/)을
참고하십시오.

---

### 만든 사람

- 개발·운영: atinjin
- 문의: [atinjin@gmail.com](mailto:atinjin@gmail.com)
- 소스 코드: [github.com/atinjin/seraph-v2](https://github.com/atinjin/seraph-v2)
