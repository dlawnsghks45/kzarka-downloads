# 크자카 오버레이 · KZARKA OVERLAY

공식 소개 및 다운로드: https://dlawnsghks45.github.io/kzarka-downloads/

버전별 변경 사항: [업데이트 노트](https://dlawnsghks45.github.io/kzarka-downloads/?view=updates)

Windows 설치 파일은 [Releases](https://github.com/dlawnsghks45/kzarka-downloads/releases)에서 제공합니다. 이 저장소에는 공개 홈페이지의 빌드 결과와 배포 안내만 보관합니다.

최신 버전은 [0.1.24](https://github.com/dlawnsghks45/kzarka-downloads/releases/tag/v0.1.24)입니다. **앱은 Discord 로그인이 필수입니다.** 공식 서버 `https://kzarka-overlay.onrender.com`을 통한 공개 0.1.0 패키지의 실제 소유자 로그인, 개인 기록 API 접근, 앱 재시작 시 로그인 복구와 로그아웃을 확인했습니다. 0.1.1 패키지도 네이티브 화면에서 실제 로그인, 암호화된 인증 정보 저장과 로그아웃을 확인했습니다. 일반 사용자는 기록 서버나 업데이트 주소를 입력·변경하지 않으며 앱에 포함된 공식 주소를 사용합니다. 로그인 화면에서도 앱 업데이트를 확인할 수 있습니다.

**0.1.5·0.1.6 업데이트 실패 복구:** 앱을 종료한 뒤 0.1.7 설치 파일을 기존 설치 위치에 한 번 덮어 설치해 주세요. 앱 제거는 필요 없으며 기록·설정을 유지합니다. 이전 업데이트 기능이 앱 묶음 파일을 잘못 읽는 오류가 있어 스스로 수정 코드를 받을 수 없습니다. 0.1.7은 실제 파일을 읽도록 수정했으며 창 없는 Electron 환경에서도 검사합니다.

0.1.6은 거래소에 없는 잡템의 상점 판매가가 미확인으로 남던 문제를 수정하고 아프로돈·아레시온 등 누락된 에다니아 사냥터 6곳을 추가합니다. 업데이트 후 로그인하면 본인 실전 기록의 빠진 가격을 다시 확인하며, 기존 가격·직접 입력한 값·사냥 시간·공개 여부를 유지합니다. 여러 사냥터가 섞인 과거 기록은 지역을 추측하지 않습니다.

복구한 0.1.7부터 후속 업데이트는 변경된 데이터 조각을 받고 검증된 새 버전으로 전환합니다. **업데이트하기 → 확인** 후 세션을 저장·종료하고 설치 프로그램 없이 다시 시작합니다. 0.1.4 이하도 최신 설치 파일을 사용해 주세요. 새 버전이 로컬 시작을 완료하지 못하면 다음 실행 때 이전 정상 버전으로 복구합니다. 설치 파일은 신규 설치와 복구용으로 계속 제공합니다. 사용 중인 Windows 앱의 두 버전 간 재시작은 이번 작업에서 실행하지 않았습니다.

Neon 데이터베이스의 실제 TLS 연결과 스키마 적용, 소유자의 웹 세션 인증도 확인했습니다. 원격 기록 저장·재조회·공유와 두 버전 간 업데이트 설치는 아직 검증하지 않았습니다. 홈페이지는 공식 기록실 링크와 실제 게임을 읽지 않는 웹 체험을 제공합니다. 한국어·영어, 사냥 아이템과 수익 오버레이, 한국 서버의 다음 두 보스 시간, 설정 가능한 단축키를 제공합니다.

0.1.1은 배포 앱의 개발자 도구·외부 원격 디버깅을 제한하고 수집 파일의 무결성을 확인합니다. 최종 패키지의 Electron fuse 5개, PE에 포함된 ASAR 해시와 수집 파일 949개의 무결성 목록 일치를 확인했으며 보호 검사 16개가 통과했습니다. 공개 0.1.1 다운로드·업데이트 피드의 HTTP 200 응답과 해시 일치, 실제 0.1.0 앱의 새 버전 감지·사용자 동의 다운로드·SHA-512 검증·로그인 전 설치 버튼 표시까지 확인했습니다. 설치는 실행하지 않았습니다. 이러한 검사로 완전한 분석 방지나 백신 무검출을 보장하지 않습니다.

설치 파일은 현재 코드 서명되지 않았습니다. Windows 게시자·평판 경고와 백신 탐지는 서로 다른 판정이며, 무경고·무검출을 보장하지 않습니다. 배포 파일의 SHA-256은 각 릴리스에서 확인할 수 있습니다. 보안 프로그램 해제나 예외 등록을 요구하지 않습니다.

실제 게임 수집 정확도와 운영사 허용 여부는 별도 검증이 필요합니다. 검은사막의 공식 제품이 아니며 게임 관련 이미지·명칭의 권리는 각 권리자에게 있습니다. 보스 이미지 출처는 `bosses/SOURCES.md`에 기록합니다.

**0.1.23 — 스킬 캐시 직업 추정과 경험치 OCR:** 저장된 스킬로 직업과 가능한 전승·각성을 추정합니다. 검은사막 게임 창의 제한된 영역에서 사냥 중 60초(선택 30초) 간격으로 레벨·경험치%를 읽고, 증가분을 대시보드·기록·기존 사냥 오버레이와 OBS 사냥 소스에 표시합니다. 캐시는 현재 캐릭터나 프리셋의 확정 근거가 아니며, 경험치는 절대 EXP가 아닌 레벨·퍼센트 기준입니다. 전리품 드롭은 기존 패킷 수집을 유지하며 저장된 사냥 목표와 기록을 보존합니다. 실제 게임 정확도와 FPS는 아직 측정하지 않았습니다.

**0.1.23 — Saved-skill class estimates and experience OCR:** Estimate class and supported specialization from saved skills. During hunting, read level and experience percentage from a bounded Black Desert window region every 60 seconds (optionally 30), and show gains in the dashboard, records, existing hunt overlay and its OBS source. Cached skills do not confirm the current character or preset; experience uses level and percentage rather than absolute XP. Loot drops still use packet collection. Saved hunting goals and records are preserved. Live accuracy and FPS have not been measured.

**0.1.24 — PaddleOCR 경험치 판독과 사냥 표시 수정:** 경험치 판독에 공개 PP-OCRv6 tiny 검출 모델과 PP-OCRv5 한국어 인식 모델을 독립적으로 적용합니다. 검은사막 전면 창의 작은 레벨·경험치 영역만 숨긴 CPU 프로세스에서 기본 60초(선택 30초) 간격으로 읽습니다. 아그리스 활성 표시는 제거하고 패킷으로 확인한 소모량을 유지합니다. 다른 게임 TCP 연결의 변화로 유지 중인 사냥 연결의 경험치 기준값과 분할 프레임이 초기화되던 문제를 수정합니다. 전리품·추정 처치는 패킷을 유지하고 OCR 퍼센트 증가를 처치 수로 환산하지 않습니다. 경험치 요약은 기존 사냥 오버레이와 OBS 소스에 표시하며 저장된 목표·기록과 계정 보호를 유지합니다. 실제 게임 판독 정확도·FPS·현재 사냥의 추정 처치 증가는 아직 확인하지 않았습니다.

**0.1.24 — PaddleOCR experience reading and hunt display fixes:** Use independently obtained public PP-OCRv6 tiny detection and PP-OCRv5 Korean recognition models. Read only the foreground Black Desert window’s small level and EXP region in a hidden CPU process every 60 seconds (optionally 30). Remove the Agris activation display and preserve packet-derived consumption. Preserve the existing hunting connection’s XP baseline and partial frames when another game TCP connection changes. Loot and estimated kills remain packet-based; OCR percentage gains are not converted into kills. Experience summaries remain in the existing hunt overlay and OBS source, with saved goals, records and account protections preserved. Live reading accuracy, FPS and estimated-kill increases in the current hunt have not been verified.
