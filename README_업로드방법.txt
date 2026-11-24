[알바 영수증 · 단일 공유 주소 / 최종 완료자만 집계]

공식 공유 주소 (한 개만 사용):
https://gjrie432-blip.github.io/alba-receipt-final/

GitHub 저장소:
https://github.com/gjrie432-blip/alba-receipt-final

업로드 순서:
1. ZIP 압축 풀기
2. 위 저장소의 최상위(root)에 index.html, alba-receipt-share.png 두 파일 업로드
3. 이미 같은 이름의 파일이 있다면 교체한 뒤 Commit changes
4. Settings → Pages → main / (root) 배포 상태를 확인
5. 기존 공식 주소 그대로 사용 (새 링크 만들 필요 없음)

참여자 집계 규칙:
- 링크 접속: 숫자 증가 안 함
- 시작 버튼, 목표 입력, 첫 번째 목표 영수증: 숫자 증가 안 함
- 최종 '목표+근무 계획 영수증'이 화면에 나타날 때: 1회 증가 요청
- 기존에 집계된 동일 브라우저에서는 다시 증가하지 않음
- 하나의 공식 링크만 사용하며 ?preview=1로 분리하지 않음
- 공유 썸네일 og:image는 alba-receipt-final 저장소의 PNG 파일을 가리킴
- 기존 완료자 수 Abacus namespace 유지. 새로 0으로 초기화하지 않음
- 일부 브라우저/기기/카카오톡 내장 브라우저는 로컬 저장공간이 분리될 수 있음
- 집계 서버 실패 시 성공으로 표시하지 않고 사용자에게 상태를 알려 줌
- HTTP 429(요청 제한)는 자동 재시도. 응답 유실 등 상태가 불명확한 실패는
  자동으로 재전송하지 않음. 이 API는 중복 없는 정확한 1회 전송을 보장하지 못함.
- 이미 누락된 과거 참여를 자동으로 복구하지는 못함.
- HTML 로컬(file://) 실행은 실제 사용자 집계에서 제외됨.

파일 구성:
index.html : 웹사이트 및 완료자 집계 로직
alba-receipt-share.png : 카카오톡 링크 미리보기 이미지
README_업로드방법.txt : 설명용, 업로드 불필요
