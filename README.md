## Downstream Datasets Make Surprisingly Good Pretraining Corpora



This repository contains the links to the models pretrained in the paper 
[Downstream Datasets Make Surprisingly Good Pretraining Corpora
](https://arxiv.org/abs/2209.14389).
The models are pretrained from scratch on text from the train split of popular downstream datasets.
The models are hosted on Huggingface and their links are given below. The links to the datasets used for pretraining are also provided.


| Pretraining dataset                          | Corpus size (MB) | Electra model                     | Roberta model                     |  
|----------------------------------------------|------------------|-----------------------------------|-----------------------------------|
| [CoNLL-2012][ds-conll2012]                   | 6.4              | [link][electra-conll2012]         | [link][roberta-conll2012]         |
| [SQuAD-v1.1][ds-squad_v1]                    | 19               | [link][electra-squad_v1.1]        | [link][roberta-squad_v1.1]        |
| [SWAG][ds-swag]                              | 22               | [link][electra-swag]              | [link][roberta-swag]              |
| [AG News][ds-agnews]                         | 27               | [link][electra-agnews]            | [link][roberta-agnews]            |
| [HellaSwag][ds-hellaswag]                    | 30               | [link][electra-hellaswag]         | [link][roberta-hellaswag]         |
| [QQP][ds-qqp]                                | 43               | [link][electra-qqp]               | [link][roberta-qqp]               |
| [Jigsaw][ds-jigsaw]                          | 59               | [link][electra-jigsaw]            | [link][roberta-jigsaw]            |
| [MNLI][ds-mnli]                              | 65               | [link][electra-mnli]              | [link][roberta-mnli]              |
| [Sentiment140][ds-sentiment140]              | 114              | [link][electra-sentiment140]      | [link][roberta-sentiment140]      |
| [PAWS][ds-paws]                              | 139              | [link][electra-paws]              | [link][roberta-paws]              |
| [DBPedia14][ds-dbpedia14]                    | 151              | [link][electra-dbpedia14]         | [link][roberta-dbpedia14]         |
| [Yahoo Answers Topics][ds-yahooanswertopics] | 461              | [link][electra-yahooanswertopics] | [link][roberta-yahooanswertopics] |
| [Discovery][ds-discovery]                    | 293              | [link][electra-discovery]         | [link][roberta-discovery]         |
| [Amazon Polarity][ds-amazonpolarity]         | 1427             | [link][electra-amazonpolarity]    | [link][roberta-amazonpolarity]    |


### Pretraining Hyperparameters

| Hyperparameter | ELECTRA | Roberta |
|---|---|---|
| Size | Small | Base |
| Parameter count | 14M | 110M |
| Training steps | 1M | 100K |
| Warmup steps | 10K | 6K |
| Batch size | 128 | 512 |
| Peak learning rate | 5e-4 | 5e-4 |
| Sequence length | 128 | 512 |
---

More details can be found in the paper: [https://arxiv.org/abs/2209.14389](https://arxiv.org/abs/2209.14389)

If you use these models, please use citation given below:
```
@article{krishna2022downstream,
  title={Downstream datasets make surprisingly good pretraining corpora},
  author={Krishna, Kundan and Garg, Saurabh and Bigham, Jeffrey P and Lipton, Zachary C},
  journal={arXiv preprint arXiv:2209.14389},
  year={2022}
}
```


[electra-agnews]: https://huggingface.co/kundank/dspt-electra-small-agnews
[electra-amazonpolarity]: https://huggingface.co/kundank/dspt-electra-small-amazonpolarity
[electra-conll2012]: https://huggingface.co/kundank/dspt-electra-small-conll2012
[electra-dbpedia14]: https://huggingface.co/kundank/dspt-electra-small-dbpedia14
[electra-discovery]: https://huggingface.co/kundank/dspt-electra-small-discovery
[electra-hellaswag]: https://huggingface.co/kundank/dspt-electra-small-hellaswag
[electra-jigsaw]: https://huggingface.co/kundank/dspt-electra-small-jigsaw
[electra-mnli]: https://huggingface.co/kundank/dspt-electra-small-mnli
[electra-paws]: https://huggingface.co/kundank/dspt-electra-small-paws
[electra-qqp]: https://huggingface.co/kundank/dspt-electra-small-qqp
[electra-sentiment140]: https://huggingface.co/kundank/dspt-electra-small-sentiment140
[electra-squad_v1.1]: https://huggingface.co/kundank/dspt-electra-small-squad_v1.1
[electra-swag]: https://huggingface.co/kundank/dspt-electra-small-swag
[electra-yahooanswertopics]: https://huggingface.co/kundank/dspt-electra-small-yahooanswertopics

[roberta-agnews]: https://huggingface.co/kundank/dspt-roberta-base-agnews
[roberta-amazonpolarity]: https://huggingface.co/kundank/dspt-roberta-base-amazonpolarity
[roberta-conll2012]: https://huggingface.co/kundank/dspt-roberta-base-conll2012
[roberta-dbpedia14]: https://huggingface.co/kundank/dspt-roberta-base-dbpedia14
[roberta-discovery]: https://huggingface.co/kundank/dspt-roberta-base-discovery
[roberta-hellaswag]: https://huggingface.co/kundank/dspt-roberta-base-hellaswag
[roberta-jigsaw]: https://huggingface.co/kundank/dspt-roberta-base-jigsaw
[roberta-mnli]: https://huggingface.co/kundank/dspt-roberta-base-mnli
[roberta-paws]: https://huggingface.co/kundank/dspt-roberta-base-paws
[roberta-qqp]: https://huggingface.co/kundank/dspt-roberta-base-qqp
[roberta-sentiment140]: https://huggingface.co/kundank/dspt-roberta-base-sentiment140
[roberta-squad_v1.1]: https://huggingface.co/kundank/dspt-roberta-base-squad_v1.1
[roberta-swag]: https://huggingface.co/kundank/dspt-roberta-base-swag
[roberta-yahooanswertopics]: https://huggingface.co/kundank/dspt-roberta-base-yahooanswertopics

[ds-agnews]: https://huggingface.co/datasets/ag_news
[ds-amazonpolarity]: https://huggingface.co/datasets/amazon_polarity
[ds-conll2012]: https://github.com/explosion/conll-2012
[ds-dbpedia14]: https://huggingface.co/datasets/dbpedia_14
[ds-discovery]: https://huggingface.co/datasets/discovery
[ds-hellaswag]: https://huggingface.co/datasets/hellaswag
[ds-jigsaw]: https://huggingface.co/datasets/jigsaw_toxicity_pred
[ds-mnli]: https://huggingface.co/datasets/glue
[ds-paws]: https://huggingface.co/datasets/paws
[ds-qqp]: https://huggingface.co/datasets/glue
[ds-sentiment140]: https://huggingface.co/datasets/sentiment140
[ds-squad_v1]: https://huggingface.co/datasets/squad
[ds-swag]: https://huggingface.co/datasets/swag
[ds-yahooanswertopics]: https://huggingface.co/datasets/yahoo_answers_topics

