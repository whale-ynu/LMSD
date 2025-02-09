# Reference

If you use the code, please cite the following [paper](https://link.springer.com/article/10.1007/s00521-023-08308-3):

```
@article{DBLP:journals/nca/QinWZLD23,
  author       = {Shaowei Qin and
                  Hao Wu and
                  Lihua Zhou and
                  Jiahui Li and
                  Guowang Du},
  title        = {Learning metric space with distillation for large-scale multi-label
                  text classification},
  journal      = {Neural Comput. Appl.},
  volume       = {35},
  number       = {15},
  pages        = {11445--11458},
  year         = {2023}
}
```

## Requirements
* python==3.8.8
* tensorflow==2.7.0

## Datasets
* [Reuter](https://archive.ics.uci.edu/ml/datasets/Reuters-21578+Text+Categorization+Collection)
* [EUR-Lex](https://drive.google.com/open?id=1iPGbr5-z2LogtMFG1rwwekV_aTubvAb2)
* [Wiki10-31K](https://drive.google.com/open?id=1Tv4MHQzDWTUC9hRFihRhG8_jt1h0VhnR)
* [CiteULike-t](https://github.com/js05212/citeulike-t)
* Download the GloVe embedding (840B,300d)  (https://nlp.stanford.edu/projects/glove/)

## Train and Test
Run main.py for train and test datasets with tokenized texts as follows:
```bash
python main.py --data 'Wiki10-31K' --la 1.0 --ba 1.0 --emb_num 256 --n_negative 1000
```
