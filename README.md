# M1-1 AI 데이터 분석: 데이터 기반 트렌드 분석

## 국내 자동차 제조업 생산활동 시계열 분석
KOSIS의 자동차 및 트레일러 제조업 월별 데이터를 활용하여  
2015년 1월부터 2026년 7월까지 생산능력과 가동률의 장기 추세, 변동성 및 계절성을 분석한 프로젝트

## 1. 주요 분석 내용

- 생산능력지수의 장기 추세 분석
- 가동률의 주요 상승·하락 시점 분석
- 월별 계절성 분석
- 가동률 원지수와 계절조정지수 비교
- 이동평균, 전월 대비 변화율, 표준편차 활용
- 가동률지수 시계열 분해를 통한 추세·계절성 분석

## 2. 프로젝트 구조

```text
M1-1/
├─ data/
│  ├─ automobile_manufacturing_indices_2015_2026.csv
│  └─ raw/
│     └─ KOSIS_제조업_생산능력_및_가동률지수_원본.csv
├─ images/
│  ├─ 01_production_capacity_trend.png
│  ├─ 02_utilization_major_changes.png
│  ├─ 03_monthly_utilization_pattern.png
│  ├─ 04_original_vs_seasonally_adjusted.png
│  └─ 05_utilization_decomposition.png
├─ analysis.ipynb
├─ REPORT.md
├─ README.md
└─ requirements.txt
```

## 3. 실행 방법

### 3-1. 개발 환경

- Python 3.10 이상
- Jupyter Notebook
- 주요 Python 라이브러리는 `requirements.txt`에 명시

### 3-2. 의존성 설치

프로젝트 루트에서 다음 명령 실행

```bash
pip install -r requirements.txt
```

### 3-3. Jupyter Notebook 실행

```bash
jupyter notebook
```

이후 `analysis.ipynb`를 열고 전체 셀을 순서대로 실행  
최종 제출 전 **Restart → Run All**을 통해 처음부터 마지막 셀까지 오류 없이 실행 확인  

## 4. 결과 리포트

상세한 분석 과정, 시각화, 인사이트 및 한계점은 [`REPORT.md`](REPORT.md)에서 확인

## 5. 데이터 출처

- **출처:** KOSIS 국가통계포털
- **분석 대상:** 자동차 및 트레일러 제조업
- **분석 기간:** 2015.01 ~ 2026.07
- **데이터 수:** 139개월
