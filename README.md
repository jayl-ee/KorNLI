# 한국어 문장 관계 분류 경진대회\(DACON주최)

# Requirements
- torch == 1.6.0
- transformers == 3.3.1
- seqeval
- fastprogress
- attrdict

## Data
* train_data.csv
* test_data.csv
* sample_submission.csv

COLUMNS : Index , Premise, Hypothesis, label\
LABEL : contradiction , entailment, neutral

## Model
- KoElectra [링크] (https://github.com/monologg/KoELECTRA)
- Kobert [링크] (https://github.com/SKTBrain/KoBERT)
- Roberta [링크] (https://huggingface.co/Huffon/klue-roberta-base-nli/tree/main)



## Example
``` python
from transformers import AutoTokenizer, TFAutoModel

tokenizer = AutoTokenizer.from_pretrained(model_name)
model = TFAutoModel.from_pretrained(model_name, from_pt=True)
```

