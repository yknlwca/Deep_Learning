### Attention
* Hidden States -- Hidden 계층
* seq2seq + attention

### Sequence to sequence
* 입력된 정보에서 추출된 정보들을 하나의 벡터로 만듬
* Sequence to sequence ATTENTION모델
* 모든 각각에 셀에 있는 hiddenstates가 다 넘어감
* encoder 쪽에서 decoder쪽으로 모든 스텝에 해당하는 hidden states가 넘어간다
* encoder에서 전달받은 전체 hidden states를 확인한다 -> 각각의 hidden state는 이전단어에 대한 입력단어에 대한 정보도 있고
* 현재 단어에 대한 입력 정보도 있는데 이러한 hidden state마다 점수를 계산한다 -> 계산된 점수에 대해 softmax를 취하고 각각의 벡터하고 연산을 취함 -> 어느 단어에 집중해야할지 나옴

### Context vector
* 실수형태의 값들이 저장되어있는 벡터 : 압축되어있는 정보

### Self - Attention
* 다른 단어들과의 관계 살펴보는 단계 그 후 신경망으로 입력

### Encoder 
* 전체 입력되어지는 문장에대한 의미
* encoder-> context벡터 출력 -> decoder ->기계번역
* encdoer 와 decorder에서는 모두 RNN 구조를 사용(hidden_stats)

### Transfomer
* 현재시점에 처리를 하고 있는 단어에 연관이 있는 단어를 Understanding 시켜줌(Self-Attention 이용)

### Self-Attention Detail
* Query Vector - Key Vector - Value Vector
* Enbedding 백터보단 차원은 작음.
* ex) 512 차원 -> 64차원
