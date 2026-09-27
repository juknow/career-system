# Career System

취업 준비 과정에서 지원자 정보를 일관되게 관리하고, 채용공고 분석부터 자기소개서 작성·검수까지 진행하기 위한 개인용 시스템입니다.

## 구성

| 위치 | 용도 |
| --- | --- |
| [`Career_System_Common_Rules.md`](Career_System/Career_System_Common_Rules.md) | 모든 단계에 공통으로 적용하는 질문·검토·승인 규칙 |
| [`Data/Career_Master_Profile.md`](Career_System/Data/Career_Master_Profile.md) | 학력, 프로젝트, 직접 수행한 역할, 기술 및 성과에 대한 기준 정보 |
| [`Data/Personal_Writing_Knowledge_Base.md`](Career_System/Data/Personal_Writing_Knowledge_Base.md) | 과거 자기소개서의 문항별 기록, 인사이트 및 작성 방식 |
| [`Data/Experience_Story_Bank.md`](Career_System/Data/Experience_Story_Bank.md) | 사건별 경험 카드. 원문 근거와 사용자 승인 범위에서 수정·추가 |
| [`Prompts/`](Career_System/Prompts/) | 단계별 실행 프롬프트 |
| [`Guide/Career_System_사용_가이드_Notion.html`](Career_System/Guide/Career_System_사용_가이드_Notion.html) | 실제 사용 순서를 설명하는 Notion용 가이드 |
| [`Review/`](Career_System/Review/) | 변경 내역 및 검토 자료 |

## 사용 순서

**처음 한 번:** ChatGPT 웹의 Career System 프로젝트 지침을 등록하고, 아래 **네 개의 MD 파일을 모두 프로젝트 소스에 등록**합니다. Story Bank는 등록 필수이지만 구체적인 사건을 확인할 때만 참조하며, 별도 승인 없이 내용을 수정하지 않습니다. Google Drive의 지원서 원본 폴더도 연결합니다. 기존 `01_Career_Profile_로딩` 파일은 보존하지만 프로젝트 내부에서는 매번 실행하지 않습니다.

**프로젝트 소스 초기 등록 목록**

1. [Career_System_Common_Rules.md](Career_System/Career_System_Common_Rules.md)
2. [Career_Master_Profile.md](Career_System/Data/Career_Master_Profile.md)
3. [Personal_Writing_Knowledge_Base.md](Career_System/Data/Personal_Writing_Knowledge_Base.md)
4. [Experience_Story_Bank.md](Career_System/Data/Experience_Story_Bank.md)
5. [Google Drive · Career_Originals/Applications](https://drive.google.com/drive/folders/1H6306HKrzjMN5e_8-DO49w8pH0Lepuc-) 폴더를 프로젝트 소스에 연결합니다. 필요한 경우 Google Drive 앱 권한을 승인합니다. 폴더 링크 등록만으로 전체 파일이 미리 읽히거나 동기화되는 것은 아니므로, 과거 지원서가 필요할 때 실제 원문을 검색·열람합니다. 연결이 불가능하다면 접근 가능한 Private GitHub 백업을 이용하거나 해당 원문을 채팅에 첨부합니다.

GitHub·Google Drive의 변경 사항은 프로젝트 소스의 등록 파일을 자동 갱신하지 않으므로, 원본 파일이 바뀌면 직접 교체합니다.

**기업별 작업:**

1. 필요할 때만 [`02_지원가치_판단_중복지원_선택`](Career_System/Prompts/02_지원가치_판단_중복지원_선택.md)을 실행합니다.
2. [`03_최종_직무_선정`](Career_System/Prompts/03_최종_직무_선정.md)으로 지원 직무를 확정합니다.
3. [`04_지원서_전체_전략`](Career_System/Prompts/04_지원서_전체_전략.md)에서 문항별 경험을 배정합니다.
4. [`05_자소서_단일_문항_작성`](Career_System/Prompts/05_자소서_단일_문항_작성.md)을 문항별로 실행합니다.
5. [`06_지원서_전체_QA`](Career_System/Prompts/06_지원서_전체_QA.md)로 제출 전 전체를 검수합니다.

새 채팅에 이전 단계의 확정 결과가 없다면 확정 직무·문항별 경험 배정표의 해당 내용 등을 직접 전달합니다. 프로젝트 공통 파일은 접근 가능하면 반복 첨부하지 않아도 됩니다.

자세한 초기 설정 및 사용 방법은 [사용 가이드](Career_System/Guide/Career_System_사용_가이드_Notion.html)를 참고합니다.

## 자료 사용 원칙

- 지원자에 관한 사실은 Career Master Profile을 우선합니다.
- 과거 자기소개서의 해석과 표현은 Writing Knowledge Base에서 참고하며, 새로운 사실의 증거로 자동 확정하지 않습니다.
- 중요한 경험 변경, 전략 수정, 파일 수정은 사용자 검토와 승인 후 반영합니다.
- 이 저장소는 **Public**이며 공통 규칙·경력 기준 자료·프롬프트·가이드의 기준 위치입니다. 경력 자료에도 개인정보가 포함될 수 있으므로 공개 전 내용을 확인합니다. 자기소개서 원문·원본 PDF는 이 공개 저장소에 올리지 않습니다.
- `.gitignore`는 새 파일이 실수로 추가되는 것을 줄이지만, 이미 커밋한 파일이나 과거 Git 이력을 삭제하지는 않습니다.

## 자동 백업과 개인 원본 보관

| 대상 | 원본 / 수정 위치 | 자동 백업 위치 |
| --- | --- | --- |
| 공통 규칙·Master·Writing KB·프롬프트·가이드·Review | [Public career-system](https://github.com/juknow/career-system)의 동일 파일 | [Private career-system-private](https://github.com/juknow/career-system-private)의 동일 경로 |
| 지원서 PDF·원문 MD/TXT | Google Drive의 `Career_Originals/Applications/연도/기업명/` | Private의 `Career_System/Data/Essay_Archive/연도/기업명/` |

- Google Apps Script의 `syncDriveToGitHub`가 약 5분마다 변경 사항을 확인하는 **단방향** 백업입니다. 작업 성공 여부는 Apps Script의 트리거와 최신 실행 로그에서 확인합니다. 자동화 오류가 발생하면 최신 파일의 반영이 지연될 수 있습니다.
- Private의 공통 파일을 직접 수정하지 않습니다. 공통 자료는 사용자 승인 후 Public 파일에서 수정하고, 개인 원본은 Google Drive에 저장합니다.
- ChatGPT 프로젝트에 등록한 자료와 Notion 페이지는 GitHub·Drive 자동 백업으로 자동 갱신되지 않습니다. 공통 파일이 바뀌면 ChatGPT 프로젝트에 최신 파일을 다시 등록하고, Notion 가이드는 필요할 때 직접 갱신합니다.
- 실제 사용 및 오류 확인 절차는 [Notion용 사용 가이드](Career_System/Guide/Career_System_사용_가이드_Notion.html)를 참고합니다. GitHub 접근 토큰은 어떤 저장소에도 커밋하지 않습니다.
