# Claude Code 키보드 단축키 정리

## 1. 일반 컨트롤

| 단축키 | 설명 |
|---|---|
| `Ctrl+C` | 현재 입력 또는 생성 취소 |
| `Ctrl+D` | Claude Code 세션 종료 |
| `Ctrl+L` | 프롬프트 입력 삭제 |
| `Ctrl+R` | 명령어 히스토리 역검색 |
| `Ctrl+O` | 트랜스크립트 뷰어 토글 |
| `Ctrl+T` | 작업 목록 토글 |
| `Ctrl+G` 또는 `Ctrl+X Ctrl+E` | 기본 텍스트 에디터에서 열기 |
| `Ctrl+V` / `Alt+V` (Windows) | 클립보드에서 이미지 붙여넣기 |
| `Ctrl+B` | 현재 Bash 명령어 백그라운드 실행 |
| `Ctrl+X Ctrl+K` | 모든 백그라운드 에이전트 종료 (3초 내 2회) |
| `Esc Esc` | 되감기 또는 요약 |
| `↑ / ↓` | 명령어 히스토리 탐색 |
| `← / →` | 대화 탭 순환 |

## 2. 모드 전환

| 단축키 | 설명 |
|---|---|
| `Shift+Tab` 또는 `Alt+M` | 권한 모드 순환 (`default` → `acceptEdits` → `plan` → `auto` → `bypassPermissions`) |
| `Alt+P` (Windows/Linux) / `Option+P` (macOS) | 모델 전환 |
| `Alt+T` (Windows/Linux) / `Option+T` (macOS) | Extended thinking 토글 |
| `Alt+O` (Windows/Linux) / `Option+O` (macOS) | Fast mode 토글 |

## 3. 텍스트 편집

| 단축키 | 설명 |
|---|---|
| `Ctrl+K` | 커서부터 줄 끝까지 삭제 |
| `Ctrl+U` | 커서부터 줄 시작까지 삭제 |
| `Ctrl+Y` | 삭제한 텍스트 붙여넣기 |
| `Alt+Y` | 붙여넣기 히스토리 순환 (Ctrl+Y 이후) |
| `Alt+B` | 커서를 한 단어 뒤로 이동 |
| `Alt+F` | 커서를 한 단어 앞으로 이동 |

## 4. 여러 줄 입력

| 방법 | 설명 |
|---|---|
| `\` + `Enter` | 모든 터미널에서 작동 |
| `Option+Enter` (macOS) | macOS 기본값 |
| `Shift+Enter` | iTerm2, WezTerm, Ghostty, Kitty 지원 |
| `Ctrl+J` | 라인 피드 문자 입력 |

## 5. 빠른 입력 접두사

| 접두사 | 설명 |
|---|---|
| `/` | 슬래시 명령어 또는 스킬 목록 표시 |
| `!` | Bash 명령어 직접 실행 |
| `@` | 파일 경로 자동완성 |

## 6. 트랜스크립트 뷰어

| 단축키 | 설명 |
|---|---|
| `Ctrl+O` | 트랜스크립트 뷰어 열기/닫기 |
| `Ctrl+E` | 모든 콘텐츠 표시 토글 |
| `q` / `Ctrl+C` / `Esc` | 뷰어 종료 |

## 7. Vim 편집 모드

> `/vim` 명령어 또는 설정으로 활성화

### 모드 전환

| 키 | 동작 |
|---|---|
| `Esc` | NORMAL 모드 진입 |
| `i` | 커서 앞에 삽입 |
| `I` | 줄 시작에 삽입 |
| `a` | 커서 뒤에 삽입 |
| `A` | 줄 끝에 삽입 |
| `o` / `O` | 아래/위에 새 줄 열기 |

### 이동 (NORMAL 모드)

| 키 | 동작 |
|---|---|
| `h / j / k / l` | 좌/하/상/우 이동 |
| `w / e / b` | 다음 단어 / 단어 끝 / 이전 단어 |
| `0 / $` | 줄 시작 / 줄 끝 |
| `gg / G` | 입력 시작 / 끝 |
| `f{char}` / `F{char}` | 해당 문자로 앞/뒤 이동 |

### 편집 (NORMAL 모드)

| 키 | 동작 |
|---|---|
| `dd` / `D` | 줄 삭제 / 끝까지 삭제 |
| `cc` / `C` | 줄 변경 / 끝까지 변경 |
| `yy` / `p` / `P` | 줄 복사 / 뒤에 붙여넣기 / 앞에 붙여넣기 |
| `.` | 마지막 변경 반복 |
| `>>` / `<<` | 들여쓰기 / 내어쓰기 |

## 8. 단축키 커스터마이징

- 설정 파일: `~/.claude/keybindings.json`
- 활성화: `/keybindings` 명령어

## 9. macOS 주의사항

`Alt+B`, `Alt+F`, `Alt+M`, `Alt+P`, `Alt+T` 등 Alt 단축키 사용 시 Option을 Meta로 설정 필요:
- **iTerm2:** Settings → Profiles → Keys → `Esc+` 선택
- **Terminal.app:** Settings → Keyboard → `Use Option as Meta Key` 체크
- **VS Code:** `"terminal.integrated.macOptionIsMeta": true`

## 10. 예약된 단축키 (변경 불가)

| 단축키 | 이유 |
|---|---|
| `Ctrl+C` | 중단/취소 (하드코딩) |
| `Ctrl+D` | 종료 (하드코딩) |
| `Ctrl+M` | Enter와 동일 |
