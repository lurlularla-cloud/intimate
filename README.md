# 🌸 여성청결제 시장 분석 & 상세페이지 리뉴얼 인터랙티브 대시보드
> **(Feminine Wash Market Intelligence & Conversion Strategy Dashboard)**

올리브영 및 D2C 상위 18개 주요 브랜드(기준 제품: 라엘 포함)의 상세페이지 전수 벤치마킹 데이터, 2x2 포지셔닝 맵, 6대 요소 비교 매트릭스, Top-to-Bottom Storyline 전개 순서 및 라엘 리뉴얼 전략을 제공하는 인터랙티브 대시보드 프로젝트입니다.

---

## 🚀 배포 링크
- **라이브 대시보드 (Streamlit Cloud)**: [Streamlit Cloud 배포 링크](https://share.streamlit.io/deploy?repository=lurlularla-cloud/intimate&branch=main&mainModule=app.py)
- **GitHub 저장소**: [https://github.com/lurlularla-cloud/intimate](https://github.com/lurlularla-cloud/intimate)

---

## 📊 주요 기능 및 대시보드 구성

| 탭 메뉴 | 핵심 제공 기능 | 시각화 도구 |
| :--- | :--- | :---: |
| **Top KPI 카드** | 총 분석 브랜드(18개), 평균 실판매가, 100ml당 단가, 99.9% 항균 소구율, 유익균 채택율 | Metric Card |
| **Tab 1. 시장 개요 & 가격 분석** | 브랜드별 판매가 바 차트 및 용량 대비 100ml당 단가 버블 차트 | Plotly (인터랙티브) |
| **Tab 2. 2x2 포지셔닝 맵** | 4대 시장 클러스터 산점도 및 Next White Space, 라엘 Next 목표 이동 경로 | Plotly 2x2 Matrix |
| **Tab 3. 18개 브랜드 전수 비교 매트릭스** | 라엘 최상단 고정 및 18개 전 브랜드 6대 핵심 요소 상세 카드 연속 뷰어 | Interactive Table & Cards |
| **Tab 4. 상세페이지 Storyline 비교** | 브랜드별 5단계(Hero 후킹 ──► 문제 공감 ──► 솔루션 ──► 임상 ──► 가치 락인) 플로우 | Storyline Table |
| **Tab 5. 라엘(Target) 리뉴얼 마스터 플랜** | 4대 결핍 vs 해결책, 3대 컨셉 Before/After 헤드카피, 7개 섹션 풀 와이어프레임 | Tabs & Accordion |

---

## 📁 디렉토리 구조

```
intimate/
├── app.py                     # Streamlit 대시보드 메인 애플리케이션
├── requirements.txt           # 패키지 의존성 목록
├── .streamlit/
│   └── config.toml            # Streamlit 테마 및 서버 설정
├── generate_excel.py          # 18개 제품 13개 컬럼 비교 엑셀 생성기
├── generate_pptx.py           # 10장 고화질 발표 슬라이드 생성기
├── merge_reports.py           # 18개 분석 리포트 단일 통합기
├── data/                      # 18개 브랜드별 수집된 JSON 원본 데이터
├── report/                    # 분석 보고서, 엑셀, PPTX 최종 산출물
│   ├── all_products_analysis_integrated.md  # 18개 전 제품 통합 리포트
│   ├── competitor_comparison.xlsx          # 18개 제품 상세 비교 엑셀
│   ├── market_analysis_and_strategy.pptx   # 10장 프레젠테이션 슬라이드
│   ├── comprehensive_market_comparison.md  # 5단계 종합 마스터 플랜
│   ├── gap_analysis_and_copy_strategy.md   # 4단계 결핍 분석 & 카피 전략
│   ├── competitive_matrix_analysis.md      # 3단계 6대 요소 종합 매트릭스
│   ├── market_positioning_map.md           # 2단계 2x2 포지셔닝 맵
│   └── target_rael_analysis.md             # 1단계 라엘 기준 프로파일링
└── images/                    # 상세페이지 주요 섹션 캡처 이미지
```

---

## 💻 로컬 실행 방법

```bash
# 1. 패키지 설치
pip install -r requirements.txt

# 2. Streamlit 대시보드 실행
streamlit run app.py
```
브라우저에서 `http://localhost:8501`로 접속합니다.
