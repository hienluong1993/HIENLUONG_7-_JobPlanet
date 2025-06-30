# 🛠️ 잡플래닛(JobPlanet) 기업 리뷰 및 평점 크롤러

**Selenium + BeautifulSoup** 기반으로 잡플래닛에서 **기업의 리뷰 수, 평점, 세부 평가**를 자동으로 수집하는 Python 크롤러입니다.

---

## 📌 주요 기능

✅ 잡플래닛 기업명 검색 → 기업 ID 추출  
✅ 기업 상세 페이지 진입 → 리뷰 수, 평점, 상세 평점 추출  
✅ `enterprise_df_10k_utf8_data.csv`에서 특정 담당자 기업 리스트 불러와 자동 진행  
✅ 에러 발생 시 에러 로그 파일 별도 저장  
✅ 진행상황 자동 주기적 저장 (`jobplanet_crawling_progress.csv`, `jobplanet_crawling_error.csv`)  
✅ 크롤링 재시작 시 이전 진행 내용 이어서 실행 가능  
✅ `tqdm`로 진행 상황 실시간 모니터링

---

## 🗂️ 폴더 구조 예시

📦jobplanet_crawler
┣ 📄 jobplanet_crawler.py
┣ 📄 enterprise_df_10k_utf8_data.csv
┣ 📄 requirements.txt
┣ 📄 README_kr.md

---

## ⚙️ 설치 방법

1️⃣ **Python 3.8+ 필요**  
2️⃣ 의존 라이브러리 설치:
```bash
pip install selenium beautifulsoup4 pandas tqdm
