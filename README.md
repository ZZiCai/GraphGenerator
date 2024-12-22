# GraphGenerator

Repo link: [AI4Risk/GraphGenerator](https://github.com/AI4Risk/GraphGenerator)

[AI4Risk/GraphGenerator](https://github.com/AI4Risk/GraphGenerator) integrates various **pre-processing codes** for static and dynamic graph data, multiple **learning-based methods** for static and dynamic graph generation, as well as related **evaluation tools**.

## Learning-based Methods

- `BTGAE`: **Divide and Conquer: A Topological Heterogeneity-based Framework for Scalable and Realistic Graph Generation**. *(Official PyTorch Implementation)*
- `CPGAE`: **Efficient Learning-based Community-Preserving Graph Generation**, in *ICDE* 2022. (GAE version of CPGAN)
- `VRDAG`: **Efficient Dynamic Attributed Graph Generation**, in *ICDE* 2025.
- `TGAE`: **Efficient Learning-based Graph Simulation for Temporal Graphs**, in *ICDE* 2025.

Implementation of baselines:

- `GraphRNN`: **GraphRNN: Generating Realistic Graphs with Deep Auto-regressive Models**, in *ICML* 2018.

## Data Description

The following datasets are mainly from [linqs](https://linqs.org/datasets/) and [snap](https://snap.stanford.edu/data/).

| Data     | #Nodes  | #Edges    | $d_{mean}$ | GINI  | PWE   |
| -------- | ------- | --------- | ---------- | ----- | ----- |
| citeseer | 3,327   | 4,732     | 2.774      | 0.435 | 2.420 |
| cora     | 2,708   | 5,429     | 3.898      | 0.405 | 1.932 |
| pubmed   | 19,717  | 44,338    | 4.496      | 0.604 | 2.176 |
| Epinions | 75,879  | 508,837   | 10.694     | 0.805 | 2.026 |
| google   | 875,713 | 5,105,039 | 9.871      | 0.587 | 1.617 |
| YelpChi  | 45,954  | 3,846,979 | 167.427    | 0.322 | 1.205 |

$d_{mean}$: mean degree.

`GINI`:  GINI index, which is a common measure for inequality in a degree distribution.

`PWE`: power-law exponent.



The following **temporal network datasets** are from [linqs](https://linqs.org/datasets/) and [Network Repository](https://networkrepository.com/). For more information, please refer to the [VRDAG paper](https://arxiv.org/abs/2412.08810).

| Data          | #Nodes | #Edges  | T    |
| ------------- | ------ | ------- | ---- |
| Emails-DNC    | 1,891  | 39,264  | 14   |
| Bitcoin-Alpha | 3,783  | 24,186  | 37   |
| Wiki-Vote     | 7,115  | 103,689 | 43   |

## Contributors

<a href="https://github.com/AI4Risk/GraphGenerator/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=AI4Risk/GraphGenerator" /></a>

## Citing

If you find *GraphGenerator* is useful for your research, please consider citing the following papers:

```bibtex
@inproceedings{xiang2022efficient,
  title={Efficient learning-based community-preserving graph generation},
  author={Xiang, Sheng and Cheng, Dawei and Zhang, Jianfu and Ma, Zhenwei and Wang, Xiaoyang and Zhang, Ying},
  booktitle={2022 IEEE 38th International Conference on Data Engineering (ICDE)},
  pages={1982--1994},
  year={2022},
  organization={IEEE}
}

@inproceedings{li2025efficient,
  title={Efficient Dynamic Attributed Graph Generation},
  author={Li, Fan and Wang, Xiaoyang and Cheng, Dawei and Chen, Cong and Zhang, Ying and Lin, Xuemin},
  booktitle={2025 IEEE 41th International Conference on Data Engineering (ICDE)},
  year={2025},
  organization={IEEE}
}

@inproceedings{xiang2025efficient,
  title={Efficient Learning-based Graph Simulation for Temporal Graphs},
  author={Xiang, Sheng and Xu, Chenhao and  Cheng, Dawei and Wang, Xiaoyang and Zhang, Ying},
  booktitle={2025 IEEE 41th International Conference on Data Engineering (ICDE)},
  year={2025},
  organization={IEEE}
}
```
