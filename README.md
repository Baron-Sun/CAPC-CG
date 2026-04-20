# CAPC-CG

> **Chinese Adaptive Policy Communication (Central Government) Corpus** —
> the companion dataset to our ACL 2026 paper.

[![Hugging Face](https://img.shields.io/badge/🤗%20Dataset-Baron--Sun/CAPC--CG__V1.0-yellow?style=for-the-badge)](https://huggingface.co/datasets/Baron-Sun/CAPC-CG_V1.0)
[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey?style=for-the-badge)](https://creativecommons.org/licenses/by-nc/4.0/)
[![ACL 2026](https://img.shields.io/badge/ACL-2026%20Main-red?style=for-the-badge)](https://2026.aclweb.org/)
[![arXiv](https://img.shields.io/badge/arXiv-2510.08986-b31b1b?style=for-the-badge)](https://arxiv.org/abs/2510.08986)

---

## 📦 The dataset now lives on Hugging Face Hub

**👉 [huggingface.co/datasets/Baron-Sun/CAPC-CG_V1.0](https://huggingface.co/datasets/Baron-Sun/CAPC-CG_V1.0)**

The corpus (≈3.3 M paragraphs, 1949–2023) and the gold-standard labeled splits
(`task1_level1` / `task2_level2`) are all hosted there as Parquet, queryable
directly with `🤗 datasets`:

```python
from datasets import load_dataset

# Full corpus (3.3M paragraphs, streaming recommended)
corpus = load_dataset("Baron-Sun/CAPC-CG_V1.0", "full_corpus",
                      split="train", streaming=True)

# Gold-standard labeled splits
task1 = load_dataset("Baron-Sun/CAPC-CG_V1.0", "task1_level1")   # N / R / W
task2 = load_dataset("Baron-Sun/CAPC-CG_V1.0", "task2_level2")   # B / Y / C / G
```

---

## 🔐 Access

The dataset is released as a **gated resource** under **CC BY-NC 4.0**
(non-commercial research use only). To get it:

1. Sign in to [Hugging Face](https://huggingface.co) (free).
2. On [the dataset page](https://huggingface.co/datasets/Baron-Sun/CAPC-CG_V1.0),
   click **"Request Access"** and fill in the short form
   (name · affiliation · intended use · agree to cite & not redistribute).
3. We aim to approve within **one week**. You'll get an email notification.
4. Once approved, `load_dataset(...)` works with your Hugging Face token:

   ```bash
   huggingface-cli login   # paste your HF read token
   ```

For urgent or cross-institution requests, you may also email
**bolun.sun@kellogg.northwestern.edu** with your background and use case.

---

## 🔔 Stay in the loop — updates & new releases

CAPC-CG is an **actively maintained** resource. We plan to release:

- Periodic corpus refreshes as new policy documents are issued;
- Improved annotations as the codebook evolves;
- Additional data streams (leadership speeches, local-government policies).

👉 **[Join our announcement mailing list](https://groups.google.com/g/capc-cg-announce)**
to be notified the moment a new version goes live. *(low-volume, ≤ 1 email/month,
unsubscribe anytime)*

*Not on Google? Email us at `bolun.sun@kellogg.northwestern.edu` with subject
**"Subscribe CAPC-CG"** and we'll add you manually.*

---

## 📄 Paper

**CAPC-CG: A Large-Scale, Expert-Directed LLM-Annotated Corpus of Adaptive
Policy Communication in China**
Bolun Sun¹·², Charles Chang³, Yuen Yuen Ang¹, Ruotong Mu¹, Yuchen Xu¹,
Zhengxin Zhang¹, Pingxu Hao¹
*¹ Johns Hopkins University  · ² Northwestern University  · ³ Duke Kunshan University*
**Accepted to ACL 2026 (Main Conference).**

**📑 Preprint:** [arXiv:2510.08986](https://arxiv.org/abs/2510.08986)

---

## 📖 Citation

If you use CAPC-CG in any publication, presentation, blog post, or other
public artifact, **please be sure to cite our paper**:

```bibtex
@inproceedings{sun2026capccg,
  title     = {{CAPC-CG}: A Large-Scale, Expert-Directed {LLM}-Annotated Corpus
               of Adaptive Policy Communication in China},
  author    = {Sun, Bolun and Chang, Charles and Ang, Yuen Yuen and
               Mu, Ruotong and Xu, Yuchen and Zhang, Zhengxin and Hao, Pingxu},
  booktitle = {Proceedings of the 64th Annual Meeting of the Association for
               Computational Linguistics (ACL)},
  year      = {2026},
  publisher = {Association for Computational Linguistics}
}
```

---

## 📬 Contact

- **General / access requests:** [bolun.sun@kellogg.northwestern.edu](mailto:bolun.sun@kellogg.northwestern.edu)
- **Bug reports / data errata:** open an issue in this repository
- **Collaboration & commercial licensing:** please reach out by email

---

## ⚖️ License

CAPC-CG is released under the
[**Creative Commons Attribution-NonCommercial 4.0 International License**
(CC BY-NC 4.0)](https://creativecommons.org/licenses/by-nc/4.0/).

You are free to **share** and **adapt** the data for **non-commercial research
purposes**, provided that you cite the accompanying paper and do not
redistribute the data in whole or in part.
