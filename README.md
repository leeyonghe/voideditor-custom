# Void 커스터마이징

**Void**는 오픈소스 코드 에디터로, AI 에이전트와의 통합을 통해 개발 생산성을 극대화합니다. 사용자는 코드베이스 내에서 AI와 직접 대화하며, 코드 변경 사항을 체크포인트로 저장하고 시각화할 수 있습니다. Void는 모든 AI 메시지를 외부 제공자에게 직접 전송하며, 사용자의 데이터는 저장하지 않습니다.

Void는 Microsoft의 VSCode를 기반으로 하여, VSCode의 안정성과 확장성을 유지하면서 AI 중심의 개발 환경을 제공합니다. VSCode의 오픈소스 라이선스(MIT)를 따르며, 커뮤니티 기여를 통해 지속적으로 발전하고 있습니다. 이 프로젝트는 VSCode의 기본 기능을 유지하면서, AI 통합 및 커스터마이징을 통해 개발자 경험을 향상시키는 것을 목표로 합니다.

### 주요 기능
- 다양한 AI 모델 및 호스트를 로컬/원격에서 자유롭게 연결
- 코드 변경 이력의 시각적 추적 및 롤백(체크포인트)
- VSCode 기반의 친숙한 UI/UX, 오픈소스 커뮤니티 중심 개발
- 데이터 프라이버시 보장: 메시지/코드가 서버에 저장되지 않음
- 확장 가능한 플러그인/익스텐션 구조

### 폴더 구조 예시
- `src/`: 에디터 및 주요 기능 소스코드
- `extensions/`: 플러그인 및 확장 기능
- `scripts/`: 빌드 및 배포 스크립트

### 설치 및 실행
```bash
git clone https://github.com/voideditor/void.git
cd void
npm install
# 빌드: (VSCode에서 Ctrl+Shift+B 또는 아래 명령어)
npm run watch
# 실행: (OS별)
# Windows: ./scripts/code.bat
# Mac/Linux: ./scripts/code.sh
```
자세한 빌드/실행 방법은 [HOW_TO_CONTRIBUTE.md](https://github.com/voideditor/void/blob/main/HOW_TO_CONTRIBUTE.md)를 참고하세요.

### 윈도우 환경에서 빌드 시 주의사항
- 윈도우 환경에서 빌드하려면 Visual Studio 2022 또는 VS Build Tools가 필요합니다. 자세한 설치 방법은 [HOW_TO_CONTRIBUTE.md](https://github.com/voideditor/void/blob/main/HOW_TO_CONTRIBUTE.md)를 참고하세요.
- 추가적인 빌드 라이브러리(예: MSVC, C++ ATL, C++ MFC 등)가 필요할 수 있습니다. 설치 시 "Workloads" 및 "Individual Components" 탭에서 필요한 항목을 선택하세요.
	- MSVC v143 - VS 2022 C++ x64/x86 Spectre-mitigated libs (Latest)

### 기여 방법
- [VOID_CODEBASE_GUIDE.md](https://github.com/voideditor/void/blob/main/VOID_CODEBASE_GUIDE.md)에서 코드 구조를 확인하세요.
- [HOW_TO_CONTRIBUTE.md](https://github.com/voideditor/void/blob/main/HOW_TO_CONTRIBUTE.md)에서 빌드 및 PR 가이드를 확인하세요.
- Discord, Issue, PR 등 다양한 방법으로 자유롭게 참여할 수 있습니다.
