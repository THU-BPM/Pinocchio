# Pinocchio
Dataset Pinocchio for paper "Towards Understanding Factual Knowledge of Large Language Models" accepted by ICLR 2024 (Spotlight)

### Pinocchio Dataset

[[paper](https://arxiv.org/abs/2310.05177)]

Large language models (LLMs) have recently driven striking performance improvements across a range of natural language processing tasks. The factual knowledge acquired during pretraining and instruction tuning can be useful in various downstream tasks, such as question answering, and language generation. Unlike conventional Knowledge Bases (KBs) that explicitly store factual knowledge, LLMs implicitly store facts in their parameters. Content generated by the LLMs can often exhibit inaccuracies or deviations from the truth, due to facts that can be incorrectly induced or become obsolete over time. To this end, we aim to explore the extent and scope of factual knowledge within LLMs by designing the benchmark Pinocchio. Pinocchio contains 20K diverse factual questions that span different sources, timelines, domains, regions, and languages. Furthermore, we investigate whether LLMs can compose multiple facts, update factual knowledge temporally, reason over multiple pieces of facts, identify subtle factual differences, and resist adversarial examples.


<p align="center">
    <img src="img/Pinocchios_00.jpg" height="300"/>
</p>

### Dataset Details

|     Domain      |                  Description                  |      Sources       |  |   Label   | Distribution |        |
| :-------------: | :-------------------------------------------: | :----------------: | :----------: | :-------: | :---: | :----: |
|                 |                                               |                    |    Fact.     | Non-Fact. | NEI   | ALL    |
|  Multifaceted   |            Contain multiple facts             |       FEVER        |    1,111     | 1,111     | 1,110 | 3,332  |
|   Structural    |   Contain structured and unstructured facts   |      FEVEROUS      |    1,741     | 1,953     | 250   | 3,944  |
|   Adversarial   |  Contain facts edited by adversarial methods  |   Symmetric, FM2   |     815      | 921       | -     | 1,736  |
|    Temporal     |      Contain facts that change over time      |      VitaminC      |    1,898     | 1,043     | 355   | 3,296  |
|   Real-World    |   Contain factual statements spread online    |     PolitiFact     |     986      | 1,987     | 609   | 3,582  |
| Domain-Specific | Contain facts from health and science domains | PubHealth, SciFact |    1,156     | 715       | 737   | 2,608  |
|  Multi-Lingual  |     Contain facts in different languages      |    XFact, CHEF     |     820      | 848       | 547   | 2,215  |
|      % All      |                                               |                    |    8,713     | 9,619     | 3,608 | 21,940 |

The raw Pinocchio dataset file can be found in:

- `Pinocchio/dataset.jsonl`

The Pinocchio Lite dataset files can be found in:

- `Pinocchio/lite/`

### Citation

Please use the below BibTeX entry to cite this dataset:

~~~tex
@article{HuPino2023,
  author       = {Xuming Hu and
                  Junzhe Chen and
                  Xiaochuan Li and
                  Yufei Guo and
                  Lijie Wen and
                  Philip S. Yu and
                  Zhijiang Guo},
  title        = {Towards Understanding Factual Knowledge of Large Language Models},
  journal      = {12th International Conference on Learning Representations, {ICLR} 2024, Messe Wien Exhibition and Congress Center, Vienna Austria
              May 7th, 2024 to May 11th, 2024},
  volume       = {2024},
  year         = {2024},
  url          = {https://doi.org/10.48550/arXiv.2310.05177},
  doi          = {10.48550/ARXIV.2310.05177},
  eprinttype    = {arXiv},
  eprint       = {2310.05177},
  timestamp    = {Fri, 20 Oct 2023 12:04:38 +0200},
  biburl       = {https://dblp.org/rec/journals/corr/abs-2310-05177.bib},
  bibsource    = {dblp computer science bibliography, https://dblp.org}
}
~~~

