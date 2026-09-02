# 마케터 포트폴리오 웹사이트

프리랜서 전환을 준비하는 마케터를 위한 포트폴리오 웹페이지. 채용 담당자가 30초 안에 역량을 파악할 수 있는 구성을 목표로 했음.

강의 「Vibe Coding for DSMP」 2장 실습 산출물임. 클로드 아티팩트에서 PRD를 작성하고, 그 PRD를 기반으로 웹페이지를 구현한 과정 전체가 강의 노트에 정리되어 있음.

게시된 페이지: <https://logistex.github.io/marketerPortfolio/>

## 폴더 구성

| 경로 | 내용 |
|---|---|
| `마케터 포트폴리오 웹사이트 PRD/portfolio-prd.md` | 클로드가 작성한 제품 요구사항 문서. 8장 구성 |
| `마케터 포트폴리오 웹사이트 PRD/프리랜서 마케터 포트폴리오 웹사이트 PRD.pdf` | 같은 문서의 PDF 판 |
| `산출물/index.html` | 완성된 웹페이지. 단일 HTML 파일 |
| `산출물/게시된 포트폴리오.webloc` | 게시 주소 바로가기 |
| `index.html` | 루트 사본. 깃허브 페이지가 루트를 배포하므로 `산출물/index.html`과 같은 파일을 둠 |

루트의 `index.html`을 고칠 때는 `산출물/index.html`도 함께 고쳐야 두 벌이 어긋나지 않음.

## 만든 방법

| 단계 | 내용 |
|---|---|
| 1 | 5W1H를 갖춘 프롬프트로 PRD 작성을 요청 |
| 2 | PRD를 기반으로 HTML 뼈대를 만들고 섹션마다 고유한 id를 부여 |
| 3 | 실제 경력 데이터를 섹션별로 반영 |
| 4 | 워드프레스 Dorya 테마를 참고해 섹션별 색상 톤을 구분 |
| 5 | PRD 대비 검수 후 발견된 문제를 보완 |
| 6 | 깃허브 페이지로 배포 |

## 기술 구성

외부 프레임워크 없이 단일 HTML 파일로 만들었음. 인라인 CSS와 바닐라 자바스크립트를 씀. 빌드 과정이 없어 파일을 브라우저로 열면 그대로 동작함.

PRD 4.1절은 Next.js와 Tailwind CSS를 제안했으나, 구현 단계에서 단일 HTML 파일로 방향을 정했음. 강의 실습이라 설치와 빌드 없이 결과를 바로 확인하는 쪽을 택한 것임.

## 화면 구성

`nav-global`, `mobile-menu`, `section-hero`, `section-impact`, `section-about`, `section-projects`, `section-skills`, `section-testimonials`, `section-contact`, `footer-global` 열 개 영역으로 나뉨. 각 영역에 고유한 id가 있어 부분 수정을 지시하기 쉬움.
