* Bag of Words Meets Bag of Popcorns
NLP 관련 Kaggle Projects 중 하나로, 영화 리뷰를 작성하는 IMDB 웹사이트의 리뷰의 sentiment 를 학습하고 예측하는 과제입니다. Kaggle 에 tutorial 이 제공되어있어 초보자에게 좋은 과제라고 알려져 있습니다. (https://www.kaggle.com/c/word2vec-nlp-tutorial)

** 참고한 자료
- Kaggle tutorial
- 박조은 님의 깃헙 (https://github.com/corazzon)

** 소감
본 과제는 주어진 언어 corpus 를 어떤 형식의 input 으로 만들어 학습시킬 것인지를 배우는데 좋은 것 같습니다.
part 1 에서는 BOW (Bag of words)을 사용하여 review 에 사용된 단어의 갯수로 구성된 벡터를 사용하여 학습하며,
part 2 는 word2vec embedding matrix 를 만들고 reveiw 별 embedding vector average 를 구하여 학습합니다.
part 3 는 word2vec embedding vector 를 바탕으로 clustering 한 후에 cluster index 로 BOW 와 비슷한 작업을 하여 학습시킵니다.

part 1~3 모두 review 단어간의 연관관계를 분석하기보다는, 단어 벡터(클러스터)의 조합으로 분석을 하기 때문에 한계가 정확도가 높지 않습니다. embedding vector 로 LSTM 모델을 만들어서 sentiment 를 학습하는 것을 시도해봐도 좋을것 같다는 의견!
