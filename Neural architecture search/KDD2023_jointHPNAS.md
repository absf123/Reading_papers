### 240124
#### KDD'23 
#### 요약
1. Automated Machine Learning(AutoML) techniques는 Collaborative Filltering (CF) model를 data specific manner로 설계하는데 현재 사용되고 있다.
2. 하지만 기존 방법들은 architecture search를 할때 hyperparameter의 영향을 무시하고 진행한다 (fixed hyperparameter)
3. 그래서 우리는 reduced space에서 proper configurations찾아서 효율적으로 architecture와 hyperparameter의 joint space를 탐색하는 two-stage serach algorithm을 제안한다. 
4. 이때, First stage는 SRCC를 이용해 hyperparameter space를 줄이고, subsampled dataset으로 evaluation cost를 줄인다음 surrogate RF model을 학습시킨다.
5. 이후 second stage에서 전체 data에서 top candidate model을 효율적으로 fine-tuning하여 효율적으로 optimal한 architecture와 hyperparameter pair를 찾을 수 있게 된다.

[Notion review](https://www.notion.so/Efficient-and-Joint-Hyperparameter-and-Architecture-Search-for-Collaborative-Filtering-4a9ae27fa2704c768b033f5df00ae7d4?pvs=4)
#### 논문 소속: Tencent, Baidu, Tsinghua university 
