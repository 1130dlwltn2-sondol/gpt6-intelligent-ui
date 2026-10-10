# 후속 작업 안내 (handoff)

## 파일 구조

```
gpt6-intelligent-ui/
├── README.md                  # 책 소개 (위키독스 연동용)
├── TOC.md                     # 전체 목차 (위키독스 연동용)
├── manuscript_full.md         # 전체 통합 원고 (편집용)
├── references.md              # 원문 제목·기관·발표일·접근일·URL·권리 상태
├── qa_report.md               # 검증 PASS/FAIL/미확인 기록
├── handoff.md                 # 이 파일
├── chapters/
│   ├── 01.md ~ 08.md          # 장별 원고 (위키독스 게시용)
├── pages/
│   ├── 00-cover.md            # 표지
│   ├── 01-copyright.md        # 판권·사용 안내
│   ├── 02-preface.md          # 머리말
│   ├── 03-preparation.md       # 준비물·기능 확인
│   ├── 04-toc.md              # 목차
│   ├── 05-chapter-01.md ~ 12-chapter-08.md  # chapters/ 복사본 (위키독스 페이지 순서)
│   ├── 13-final-project.md    # 종합 실습
│   ├── 14-glossary.md         # 용어집·출처
│   ├── 15-final-guide.md       # 마지막 안내
├── assets/
│   ├── cover.png              # 표지 (1000x1300)
│   ├── fig-concept-elements.png   # 1장 도식
│   ├── fig-availability.png       # 2장·준비물 도식
│   ├── fig-5elements.png          # 3장 도식
│   ├── fig-verify-flow.png        # 7장 도식
│   └── cover-illustration-*.png   # 표지 삽화 원본 (중간 산출물)
├── 2026-10-10_topic1_sources.md    # 조사 노트 (근거)
└── 2026-10-10_topic1_curriculum.md # 교재 설계서 (근거)
```

## 위키독스 업로드 담당자를 위한 안내

- pages/의 16개 파일을 위키독스 페이지 순서대로 업로드한다.
- 이미지 경로는 상대 경로(../assets/)를 사용했다. 위키독스 업로드 시 이미지 첨부 방식에 맞게 조정한다.
- 붙여넣기 후 제목, 표, 코드 블록, 내부 링크, 모바일 가독성을 검수한다.

## 최신 정보 갱신 지점

기능과 화면은 변경될 수 있다. 다음 지점을 주기적으로 확인한다.

1. O2 공식 도움말의 지원 범위 (플랜별 모델, 미지원 범위, 설정 범위)
2. 순차 배포 완료 여부 (2장, 준비물 페이지의 서술)
3. 업데이트 기준일 (판권 페이지, references.md, qa_report.md)

갱신 시에는 해당 원문을 직접 열어 확인하고, 접근일을 함께 기록한다.

## 수정 방법

- 장별 수정: chapters/의 해당 파일을 고친 뒤, pages/의 대응 파일에 동일 내용을 반영한다 (현재는 복사본).
- 전체 수정: manuscript_full.md는 조립 산출물이므로 직접 고치지 말고, 원본(pages/, chapters/)을 고친 뒤 다시 조립한다.
- 표지·도식 수정: /tmp/make_diagrams.py와 /tmp/make_cover2.py는 임시 파일이므로, 재생성이 필요하면 스크립트를 다시 만들어 실행한다.
