# QA 보고서 (qa_report)

검증일: 2026-10-10

## 링크 검증

| 링크 | 상태 | 비고 |
|------|------|------|
| https://openai.com/index/gpt-6-for-everyone/ | PASS | 2026-10-10 직접 열람. 발표일 2026-10-07 확인 |
| https://help.openai.com/en/articles/20001598-intelligent-ui-in-chatgpt | PASS | 2026-10-10 직접 열람. 플랜별 가용성·지원 범위 확인 |
| https://help.openai.com/en/articles/28360-chatgpt-release-notes | PASS | 검색 결과로 확인 |
| https://github.com/gongnyang/bookforge | 미확인 | PDF 빌드 단계에서 README 확인 예정 |
| https://open.kakao.com/o/s4OEqBai | 미확인 | 사용자가 제공한 단톡방 주소. 접속 테스트를 하지 않았다 |

## 사실 검증

- GPT-6 + Intelligent UI 2026-10-07 공개: PASS (O1 직접 확인)
- 유료 플랜부터, Free·Go는 10-08부터 순차 배포: PASS (O1 직접 확인)
- GPT-6 Sol(유료)·Luna(Free/Go): PASS (O1, O2 직접 확인)
- Pro 추론(Astra) 미지원, Instant~Extra High 동작: PASS (O2 직접 확인)
- Chat 탭 전용, Work·Codex·Voice·구형 데스크톱 앱 미지원: PASS (O1, O2 직접 확인)
- 사용자 지정 지침으로 스타일 안내 가능, 레이아웃 변경 가능: PASS (O2 직접 확인)

## 저작권·인용 검증

- 원문 PDF 허위 표기: PASS (없음. 웹 원문임을 명시)
- 원문 전체 무단 복제: PASS (없음. 독자적 문장으로 요약)
- 공식 스크린샷을 직접 촬영한 것처럼 사용: PASS (없음. 실제 화면 미확보로 명시하고 모식도 사용)
- 가상 데이터 표시: PASS (5장의 계산 예시에 가상 데이터임 명시)
- 커뮤니티 의견의 통계적 사용: PASS (없음. 정성 신호로만 언급)
- 이미지 권리: PASS (표지 삽화는 AI 생성 독창 이미지, 도식은 PIL 직접 제작)

## 원고 품질 검증

- Markdown 굵은 표시 사용: PASS (없음)
- 장식성 이모지: PASS (없음)
- 과장 표현(완벽 가이드·완전 정복 등): PASS (없음)
- 한글 폰트·깨짐: PASS (표지·도식 렌더링 직접 확인)
- 프롬프트 복사 가능 여부: PASS (fenced code 블록 사용)
- 각 장 최소 구성(개념·준비물·실습·프롬프트·성공/실패·FAQ·점검·확인문제·출처): PASS (8장 모두 포함)
- 미지원 환경 대체 경로: PASS (전 장에 포함)
- 개인정보·민감정보 포함: PASS (없음)

## 미완료 항목

- book.pdf: 미완료. Bookforge README를 확인했으나(2026-10-10), git clone이 네트워크 타임아웃으로 실패했고 Typst·PyMuPDF·markdown-it-py가 설치돼 있지 않아 빌드 불가. 임의로 통과 처리하지 않았다.
- 단톡방 링크 접속 테스트: 미실시 (사용자 제공 주소를 그대로 기재)
- 위키독스 붙여넣기 후 검수: 출판 담당자(타 AI)가 위키독스 업로드 시 수행
