---
layout: page
title: Seraph2 개인정보처리방침
permalink: /seraph2/privacy/
---

## Seraph2 개인정보처리방침

최종 수정일: 2026년 9월 12일

Seraph2([소개]({{ site.url }}/seraph2/))는 개발자 본인 한 사람이 쓰기 위해
만든 개인용 AI 비서입니다. 공개 서비스가 아니며 다른 사용자를 받지
않습니다. 따라서 이 방침이 말하는 "이용자" 는 곧 운영자 본인입니다.

---

### 1. 수집하는 정보

Seraph2 는 회원 가입을 받지 않고, 이용자가 직접 연결한 계정의 데이터만
다룹니다.

- **Google 계정 데이터** — 이용자가 OAuth 동의로 직접 연결한 경우에 한해
  Google 캘린더 일정과 Gmail 메시지(제목·본문·발신자·라벨)를 읽습니다.
- **대화 내용** — Telegram 으로 주고받은 메시지.
- **기기 내 개인 데이터** — macOS 미리알림, 개인 노트 등 이용자가 기능을
  요청했을 때 접근하는 항목.

광고 식별자, 위치 정보, 결제 정보는 수집하지 않습니다.

### 2. 이용 목적

수집한 정보는 이용자가 요청한 기능을 수행하는 데에만 씁니다 — 일정 확인과
등록, 메일 요약과 정리, 할 일 관리, 정기 브리핑 발송. 그 밖의 목적으로는
사용하지 않습니다.

### 3. 저장 위치와 보관 기간

모든 데이터는 **운영자 개인 컴퓨터(macOS) 안에만** 저장됩니다. 외부 서버로
옮겨 보관하지 않습니다.

- 대화 기록·일정 캐시·메모: 로컬 SQLite 데이터베이스 (`~/.seraph2/`)
- Google 인증 토큰: 로컬 파일에 소유자만 읽을 수 있는 권한(0600)으로 저장

보관 기간은 따로 정해져 있지 않으며, 이용자가 로컬 데이터베이스 파일을
삭제하면 즉시 사라집니다.

### 4. 제3자 제공

수집한 정보를 **판매하거나 광고·마케팅 목적으로 제공하지 않습니다.**
기능 수행에 반드시 필요한 다음 경우에만 외부로 전달됩니다.

| 전달 대상 | 전달되는 것 | 이유 |
| --- | --- | --- |
| LLM 공급자 ([OpenRouter](https://openrouter.ai/privacy) 및 그가 중계하는 모델 제공사) | 이용자가 요청한 작업 처리에 필요한 대화·문서 내용 | 자연어 이해·응답 생성 |
| [Telegram](https://telegram.org/privacy) | 주고받는 메시지 | 메신저 전송 |

법령에 따라 적법한 절차로 요구되는 경우 외에는 그 밖의 제공이 없습니다.

### 5. Google 사용자 데이터의 제한적 사용 (Limited Use)

Seraph2 가 Google API 로부터 받은 정보의 이용·전송은
[Google API 서비스 사용자 데이터 정책](https://developers.google.com/terms/api-services-user-data-policy)을
따르며, 여기에는 **제한적 사용(Limited Use) 요건**이 포함됩니다.

> Seraph2's use and transfer of information received from Google APIs to any
> other app will adhere to the
> [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy),
> including the Limited Use requirements.

구체적으로 Seraph2 는 Google 사용자 데이터를 다음과 같이 다룹니다.

- 이용자에게 보이는 기능을 제공하는 목적으로만 사용합니다.
- 광고 목적으로 사용하거나 제3자에게 판매하지 않습니다.
- 사람이 읽지 않습니다. 단, 이용자 본인이 명시적으로 동의했거나, 보안
  목적(예: 남용 조사)이거나, 법령을 준수해야 하거나, 데이터가 통계 목적으로
  집계·익명화된 경우는 예외입니다.

### 6. 권한 회수와 데이터 삭제

- **Google 권한 회수** — [Google 계정 권한 관리](https://myaccount.google.com/permissions)
  에서 Seraph2 의 액세스를 언제든 제거할 수 있습니다. 제거하면 Seraph2 는
  더 이상 캘린더·Gmail 에 접근하지 못합니다.
- **로컬 데이터 삭제** — 운영자 컴퓨터의 `~/.seraph2/` 디렉터리를 삭제하면
  저장된 대화·캐시·토큰이 모두 사라집니다.

### 7. 보안

- Google 인증 토큰은 로컬 파일 권한 0600(소유자 전용)으로 저장합니다.
- 재인증 과정의 임시 수신 서버는 `127.0.0.1` 에만 연결을 받아, 같은 컴퓨터
  바깥에서는 접근할 수 없습니다.
- 외부 통신은 모두 HTTPS 로 이루어집니다.

다만 Seraph2 는 개인이 운영하는 소프트웨어이며, 어떤 방식도 완벽한 보안을
보장하지는 못합니다.

### 8. 아동의 개인정보

Seraph2 는 만 14세 미만 아동을 대상으로 하지 않으며, 아동의 개인정보를
의도적으로 수집하지 않습니다.

### 9. 방침 변경

이 방침이 바뀌면 이 페이지의 내용과 최종 수정일을 갱신합니다.

### 10. 문의

개인정보 처리에 관한 문의: [atinjin@gmail.com](mailto:atinjin@gmail.com)
