# MyIdol

책상 위에 사는 도트 연습생. 물을 마시고, 스트레칭하고, 집중하면 연습생이 자라서 데뷔한다.

*A pixel trainee that lives on your desktop. Drink water, stretch, focus, and your trainee grows toward debut.*

이 저장소는 **배포 전용**입니다. 소스 코드는 비공개입니다.

---

## 다운로드

**[최신 버전 받기 →](https://github.com/lani319/myidol-releases/releases/latest)**

| | 파일 | 설명 |
|---|---|---|
| 설치판 | [MyIdol-x64-setup.exe](https://github.com/lani319/myidol-releases/releases/latest/download/MyIdol-x64-setup.exe) | 일반적인 설치. Windows 시작 시 자동 실행 지원 |
| 무설치판 | [MyIdol-x64-portable.zip](https://github.com/lani319/myidol-releases/releases/latest/download/MyIdol-x64-portable.zip) | 압축만 풀고 실행. 자동 실행 미지원 |

위 링크는 항상 **최신 버전**을 가리킵니다. 현재 버전과 변경 내역은 [릴리스 페이지](https://github.com/lani319/myidol-releases/releases/latest)에서 확인하세요.

Windows 10 이상 64비트. Microsoft Edge WebView2 런타임이 필요하며 최신 Windows에는 기본 포함되어 있습니다.

---

## ⚠️ 처음 실행할 때 경고가 뜹니다

이 앱에는 **코드 서명 인증서가 없습니다.** 그래서 다운로드와 실행 단계에서 Windows가 경고를 표시합니다. 파일이 손상됐거나 악성이라는 뜻이 아닙니다.

**1단계 — 브라우저 다운로드 경고**

Chrome이나 Edge가 "일반적으로 다운로드되는 파일이 아닙니다"라고 표시하면, 다운로드 항목의 `⋮` 메뉴에서 **[보관]** 또는 **[계속]** 을 선택하세요.

**2단계 — SmartScreen 파란 창**

실행하면 "Windows의 PC 보호" 창이 뜹니다.

```
[추가 정보]  ←  먼저 이걸 누르고
[실행]       ←  그 다음 이걸 누릅니다
```

한 번 통과하면 다음부터는 뜨지 않습니다.

**3단계 — 파일 무결성 직접 확인 (권장)**

받은 파일이 원본과 같은지 직접 대조할 수 있습니다. PowerShell에서:

```powershell
Get-FileHash .\MyIdol-x64-setup.exe -Algorithm SHA256
```

출력된 값이 아래 릴리스 노트의 SHA-256과 같으면 원본입니다.

---

## 들어 있는 것

- **책상 위 도트 연습생** 2종(하린, 도윤). 설정에서 교체
- **육성** — 물·스트레칭 알림, 집중 25분 세션, 할 일 완료로 스탯 상승. 3일/7일/14일 승급, 14일째 졸업 화면과 데뷔 카드
- **할 일** — 우클릭으로 추가, "내일 3시 회의" 같은 자연어 시간 파싱, 알림 말풍선에서 바로 완료/10분 뒤
- **캘린더** — ICS 비공개 주소 연동(읽기 전용), 하루 한 번 브리핑, N분 전 알림
- **OS 토스트 알림**, Windows 시작 시 자동 실행(설치판)
- **안무 연습** — 자리에 있을 때 25~45분마다 잠깐 춤

---

## 개인정보

**서버로 아무것도 보내지 않습니다.**

- 세이브, 할 일, 육성 상태는 `%APPDATA%\com.lani319.myidol\` 에만 저장됩니다
- 캘린더 ICS 주소는 Windows 자격 증명 관리자(키체인)에만 저장됩니다
- 캘린더를 연동하면 앱이 사용자가 지정한 주소로 **직접** 접속합니다. 개발자 서버를 거치지 않습니다
- 전역 키보드 후킹을 하지 않습니다
- 수집하는 사용 통계나 분석 도구가 없습니다

---

## 라이선스

MyIdol은 오픈소스가 아닙니다.

- 사용 조건: [EULA.txt](https://github.com/lani319/myidol-releases/releases/latest/download/EULA.txt)
- 최초 실행일로부터 **7일 체험** 가능. 이후 육성 기능이 정지되며 알림 기능은 계속 동작합니다
- 포함된 오픈소스 구성요소 고지: [THIRD-PARTY-NOTICES.txt](https://github.com/lani319/myidol-releases/releases/latest/download/THIRD-PARTY-NOTICES.txt)

수정하지 않은 원본 설치 파일을 비영리로 공유하는 것은 허용됩니다.

---

## 알려진 제한

- 코드 서명 없음 (위 참조)
- Windows 전용
- 캐릭터 그림은 코드로 그린 플레이스홀더. 정식 아트로 교체 예정
- 구글 ICS 피드는 구글 쪽 캐시 때문에 변경 반영이 몇 시간 늦을 수 있음

---

## 문의

버그 제보와 건의는 [Issues](https://github.com/lani319/myidol-releases/issues)로 남겨 주세요.
