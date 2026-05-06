# Commit Convention

## 커밋 메시지 구조

```
<type> <subject>

<body>

<footer>
```

---

## 언어 규칙

- 커밋 메시지(subject, body)는 **한글**로 작성합니다.

---

## 헤더 형식 규칙

- type은 `< >` 문자로 감싸서 작성합니다.
- 예시: `<fix> 긴급 Fix`, `<feat> 로그인 기능 추가`

---

## Type (필수)

| 타입 | 설명 |
|------|------|
| `feat` | 새로운 기능 추가 |
| `fix` | 버그 수정 |
| `docs` | 문서 수정 (README 등) |
| `style` | 코드 포맷팅, 세미콜론 누락 등 (로직 변경 없음) |
| `refactor` | 코드 리팩토링 (기능 변경 없음) |
| `test` | 테스트 코드 추가 또는 수정 |
| `chore` | 빌드 설정, 패키지 관리 등 기타 변경 |

---

## Scope (선택)

변경된 범위를 괄호 안에 작성합니다.

예: `feat(auth)`, `fix(api)`, `docs(readme)`

---

## Subject (필수)

- 변경 사항을 간결하게 요약 (50자 이내)
- 마침표 사용 금지
- 명령형으로 작성 (예: "추가한다", "수정한다")

---

## Body (선택)

- 변경 이유 및 내용을 상세히 설명
- 72자마다 줄바꿈
- Subject와 한 줄 공백으로 구분

---

## Footer (선택)

- 관련 이슈 번호 참조: `Closes #123`, `Refs #456`
- Breaking Change 명시: `BREAKING CHANGE: <설명>`

---

## 예시

```
<feat> 소셜 로그인 기능 추가

Google, Kakao OAuth2 로그인을 지원합니다.
기존 이메일 로그인과 병행하여 사용 가능합니다.

Closes #42
```

```
<fix> 긴급 Fix

userId가 없을 경우 예외 처리 없이 null을 반환하던
문제를 수정하여 404 응답을 반환하도록 변경합니다.

Refs #87
```
