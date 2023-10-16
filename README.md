# BERT-for-Korean

- KoBERT, KcBERT, KcELECTRA를 base-model로
- domain adaptative pretrain (DAPT)
- classification train(fine-tune)을 진행함
- KcELECTRA + DAPT 성능이 가장 좋음.
- 데이터가 적어서 에포크를 증가시킬 수 없었음.
- DAPT에서 GPU가 멈추는 문제로 배치 사이즈를 높일 수 없었음
- 한글 전처리에서 py-hanspell 에러(https://github.com/ssut/py-hanspell/issues/41) API 문제라 ... 사용 못했음.
