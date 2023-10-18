# BERT-for-Korean

- KoBERT, KcBERT, KcELECTRA를 base-model로
- domain adaptive pretrain (DAPT)
    - batch size를 GPU 용량에 따라 조절할 수 있는 코드였으나 GPU가 꺼져버리는
    - batch size를 작게 고정하고 학습 진행함.
- classification train(fine-tune)을 진행함
    - 데이터가 적어서 에포크를 증가시킬 수 없었음.
- KcELECTRA + DAPT 성능이 가장 좋음.
  
- 한글 전처리에서 py-hanspell 에러(https://github.com/ssut/py-hanspell/issues/41) API 문제라 ... 사용 못했음.
