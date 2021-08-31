# PE-Program
### 주제: 코로나•주식 연관 Youtube 뉴스 영상 댓글 분석

### 목차
0. 수집 데이터
1. 단어 빈도 분석, 워드클라우드 시각화
2. 연관 분석, 네트워크 시각화
3. 주식 종목 시세 예측 알고리즘 구현
4. 소스코드


### 0️⃣ 수집 데이터
| 구분 | 내용 |
| :- | - | 
| 유튜브 채널 | 한국 뉴스 채널 4곳(SBS News, KBS News, JTBC News, YTN News)
| 주제 | 코로나•주식 연관 뉴스 영상
| 영상 개수 | 50
| 댓글 개수(raw data) | 14023

- 영상 선정 기준
1. 영상 업로드 날짜 기간: 2020.07 ~ 2021.07
2. '코로나 주식' 검색어 지정, 주제와 관련성 높은 영상순으로 선정
- 데이터 수집 방법
[포스팅](https://velog.io/@ally0526/2.-Youtube-Data-Tool로-영상-댓글-수집하기) 참고


### 1️⃣ 단어 빈도 분석, 워드클라우드 시각화
| 라이브러리 & 패키지 | 용도 |
| :- | - | 
| Konlpy | 텍스트 데이터 처리
| Hannanum | 형태소 분석, 명사 분석
| Counter | 빈도 분석
| Wordcloud | 워드클라우드 시각화

- 워드클라우드 결과물


![](https://images.velog.io/images/ally0526/post/46734be5-1aef-4494-90e1-44fcffd4ff43/image.png)


### 2️⃣ 연관 분석, 네트워크 시각화
| 라이브러리 & 패키지 | 용도 |
| :- | - | 
| Konlpy | 텍스트 데이터 처리
| Hannanum | 형태소 분석, 명사 분석
| Counter | 빈도 분석
| Networkx | 네트워크 시각화

- 연관 분석 규칙 생성

| source | target | support
| :- | - | - |
| 코로나 | 사람 | 0.333333
| 코로나 | 주식 |0 .333333
| 코로나 | 코인 |0 .333333
| 코로나 | 투자 |0 .333333
| 코로나 | 코인 |0 .333333



### 3️⃣ 주식 종목 시세 예측 알고리즘 구현
| 라이브러리 & 패키지 | 용도 |
| :- | - | 
| Keras | 모델 훈련
| Matplotlib | 그래프 시각화

- 데이터 수집: [야후 파이낸스](https://finance.yahoo.com)
- 그래프 시각화 결과
![](https://images.velog.io/images/ally0526/post/c2e43e42-7016-41c8-83ab-4ed0900baddd/image.png)



### 4️⃣ 소스코드
[깃허브 레포지토리](https://github.com/HyunJin0505/PE-Program)

------
참고 레퍼런스
[이것이 데이터분석이다 with 파이썬 (한빛미디어)](https://www.hanbit.co.kr/store/books/look.php?p_code=B2717499992)


[주식•비트코인 시세 예측하기](https://opentutorials.org/module/3811/22947)


[딥러닝을 이용한 자연어처리 입문](https://wikidocs.net/book/2155)





