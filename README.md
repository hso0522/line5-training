# 5호선 신규기관사 상황 학습 — 초안

## 구성
- index.html: 실행 파일. 선로도·또타 이미지·상황 애니메이션·3D 확대·대화형 학습·핵심 정리 포함.
- .nojekyll: GitHub Pages에서 정적 파일을 그대로 제공하도록 하는 설정.
- README.md: 배포 안내.

## GitHub 업로드 및 배포 순서
1. ZIP을 내려받아 압축을 해제합니다. ZIP 자체를 업로드하지 않습니다.
2. GitHub에 로그인한 뒤 새 저장소를 만듭니다. 예: line5-training. 무료 공개 배포는 Public으로 만듭니다.
3. 저장소에서 Add file → Upload files를 누릅니다. 빈 저장소라면 uploading an existing file을 누릅니다.
4. 압축을 푼 폴더 안의 index.html, .nojekyll, README.md를 모두 선택하여 업로드합니다. 파일끼리 업로드 순서는 상관없습니다. 바깥 폴더째 올리지 말고 저장소 최상위에 파일이 보이게 올립니다.
5. Commit changes로 저장합니다. 기본 브랜치는 main을 사용합니다.
6. Settings → Pages → Build and deployment → Source에서 Deploy from a branch를 선택합니다.
7. Branch는 main, 폴더는 /(root)를 선택하고 Save를 누릅니다.
8. Actions에서 pages build and deployment가 완료됐는지 확인하고 Settings → Pages의 Visit site로 접속합니다.
9. 상황 재생, 112번 3D 모션 재생, 대화 입력, 핵심 정리 화면을 확인합니다.

## 업데이트
같은 저장소 최상위의 index.html을 새 파일로 교체하고 Commit changes를 누릅니다. Pages 설정은 다시 할 필요 없습니다.
기존 다른 사이트를 유지하려면 새 저장소를 사용합니다. 기존 저장소의 index.html을 교체하면 해당 사이트가 바뀝니다.

## 현재 구현 범위
- 112번 표시는 제공된 선로도의 분기점에 맞춘 버전입니다.
- 차륜과 선로전환기 훼손 장면은 단순화한 3D 개념 모션이며 MP4 동영상 파일이 아닙니다.
- 대화는 키워드 기반 예시 응답입니다. 외부 AI 모델과 연결되어 있지 않습니다.
- 음성은 브라우저/운영체제의 한국어 합성 음성을 사용하므로 기기에 따라 달라지거나 지원되지 않을 수 있습니다.
- 로그인, 서버 저장, 사용자별 학습 이력 저장은 없습니다.
- 선로도와 캐릭터 이미지는 실행 파일 안에 포함되어 별도 업로드가 필요 없습니다.
- 글꼴은 네트워크 연결 시 Google Fonts를 사용하고, 실패하면 시스템 글꼴로 표시합니다.

공식 배포 설명: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
