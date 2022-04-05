# Crawling
<h4> 프로젝트 진행 중 </h4>
  <p> 1. instagram crawling 완료 ( 전처리 및 dataframe화 ) </p>
  <p> 완료 : 날짜 위치 본문내용 해시태그 댓글 및 모든 답글  </p>
  <p> 답글 내용 @아이디, : 제거 후 대화 내용만 정제 </p>
    <br>
  <p> 2. instagram 이미지 고려 (crawling, 주요 객체 선택)  </p>
  <p> 완료 : 이미지 주요 색상 추출 (3개,kmeans clustering) / 이미지의 주요객체선택여부 opencv의 grabcut 알고리즘  </p>
   <br>
  <p> 3. TfidfVectorizer  LGBMClassifier 을 이용한 감성사전기반 감성분석 </p>
  <p> 완료 : 감성 예측  정확도 및 불용어 제거 </p>
    <br>
   <p> 4. Melon top 100곡 crawling 완료 ( 전처리 및 dataframe화 ) </p>
   <p> 완료 : 가사 정제 및 감성분석 Label </p>
   <p> 개선 : 가사 영어 -> 한글 번역
  
  <br>
  <br>
  
  ### 감성분석 개선점 
  #### 1. 
  0 | 1 | 2 | 3
---- | ---- | ---- | ----
기쁨 행복 | 분노 | 불안 당황 | 슬픔 상처
  <br>  
  ### AI허브 감성사전을 그대로 쓰는 것은 노래가사와 맞지 않을 수 있음. --> Word2vec 으로 가사를 태그화하여, 불용어 처리 및 노래가사 감정사전을 새로 구
