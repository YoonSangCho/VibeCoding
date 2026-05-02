# ViveCoding

# 🎵 바이브 코딩(Vibe Coding) 실습 가이드

> AI와 함께하는 직관적 코딩 — 자연어로 아이디어를 코드로 바꾸는 실습

---

## 📚 목차

1. [바이브 코딩이란?](#바이브-코딩이란)
2. [실습 환경 1: VS Code + Claude](#실습-환경-1-vs-code--claude)
   - Visual Studio Code 소개 및 설치
   - Claude란?
   - VS Code에 Claude 연동하기
3. [실습 환경 2: Amazon Kiro](#실습-환경-2-amazon-kiro)
   - Kiro 소개
   - Kiro 설치 및 시작하기
4. [두 환경 비교](#두-환경-비교)

---

## 🌊 바이브 코딩이란?

**바이브 코딩(Vibe Coding)**이란 AI에게 자연어로 원하는 것을 설명하고, AI가 코드를 생성해 주는 방식의 개발 스타일입니다.  
코드 문법을 몰라도, 아이디어를 말로 풀어내면 AI가 코드를 짜줍니다.

> 💡 "로그인 폼 만들어줘", "투두 앱을 React로 만들어줘" → AI가 코드 생성

---

## 실습 환경 1: VS Code + Claude

### 🖥️ Visual Studio Code (VS Code) 소개

**Visual Studio Code**는 Microsoft가 만든 **무료 오픈소스 코드 에디터**입니다.  
Windows, macOS, Linux 모두 지원하며, 전 세계 개발자들이 가장 많이 사용하는 에디터 중 하나입니다.

**주요 특징:**
- ✅ 완전 무료
- ✅ 수천 가지 확장(Extension) 지원
- ✅ Git 내장 통합
- ✅ 통합 터미널 제공
- ✅ 다양한 언어 지원 (Python, JavaScript, TypeScript 등)
- ✅ AI 코딩 도구와의 뛰어난 호환성

**📥 다운로드:**  
👉 [https://code.visualstudio.com/download](https://code.visualstudio.com/download)

| 운영체제 | 다운로드 |
|--------|--------|
| Windows | `.exe` 인스톨러 다운로드 후 실행 |
| macOS | `.dmg` 또는 `.zip` 다운로드 |
| Linux | `.deb` / `.rpm` / Snap 선택 |

---

### 🤖 Claude란?

**Claude**는 Anthropic이 만든 **AI 어시스턴트**입니다.  
코드 작성, 디버깅, 설명, 아이디어 제안 등 개발 전반을 도와주는 AI입니다.

**Claude의 특징:**
- 🧠 자연어로 코드 요청 가능
- 🔍 코드베이스 전체를 이해하고 맥락 파악
- 🛠️ 파일 수정, 명령어 실행, 테스트 자동화 지원
- 🔒 코드는 모델 학습에 사용되지 않음 (프라이버시 보호)

> 💬 claude.ai에서 바로 사용하거나, VS Code와 연동해 에디터 안에서 사용 가능

---

### 🔌 VS Code에 Claude 연동하기 (Claude Code 확장)

#### 사전 준비물
- VS Code 1.98.0 이상
- Anthropic 계정 (claude.ai 가입) — Claude Pro, Max, Team, Enterprise 플랜 필요
- Node.js 18 이상 (선택: CLI 방식 사용 시)

#### 설치 방법

**방법 1: VS Code 확장 마켓플레이스에서 설치 (추천)**

1. VS Code 실행
2. 확장 탭 열기: `Ctrl+Shift+X` (Windows/Linux) 또는 `Cmd+Shift+X` (Mac)
3. 검색창에 `Claude Code` 입력
4. **Anthropic** 공식 퍼블리셔의 확장 선택 → `Install` 클릭
5. 설치 완료 후 사이드바에 ⚡ 스파크 아이콘 확인
6. 패널 클릭 → **Sign in** 버튼으로 Anthropic 계정 로그인

**방법 2: 직접 링크로 설치**

```
vscode:extension/anthropic.claude-code
```

브라우저 주소창에 위 주소를 붙여넣거나, VS Code Command Palette(`Ctrl+Shift+P`)에서 입력

#### 로그인 방법

```bash
# 처음 실행 시 브라우저 창이 열리며 Anthropic 계정으로 인증
# Claude Pro/Max 구독자: OAuth 방식 자동 로그인
# API 키 방식: Anthropic Console(console.anthropic.com)에서 API Key 발급 후 입력
```

#### 주요 기능
- **인라인 코드 제안**: 코드 작성 중 AI 자동 완성
- **채팅으로 요청**: 자연어로 기능 구현 요청
- **파일 @-멘션**: 특정 파일/라인을 대화에 포함
- **Diff 미리보기**: 변경 사항 확인 후 적용
- **대화 기록**: 이전 세션 이어서 작업 가능

---

## 실습 환경 2: Amazon Kiro

### 🚀 Amazon Kiro란?

**Amazon Kiro**는 Amazon AWS가 만든 **에이전트형 AI IDE**입니다.  
VS Code + Claude를 개별적으로 연동하는 대신, **AI와 IDE가 처음부터 하나로 통합**된 도구입니다.

> 💡 한 줄 요약: "VS Code의 편리함 + Claude급 AI + Amazon의 구조화된 개발 방식"

**공식 소개:** *"The AI IDE for prototype to production"*  
자연어 프롬프트 → 구조화된 스펙 → 실제 동작하는 코드까지 원스톱으로 처리합니다.

**📥 다운로드:**  
👉 [https://kiro.dev/downloads/](https://kiro.dev/downloads/)

| 운영체제 | 지원 |
|--------|------|
| Windows | ✅ |
| macOS | ✅ |
| Linux | ✅ |

---

### ✨ Kiro의 핵심 기능

#### 1. 📋 스펙 기반 개발 (Spec-Driven Development)
바이브 코딩의 가장 큰 단점인 "방향성 상실"을 해결하는 핵심 기능입니다.

```
사용자: "사용자 인증 기능 만들어줘"
Kiro: → 요구사항 정의
      → 시스템 설계 문서 생성
      → 구현 태스크 분리
      → 코드 + 테스트 + 문서 자동 생성
```

#### 2. 🤖 에이전트 훅 (Agent Hooks)
파일 저장, 커밋 등의 이벤트에 AI 에이전트를 자동 트리거  
예: 파일 저장 시 자동으로 린팅, 보안 취약점 스캔, 문서 업데이트

#### 3. 🧭 스티어링 파일 (Steering)
팀의 코딩 컨벤션(들여쓰기 규칙, 네이밍, 모듈 구조)을 마크다운 파일로 정의하면  
Kiro가 해당 규칙에 맞게 코드를 생성합니다.

#### 4. 🔌 MCP 서버 통합
외부 도구(GitHub, AWS, 데이터베이스 등)를 Kiro와 직접 연결 가능

#### 5. 📦 VS Code 호환
VS Code의 설정, 테마, Open VSX 플러그인을 그대로 가져올 수 있습니다.

---

### 📥 Kiro 설치 및 시작하기

#### 설치 단계

1. **다운로드**: [https://kiro.dev/downloads/](https://kiro.dev/downloads/) 에서 OS에 맞는 파일 선택
2. **실행**:
   - Windows: `.exe` 파일 더블클릭 → 설치 마법사 진행
   - macOS: `.dmg` 열기 → Applications 폴더로 드래그
3. **라이선스 동의**: AWS Customer Agreement 동의
4. **로그인**: 아래 계정 중 하나로 로그인 (AWS 계정 불필요!)
   - Google 계정
   - GitHub 계정
   - AWS Builder ID
   - 조직 IAM Identity Center
5. **VS Code 설정 가져오기** (선택): 기존 VS Code 환경 그대로 이어서 사용 가능
6. **테마 선택**: Kiro Dark / Kiro Light

#### 요금제

| 플랜 | 가격 | 에이전트 한도 |
|------|------|------------|
| **Free** (Preview) | 무료 | 월 50회 |
| **Pro** | 추후 공개 | 월 1,000회 |
| **Pro+** | 추후 공개 | 월 3,000회 |

> 현재 Preview 기간 중 무료로 사용 가능합니다!

---

## 📊 두 환경 비교

| 항목 | VS Code + Claude | Amazon Kiro |
|------|-----------------|-------------|
| **설치 복잡도** | 중간 (별도 설정 필요) | 낮음 (올인원) |
| **AI 통합** | Claude Code 확장 | 처음부터 내장 |
| **바이브 코딩** | ✅ | ✅ |
| **스펙 기반 개발** | 직접 구성 필요 | ✅ 기본 제공 |
| **에이전트 자동화** | 제한적 | ✅ Agent Hooks |
| **VS Code 호환** | 그 자체가 VS Code | ✅ 설정 가져오기 지원 |
| **무료 사용** | Claude Pro 구독 필요 | Preview 중 무료 |
| **추천 대상** | VS Code 기존 사용자 | 처음 시작하는 분 |

---

## 🏁 시작하는 순서 (추천)

```
1단계: VS Code 설치 → Claude Code 확장 연동 → 간단한 앱 바이브 코딩 체험
          ↓
2단계: Amazon Kiro 설치 → 동일한 프로젝트를 Kiro로 재현해보기
          ↓
3단계: 두 도구의 차이점 직접 체감 → 나에게 맞는 환경 선택
```

---

> 📌 **참고 링크**
> - VS Code 공식: https://code.visualstudio.com
> - Claude Code 문서: https://docs.claude.com
> - Amazon Kiro 공식: https://kiro.dev
> - Kiro 문서: https://kiro.dev/docs/
