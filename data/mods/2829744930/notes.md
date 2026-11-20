## 메모

- **유닛을 추가하지 않고 기존 것을 고친다.** 바닐라 텍스트 파일 51개의 내용이 다르다: `set/target` 16개(표적·탄 선택 규칙), `set/stuff` 14개, `entity/-vehicle` 13개, `set/vision` 3개 등. 유닛 파일로는 차량 12개, 아이템 14개, 보병 2개다.
- **새 파일은 주로 날씨다.** 새 텍스트 파일 58개 중 55개가 `set/environment` 아래다. 설명의 날씨 전환 기능과 맞는다.
- **새 구성 10행, 블록 이름 6종.** 패널 버튼 3개(`ai_auto_move`, `medic_switch`, `weather_switch`), 발각 항목 2개(`firing_binocular`, `firing_searchlight`), `look_around`.
- **새 따옴표 이름 101개.** 날씨 설정과 표적 규칙에 넣은 이름이다.
- **풀리지 않은 구문 1개 파일.** 바닐라에도 있는 `%door2`다.
- **스크립트 기능은 이 분석에 잡히지 않는다.** 자동 포격·자동 위생병 같은 기능은 맵에 심는 스크립트로 구현된다고 설명에 적혀 있다. 맵 파일은 범위 밖이다.
- **다른 모드와 겹치는 파일.** MACE와 6개(`set/panel_control/right_main.set`, `right_special.set`, `set/target/ammo.set`, `set/vision/settings.set`, `set/vision/spotting.inc`, `set/stuff/shell/bulletger_105.heat.ammo`), Fusion과 1개(`set/stuff/special/searchlight`). 모두 내용이 다르므로 로드 순서에 따라 한쪽의 변경이 사라진다.
- **2026-11-12·2026-11-18 갱신(창작마당 2026-11-19).** `resource` 안에서 바뀐 것은 `map.pak`뿐이다(분석 범위 밖). 모드 폴더의 `修改记录.txt`: 11-12판은 게임 2026-10 업데이트에 맞춰 단일 미션 15개와 새 미션 6개의 `.mi`, 멀티 공통 `inc` 8개(`frontlines` 1v1~4v4, `am/bz/dcg/ev_triggers`), `skirmish_logics.inc`를 바닐라 최신판으로 다시 만들고 자기 트리거 include와 AI 제외 태그를 다시 넣었다. 11-18판은 게임 Update 71에 맞춰 단일 미션 6개, `dcg_script.inc`, `skirmish_logics.inc`를 고치고 스커미시 5개의 `.mi` 덮어쓰기를 지웠다. `mod.info`의 `maxGameVersion`이 `"any"`에서 `"1.069.0"`이 됐다. 이 모드가 이기는 맵은 스폰 모드가 사본을 만들므로 갱신되면 `spawn-menu build`를 다시 한다(2026-11-20 대조: 사본 22개가 옛 판이었다).
