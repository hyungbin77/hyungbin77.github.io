---
title: "KSP: Kolmogorov-Smirnov metric-based Post-Hoc Calibration for Survival Analysis"
collection: publications
category: conference
excerpt: "생존분석 모델의 예측 확률을 사후 보정하는 방법. 4저자로 실험 환경 구성과 실험 수행을 담당했습니다."
date: 2025-09-01
venue: 'NeurIPS 2025 (poster)'
citation: 'Jeongho Park, Daheen Kim, Cheoljun Kim, <b>Hyungbin Park</b>, Sangwook Kang, Gwangsu Kim. (2025). &quot;KSP: Kolmogorov-Smirnov metric-based Post-Hoc Calibration for Survival Analysis.&quot; <i>NeurIPS 2025</i>, poster.'
---

생존분석 모델이 산출하는 예측 확률을 Kolmogorov-Smirnov 통계량 기준으로
**사후 보정(post-hoc calibration)** 하는 방법입니다.
구간 분할(binning)이나 Kaplan-Meier 추정에 의존하지 않아 연속시간 설정에 그대로 적용됩니다.

**담당 역할** — Linux 실험 환경 구성 및 실험 수행 지원.
GPU 서버에 실험 환경을 구축하고 반복 실험을 돌려 결과를 정리해 전달했습니다.

## 참여한 실험 규모

생존모델 6종 × 임상 벤치마크 10종 = **60개 조합**, 각 조합을 서로 다른 시드로 30회 반복했습니다.

- **임상 데이터 10종** — MIMIC-III(중환자 EHR), SEER-liver · stomach · lung(암 등록자료),
  METABRIC(유방암), WHAS, GBSG, NACD, NB-SEQ, SUPPORT
- **생존모델 6종** — DeepSurv(Cox PH), MTLR, DeepHit, Survival CRPS, Weibull AFT,
  모수적 모형 (기준선으로 Kaplan-Meier)
- **평가 지표** — 판별력 C-index + 캘리브레이션 5종 (S-cal, D-cal, KS-cal, KM-cal, IBS)

생존분석은 임상 예후 예측의 표준 방법론이고, 캘리브레이션은 임상 예측모델 검증의 필수 절차입니다.
이 실험을 통해 임상 생존 데이터를 다루는 경험을 쌓았습니다.
