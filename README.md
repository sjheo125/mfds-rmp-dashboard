# MFDS RMP Dashboard

**▶ 대시보드 바로 보기: https://sjheo125.github.io/mfds-rmp-dashboard/**
(이 저장소 화면에서 HTML 파일을 누르면 소스 코드가 보입니다. 위 주소로 들어가세요.)

식품의약품안전처(MFDS) 위해성 관리계획(RMP), 의약품 심사결과, 급여 현황을 정리하고 미국 FDA REMS를 병기한 대시보드입니다.
Dashboards on Korea MFDS Risk Management Plans (RMP) and drug approvals, with FDA REMS shown side by side.

- 데이터 기준일 / Data as of: 2026-09-30 (FDA REMS: 2026-09-28)

## 대시보드

| 파일 | 내용 |
|---|---|
| `index.html` | RMP 대시보드 (사이트 첫 화면) — 한국 RMP ↔ 美 FDA REMS 비교 (위해성 항목, 재심사기간, ETASU 구분) |
| `MFDS_Integrated_Dashboard.html` | 심사결과 + 재심사/RMP + 급여 약가 + REMS 통합 |

각 HTML은 단독으로 열리는 정적 파일입니다. 차트는 Chart.js(CDN)를 사용하므로 인터넷 연결이 필요합니다.

## 데이터 출처

- 식품의약품안전처 의약품안전나라 (https://nedrug.mfds.go.kr)
- 건강보험심사평가원 약제급여목록 및 급여상한금액표 (2026.10.1. 기준)
- 미국 FDA REMS Public Dashboard (https://fis.fda.gov)

## 유의사항

- 공개 자료를 정리한 비공식 분석 자료이며 규제·임상·투자 판단의 근거가 아닙니다. 정확한 내용은 원 출처에서 확인하세요.
- 2025년 이후 허가 품목은 재심사 제도 변경으로 재심사기간이 없어 "해당사항 없음 (규정변경)"으로 표시합니다.
- 위해성 항목이 "-"인 품목은 식약처 RMP 요약서에 기재된 항목이 없다는 뜻이며, 위해성이 없다는 의미가 아닙니다.
- 한국 RMP와 FDA REMS는 영문 성분명으로 매칭했습니다. 단, 데노수맙은 FDA REMS가 Prolia 계열(60 mg 프리필드시린지, 골다공증)에만 있고 Xgeva 계열(120 mg 바이알, 골전이)에는 없어서 제품별로 따로 매핑했습니다.
  - 이잠비아→Conexxence, 스토보클로→Stoboclo, 오보덴스→Ospomyv, 주본티→Jubbonti (식약처 제형·규격·효능효과로 계열 확인)
  - 덴브레이스·엑스브릭·오센벨트는 Xgeva 계열이라 REMS 없음으로 표시
  - 이잠비아↔Conexxence는 HK이노엔이 맵사이언스에서 도입한 제품이라는 제조사 정보에 근거한 추정이며, 공식 확인된 매핑이 아닙니다.
