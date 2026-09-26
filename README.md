# Career System

취업 준비 과정에서 지원자 정보를 일관되게 관리하고, 채용공고 분석부터 자기소개서 작성·검수까지 진행하기 위한 개인용 시스템입니다.

## 구성

| 위치 | 용도 |
| --- | --- |
| [`Career_System_Common_Rules.md`](Career_System/Career_System_Common_Rules.md) | 모든 단계에 공통으로 적용하는 질문·검토·승인 규칙 |
| [`Data/Career_Master_Profile_v1.4.md`](Career_System/Data/Career_Master_Profile_v1.4.md) | 학력, 프로젝트, 직접 수행한 역할, 기술 및 성과에 대한 기준 정보 |
| [`Data/Personal_Writing_Knowledge_Base_v0.4.md`](Career_System/Data/Personal_Writing_Knowledge_Base_v0.4.md) | 과거 자기소개서의 문항별 기록, 인사이트 및 작성 방식 |
| [`Data/Experience_Story_Bank_v1.0_READ_ONLY.md`](Career_System/Data/Experience_Story_Bank_v1.0_READ_ONLY.md) | 이전에 정리한 사건별 경험 참고 자료(읽기 전용) |
| [`Prompts/`](Career_System/Prompts/) | 단계별 실행 프롬프트 |
| [`Guide/Career_System_사용_가이드_Notion.html`](Career_System/Guide/Career_System_사용_가이드_Notion.html) | 실제 사용 순서를 설명하는 Notion용 가이드 |
| [`Review/`](Career_System/Review/) | 변경 내역 및 검토 자료 |

## 사용 순서

1. 공통 규칙과 최신 Career Master Profile, Writing Knowledge Base를 준비합니다.
2. [`01_Career_Profile_로딩`](Career_System/Prompts/01_Career_Profile_로딩.md)으로 기준 정보를 설정합니다.
3. 필요할 때만 [`02_지원가치_판단_중복지원_선택`](Career_System/Prompts/02_지원가치_판단_중복지원_선택.md)을 실행합니다.
4. [`03_최종_직무_선정`](Career_System/Prompts/03_최종_직무_선정.md)으로 지원 직무를 결정합니다.
5. [`04_지원서_전체_전략`](Career_System/Prompts/04_지원서_전체_전략.md)에서 문항별 경험을 배정합니다.
6. [`05_자소서_단일_문항_작성`](Career_System/Prompts/05_자소서_단일_문항_작성.md)을 문항별로 실행합니다.
7. [`06_지원서_전체_QA`](Career_System/Prompts/06_지원서_전체_QA.md)로 제출 전 전체를 검수합니다.

자세한 초기 설정 및 사용 방법은 [사용 가이드](Career_System/Guide/Career_System_사용_가이드_Notion.html)를 참고합니다.

## 자료 사용 원칙

- 지원자에 관한 사실은 Career Master Profile을 우선합니다.
- 과거 자기소개서의 해석과 표현은 Writing Knowledge Base에서 참고하며, 새로운 사실의 증거로 자동 확정하지 않습니다.
- 중요한 경험 변경, 전략 수정, 파일 수정은 사용자 검토와 승인 후 반영합니다.
- 개인정보가 포함될 수 있으므로 저장소는 **Private**으로 관리합니다.
