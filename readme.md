# japanese NER(Named Entity Recognition)

1. dictionary based NER
2. CRF NER
3. biLSTM CRF NER 
4. BERT NER

https://colab.research.google.com/github/JohnSnowLabs/spark-nlp-workshop/blob/master/tutorials/streamlit_notebooks/NER.ipynb#scrollTo=CGJktFHdHL1n


## 1번쨰 review

1. B I 합쳐서 점수 평가 통일
2. 에포크 충분한지 판단해서 결정하기 (loss graph 확인하면서, validation loss)
3. 오류분석
  + 오류 카테고리별로 나눠서 분석
  + 데이터 추가
  + 데이터가 어떤게 부족한지, 성능을 높이려면 어떻게 해야하는지, 어떤 종류의 데이터가 부족한지 분포 확인

4. BERT+CRF (Optional) 


## 2번째 review

1. 데이터가 제대로 학습되었는지 확인하기(전각, 반각 처리, 일본어 유니코드 특수문자)
2. BERT 결과 벤치마킹, 결과 비교, sota 조사
3. CRF feature함수를 바꿔가며 학습 비교
4. 도메인에 맞는 데이터를 모아서 태깅
5. 태그끼리 중복되거나 중의성은 없는지 확인해보고 레이블 합쳐보기
6. trainset, testset 데이터 개수를 확인할 수 있도록 표로 만들기
7. 실험을 진행할 때는 하나의 파라미터는 바꾸고 나머지는 동일하게 세팅해서 다양하게 진행
8. 학습 과정도 문제 없는지 확인해보기
