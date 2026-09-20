# 2026-09-20

렌즈: 데이터 테이블 / dense admin UI

## 레퍼런스
- Salt Design System — Density  
  https://www.saltdesignsystem.com/salt/foundations/density  
  named mode (high | medium | low). medium 기본. high는 기본값 금지(타깃 크기).
- Setproduct — Data table UI design  
  https://www.setproduct.com/blog/data-table-design  
  필터 칩, select-all 범위, sticky/frozen, sort 방향.

## 기법
1. density-mode-contract → `density.html`  
   compact | comfortable | spacious. 화면 단위 하나. 기본 comfortable. persist. compact는 a11y 고지. spacing/type만 바꿈. hit 24px 유지.
2. active-filter-truth → `filters.html`  
   칩 + 전체 N건 중 M건 + 전체 해제 + sort 방향. select-all은 페이지 vs 일치 전체. 필터/정렬은 전체 집합 기준.

## 오늘 범위
기법당 화면 하나. 프레임워크 없음.

---

# 아침 브리핑 — 설정 · progressive disclosure

## 레퍼런스
- 137Foundry — Settings that scale  
  자주 쓰는 것만 먼저, Advanced로 긴꼬리, ~20개 넘으면 검색
- Carbon — Disclosures  
  https://carbondesignsystem.com/patterns/disclosures-pattern/  
  사용자 개시, 한 번에 하나, 중첩 금지, 중요 정보 숨김 금지
- 케이스: Zoom App settings — 빈도 재배치, Advanced, 결과/상태 라벨

## 기법
3. common-first-disclosure → `common.html`  
   고빈도만 기본. 고급 한 겹. 그룹은 이름만. 입장용 카메라/마이크는 숨기지 않음. 20+면 검색(라벨·설명·동의어).
4. risk-tiered-save → `save.html`  
   저위험 자동저장 / 필드 인라인 / 구역 저장 / 긴 폼 스티키+이탈경고 / 위험 구역은 확인+결과 카피. 로딩·성공·실패·권한 잠금.

---

# 미학 + 인터랙션

## 레퍼런스
- Pika https://pika.style/templates/screenshot-editor → `pika.html` (Gleam)
- Raycast https://www.raycast.com/ → `raycast.html` (Flint)
- Family https://family.co/ → `family.html` (Sunday)

로고 복제 없음. 톤·플로우만.

---

# v4 — 화면 타입 안 겹침

- Cosmos https://www.cosmos.so/explore → `cosmos.html` (Grove) 메이슨리·컬러칩·디테일
- Craft https://www.craft.do/ → `craft.html` (Linen) 커버·/블록·todo
- Pitch https://pitch.com/ → `pitch.html` (Stage) 필름스트립·테마·Present
