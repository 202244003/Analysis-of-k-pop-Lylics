# K-pop 가사 분석 프로젝트


### 프로젝트 설명 
이 프로젝트는 연도별 순위권 K-pop 가사를 분석하여 
가사에 포함된 한국어와 영어의 비율을 시대별로 시각화하고, 
시대별로 가장 많이 사용된 단어를 도출하는 것을 목표로 합니다. 

이를 통해 시대의 문화적, 언어적 변화를 탐구하며 
대중음악 가사에 나타난 언어적 트렌드를 이해하고자 합니다.

### 프로젝트 목표 및 기대 효과
#### 목표
- 시대별 노래 가사의 한국어와 영어 비율을 분석하고 시각화.
- 시대에 따른 가장 많이 사용된 단어를 도출하여 대중음악에서의 언어적 트렌드 변화 파악.
- 빌보드 차트 기록이 있는 k-pop 가사를 분석하여 영어 가사의 글로벌화 연관성 파악.
#### 기대 효과
- 대중음악의 언어적 변화를 통해 시대의 흐름과 글로벌화의 영향을 이해.
- 향후 음악, 언어, 문화 연구의 기초 데이터로 활용 가능.

### 프로젝트 진행 범위 및 방법

데이터 가공/정제 -> 데이터 분석 -> 데이터 시각화 -> 결과 도출

pandas 사용 데이터 가공/정제

python 사용 데이터 분석 (Counter (collections 모듈), Konlpy (한국어 형태소 분석) 등

Matplotlib, Seaborn 사용 데이터 시각화

### 프로젝트 주요 내용
#### 데이터 처리 및 분석
- 중복 제거 및 필터링 과정을 거쳐 총 4220개의 노래 데이터 확보
- 가사 데이터를 기반으로 단어 비율 및 단어 빈도 데이터프레임 생성
- 형태소 분석기를 이용한 한국어 및 영어 단어 분리.
- 불필요한 문자 제거 및 데이터 정규화.
#### 시각화 작업
- 시대별 한국어와 영어 가사 비율 연도 단위 시각화.
- 사용자가 선택한 연도의 상위 10개 단어 (한국어 및 영어) 시각화.
- 빌보드 차트 기록이 있는 k-pop 한국어와 영어 가사 비율 시각화.
- 생성된 모든 시각화 결과를 PNG 파일로 저장.

### 연구 결과물

#### 언어 비율 변화:
- 연도별 K-pop 가사에서 영어와 한국어 단어 비율을 비교한 결과, 영어 단어 사용 비율은 1990년대 후반부터 꾸준히 증가하는 경향을 보임.
- 2000년대 중반 이후 글로벌 시장 진출 전략과 맞물려 영어 사용 비율이 급격히 상승한 것으로 나타남.

#### 연도별 상위 단어 분석:
- 각 연도별로 가장 많이 사용된 한국어 및 영어 단어를 추출한 결과, 1990년대 이전에는 감성적인 표현(사랑, 마음, 눈물 등)의 한국어 단어가 우세한 반면, 이후 영어 단어는 Love, Baby 등 글로벌 음악에서 흔히 사용되는 단어가 빈번히 등장하기 시작함.
- 이는 K-pop이 해외 팬들과의 소통을 고려한 가사 작성을 하고 있음을 시사함.

#### 빌보드 차트 기록이 있는 k-pop 가사 분석 :
- 2009년 빌보드 Hot100 k-pop 최초 진입 *원더걸스 - Nobody*의 가사에서 영어와 한국어 단어 비율을 비교한 결과, 영어 단어 사용 비율이 54%로 한국어 사용량보다 많은 것으로 나타남.
- 2012년 빌보드 Hot100 2위 *싸이 - 강남스타일*의 가사에서 영어와 한국어 단어 비율을 비교한 결과, 영어 단어 사용 비율이 22.3%로 이례적인 사례로 나타남.
- 2020년 빌보드 Hot100 k-pop 최초 1위 *BTS-Dynamite*의 가사에서 영어와 한국어 단어 비율을 비교한 결과, 영어 단어 사용 비율이 100%로 k-pop 가사의 혁신적인 변화를 보여줌.


#### 데이터 활용 가능성:
- 음악 산업, 문화 연구, 언어적 변화 분석 등 다양한 분야에서의 활용 가능성을
제시함.	
- K-pop 가사의 언어적 변화와 글로벌 시장에서의 성공 간의 관계를 데이터로 입증하여, K-pop의 글로벌 전략과 문화적 변화를 이해하는 데 기여함.


#### 프로젝트 결과:
- 연도별 언어 비율 변화 그래프: ./result/kpop_english_ratio.png
- 연도별 상위 단어 그래프: ./result/Korean_Words_Ranking_{{연도}.png, English_Words_Ranking_{{연도}.png
-  빌보드 차트 기록이 있는 k-pop 분석 그래프: nobody_lyrics_english_ratio.png, gangnamStyle_lyrics_english_ratio.png, dynamite_lyrics_english_ratio.png 

### 프로젝트 소스코드 
Analysis-of-k-pop-lylics.ipynb

analysis-of-k-pop-lylics.py

### 프로젝트 결과물
![kpop_english_ratio](https://github.com/202244003/Analysis-of-k-pop-Lylics/blob/main/result/kpop_english_ratio.png)

연도별 언어 비율 변화 그래프


![English_Words_Ranking_2023.png](https://github.com/202244003/Analysis-of-k-pop-Lylics/blob/main/result/English_Words_Ranking_2023.png)

연도별 영어 상위 단어 그래프 (2023)


![Korean_Words_Ranking_2023.png](https://github.com/202244003/Analysis-of-k-pop-Lylics/blob/main/result/Korean_Words_Ranking2023.png)

연도별 한국어 상위 단어 그래프 (2023)


![nobody_lylics_english_ratio](https://github.com/202244003/Analysis-of-k-pop-Lylics/blob/main/result/nobody_lyrics_english_ratio.png)

빌보드 차트 기록이 있는 k-pop 분석 그래프 (원더걸스 - Nobody)

2009년 k-pop 최초 빌보드 Hot100 진입


![gangnamStyle_lylics_english_ratio](https://github.com/202244003/Analysis-of-k-pop-Lylics/blob/main/result/gangnamStyle_lyrics_english_ratio.png)

빌보드 차트 기록이 있는 k-pop 분석 그래프 (싸이 - 강남스타일)

2012년 빌보드 Hot100 2위

![dynamite_lylics_english_ratio](https://github.com/202244003/Analysis-of-k-pop-Lylics/blob/main/result/dynamite_lyrics_english_ratio.png)

빌보드 차트 기록이 있는 k-pop 분석 그래프 (BTS-Dynamite)

2020년 빌보드 Hot100 k-pop 최초 1위
