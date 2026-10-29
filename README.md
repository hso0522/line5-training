# 5호선 기관사 학습 · 검수 완료본

2026년 10월 29일 검수 완료한 미리보기와 동일한 학습 내용입니다.

## 파일 구성
- index.html: 실행 파일. 화면·또타 이미지·선로도·애니메이션·응답 기능 포함.
- README.md: 배포 및 사용 안내.
- .nojekyll: 정적 페이지 배포 설정. 빈 파일이 정상입니다.

## 가장 간단한 교체 방법
1. ZIP을 다운로드하고 압축을 해제합니다.
2. 기존 GitHub 저장소의 Code 화면에서 Pages에 사용 중인 브랜치를 선택합니다(일반적으로 main).
3. Add file → Upload files를 누릅니다.
4. 압축을 푼 파일 3개를 저장소 최상위에 함께 올립니다. 같은 이름 파일은 새 버전으로 교체됩니다. 업로드 순서는 관계없습니다.
5. Commit changes로 저장합니다. 브랜치 보호로 직접 저장할 수 없으면 새 브랜치에 저장 후 PR을 병합합니다.
6. Settings → Pages에서 Deploy from a branch / main / /(root)을 확인합니다. 기존 배포 브랜치가 다르면 그 브랜치에 맞춥니다.
7. Actions에서 배포 성공을 확인한 뒤 기존 사이트 주소를 엽니다. 이전 화면이 보이면 Ctrl+F5로 새로고침합니다.

ZIP 파일 자체나 바깥 폴더를 올리지 말고, index.html이 배포 폴더 바로 아래에 오게 하세요.

## 기존 파일을 먼저 삭제하려는 경우
1. Code → Download ZIP으로 기존 저장소를 백업합니다.
2. 교체할 기존 index.html을 엽니다.
3. 우측 상단 … → Delete file → Commit changes를 선택합니다.
4. 기존 README.md와 .nojekyll도 제거하려면 같은 방식으로 삭제합니다.
5. 저장소 최상위로 돌아가 Add file → Upload files에서 새 파일 3개를 올리고 Commit changes합니다.

삭제부터 새 배포 완료까지 사이트가 잠시 열리지 않을 수 있습니다. 같은 이름으로 바로 교체하는 방법이 간편합니다. 저장소 자체는 삭제할 필요가 없습니다. CNAME, .github 설정, 다른 프로젝트 파일은 삭제하지 마세요. 이번 버전은 별도 이미지·CSS·JS 폴더 없이 실행되므로 구버전 전용 파일은 새 사이트 작동 확인 후 정리할 수 있습니다.

## 사용 안내
- 고덕 사례: 상황 재생 → 신호 확인 불가 시 조치 입력 → 답변 → 다음 장면 재생 → 훼손 후 조치 입력 → 문제점 및 기관사 조치요령 → 완료 배지.
- 관제원 또타는 밝은 초록색이며 원본의 웃는 표정을 유지합니다.
- 운전실 교환은 열차 내부 통로 이동으로 표현합니다.
- 해설·기관사·관제원 음성을 각각 선택할 수 있습니다. 음성이 끝나면 여유 시간을 두고 다음 장면으로 전환합니다.
- 음성은 기기/브라우저가 제공하는 한국어 합성 음성을 사용합니다. 한국어 음성이 없으면 음성 없이 진행합니다. 특정 연령·성별·성우 품질을 보장하는 녹음 음성은 아닙니다.
- 학습 도우미는 핵심어 기반 예시 응답입니다. 외부 AI에 연결되지 않았으며 모든 자유서술 답변을 정확하게 채점하는 기능은 아닙니다.
- 배지는 같은 브라우저에 저장됩니다. 브라우저 데이터를 지우면 배지도 삭제됩니다. 작성한 대화는 새로고침 시 초기화됩니다.
- Pretendard 글꼴은 CDN에서 로드하며 실패하면 시스템 글꼴로 표시합니다.

## 배포 참고
https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository
https://docs.github.com/en/repositories/working-with-files/managing-files/deleting-files-in-a-repository
https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
