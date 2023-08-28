# Data repository📌
Data 저장소는 북극성 프로젝트의 채용공고 추천 및 강의 추천에 사용된 데이터의 수집 및 전처리를 수행하기 위한 목적으로 만들어졌습니다.  
팀원 개인별 폴더를 만들어 각자 담당한 출처에서 데이터를 수집하는 코드를 작성 및 실행하였으며, 지속적으로 상호 연락하며 보완하는 과정을 거쳐 데이터를 수집하고 처리하였습니다. 뿐만 아니라 수집한 데이터를 활용해 EDA, 형태소 분석, 단어 임베딩 등 Task에 활용해 볼 법한 사항들을 실험하기도 하였습니다.  
  
# Data Set📌
1. 채용공고 데이터(Wanted, Jumpit, Jobplanet)  
2. 강의 데이터(Udemy)  

(ERD그림)

# Data Preprocessing📌
채용공고 데이터는 기 훈련된 BERT 모델의 Domain Adaptation을 위한 MLM 방식 훈련에 사용하기 위하여 중복제거 및 전처리 과정을 수행하였습니다.  
강의 데이터는 매칭 알고리즘에 활용할 목적으로 데이터 형식 및 타입을 통일하고 결측치를 제거하는 등의 전처리 과정을 수행하였습니다.  
  
(데이터 처리 그림)  
  
형태소 분석을 통해 공고상 중복되어 등장하게 되는 의미없는 듯한 단어들(~하신 분, 경험 etc..)을 제거하여 Input으로 활용했을 때 성능을 비교해 보고자 하였습니다. 분석 및 불용어 선택까지는 진행이 되었으나 시간상 제약으로 모델학습 및 비교작업까지 진행하지는 못하였습니다.

# Libraries📌
1. Selenium, BeautifulSoup Pandas, Numpy, matplotlib, seaborn, Scikit-learn  
2. Konlpy(Okt, Mecab, Hannanum), nltk
3. Customized Konlpy

# Teammates📌
|곽찬혁|김재현|백승림|임태근|최인호|
|-----|-----|-----|-----|-----|
