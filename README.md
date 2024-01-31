
## 브랜드 이미지 키워드 추출 서비스 프로젝트 

- 광고주들을 위한 인물/브랜드의 이미지와 관련된 키워드 및 특성 추출 서비스
- 멀티캠퍼스 Bootcamp semi 프로젝트
- 기간 : 2023년 7월 (팀 6인)

## Summary
**1. Image Keyword dictionary**
  - Dictionary : [KKM](http://kkma.snu.ac.kr/statistic)에서 브랜드 이미지 관련 단어만 분리 (형용사VA, 어근XR) 하여 말뭉치 사전 구축
  - Nominalization : 추출 키워드 명사화 

**2. Brand top20 Keyword Extraction**
  - Data Collection : ex. 블랙핑크, 뉴진스의 3개월 (2023.6~8월) 기사/블로그 크롤링 
  - Keyword Extraction : TF-IDF 활용 인물/브랜드 별 top20 키워드 추출

**3. BPS analysis**
  - BPS Similarity : BPS(Brand Personality Scale) 에서 규정된 5개 브랜드 이미지와 top20 Keyword 간의 유사도를 분석
    ```
    sincerity = ["정직함","다정함","건전함","친근함","진실함","본래의","사실의"]
    excitement = ["과감함","멋짐","상상력있음","독특함","유행선도적임","젊음","현대적임"]
    competence = ["성공적임","믿음직함","지적임","안전함","전문적임","선두의"]
    sophistication = ["매력적임","여성스러움","우아함","화려함","부드러움"]
    ruggedness = ["거침","남성적임","외향적임","튼튼함"]
    ```
  - Visualization : ex. 뉴진스 vs 블랙핑크 BPS 분석 비교 그래프 

## Environment
- Google Colab / Google Drive
- OS: Ubuntu 18.04.4 LTS (GNU/Linux 4.15.0-162-generic x86_64)
- Environment: Anaconda 4.10.3
