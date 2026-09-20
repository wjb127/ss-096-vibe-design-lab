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
