# Reflexive Ethics Protocol for AI Research and Vulnerable Data Subjects 
## From Vulnerable Data Subjects to Vulnerabilizing Data Practices: Navigating the Protection Paradox in AI-Based Analyses of Platformized Lives
[![arXiv](https://img.shields.io/badge/arXiv-2604.15990-b31b1b.svg)](https://arxiv.org/abs/2604.15990)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

This repository operationalizes the **Reflexive Ethics Protocol for AI Research** introduced in our paper: *[Delfina S. Martinez Pandiani, Ella Streefkerk, Laurens Naudts, and Paula Helm. 2026. From Vulnerable Data Subjects to Vulnerabilizing Data Practices: Navigating the Protection Paradox in AI-Based Analyses of Platformized Lives. In The 2026 ACM Conference on Fairness, Accountability, and Transparency (FAccT ’26), June 25–28, 2026, Montreal, QC, Canada. ACM, New York, NY, USA, 23 pages. https://doi.org/10.1145/3805689.3806735]* ([arXiv:2604.15990](https://arxiv.org/abs/2604.15990)). 

Unlike rigid compliance checklists, this framework provides a structural, reflexive journey across four core lifecycle stages of AI research to help researchers audit power dynamics, mitigate data subject vulnerabilities, and navigate systemic tensions.

## 📌 Repository Structure

* **[PROTOCOL.md](./PROTOCOL.md)**: The complete, readable reference table of technical decisions, abstracted ethical tensions, reflexive questions, potential vulnerabilities, and suggested responses.
* **[template_reflexive_ethics.md](./template_reflexive_ethics.md)**: A blank Markdown template you can copy directly into your project's repository or appendix to document your project's reflexive ethical choices.

## Lifecycle Coverage

The protocol breaks down AI pipeline choices across 4 distinct stages:
* **Stage A**: Dataset Design (Scale, Selection, Aggregation, Resolution, Access)
* **Stage B**: Operationalization (Unit of Analysis, Taxometric Architecture, Target Definition)
* **Stage C**: Inference & Evaluation (Infrastructure, Model Selection, Stochasticity, Thresholds, Validation)
* **Stage D**: Dissemination (Narrative Framing, Visualization, Publication)

## How to Use This Protocol

1. **Copy the Template**: Duplicate `template_reflexive_ethics.md` into your own project repository.
2. **Reflect & Complete**: During the design, implementation, and dissemination phases of your research, sit down with your team and systematically work through the reflexive questions.
3. **Document & Disclose**: Use the completed file as a living document. We encourage researchers to publish their completed protocols alongside their codebases or as supplementary materials in academic submissions to promote transparency and reproducibility in research ethics.


## ✍️ Citation & Attribution

If this protocol assists your research design or if you use the markdown template in your repository, please attribute this work. 

### 1. Cite the Research Paper
For academic work discussing the theoretical framework of "vulnerabilizing data practices" or the protection paradox, please cite the foundational paper:

```bibtex
@inproceedings{martinezpandiani2026vulnerable,
  author    = {Martinez Pandiani, Delfina S. and Streefkerk, Ella and Naudts, Laurens and Helm, Paula},
  title     = {From Vulnerable Data Subjects to Vulnerabilizing Data Practices: Navigating the Protection Paradox in AI-Based Analyses of Platformized Lives},
  booktitle = {Proceedings of the 2026 ACM Conference on Fairness, Accountability, and Transparency (FAccT '26)},
  series    = {FAccT '26},
  year      = {2026},
  month     = {June},
  location  = {Montreal, QC, Canada},
  publisher = {ACM},
  address   = {New York, NY, USA},
  pages     = {23},
  doi       = {10.1145/3805689.3806735},
  url       = {[https://doi.org/10.1145/3805689.3806735](https://doi.org/10.1145/3805689.3806735)}
}
```

### 2. Cite this Protocol / Repository
If you are directly adopting, modifying, or embedding this interactive protocol template into your dataset or pipeline documentation, please cite this specific repository:

```
@misc{martinezpandiani2026protocol,
  author       = {Martinez Pandiani, Delfina S. and Streefkerk, Ella and Naudts, Laurens and Helm, Paula},
  title        = {Reflexive Ethics Protocol for AI Research and Vulnerable Data Subjects (Markdown Implementation)},
  year         = {2026},
  publisher    = {GitHub},
  journal      = {GitHub Repository},
  howpublished = {\url{[https://github.com/delfimpandiani/vulnerable-data-subjects](https://github.com/delfimpandiani/vulnerable-data-subjects)}}
}
```
