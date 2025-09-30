## 💼 Internship Experience

#### **May 2025 – Sep 2025 | ByteDance ｜ Data-Recommendation**

##### Key Contributions
**Project 1: Push Content Moderation Model**
- Designed and built a benchmark for content moderation, defining evaluation metrics and producing high-quality datasets; trained **Doubao-1.5-Pro**, achieving **83.2% P@R=0.8** with false positive rate reduced to **10.8%**.
- Applied a **CoT+SFT hybrid training strategy** with 8-step CoT data, enhancing complex reasoning and bringing **+3.8% Precision** and **-2.8% false positives**, leading to successful deployment.

**Project 2: Multimodal Representation Pretraining**
- Integrated heterogeneous data from recommendation, search, and moderation to build tens of millions of multimodal samples; extended model input to **8k text tokens and 8 video frames**.
- Adopted **VLM backbone** with bi-directional attention and mean pooling embeddings; applied a **two-stage training**: (1) unsupervised contrastive learning for base semantics, (2) supervised fine-tuning with high-quality pairs and hard negatives.
- Results: **NDCG@10 from 71.2% → 80.4%** (retrieval), **+2.1% AUC** (CTR prediction), **P@R=0.5 from 17.5% → 19.0%** (classification).

---

#### **Jan 2025 – May 2025 | Baidu ｜ ERNIE Bot**

##### Key Contributions
- Proposed an **automatic synthesis pipeline** for multimodal preference data, with multi-stage filtering: query–caption overlap, key information masking with response sampling, and pair scoring with reward model or human labels.
- Achieved **99%+ accuracy** under human evaluation; in **DPO experiments**, optimized model outperformed base model on GSB metric with a **38.5% : 61.5% : 0** win–tie–loss distribution.

---

#### **Oct 2024 – Jan 2025 | Meituan ｜ Core Local Commerce**

##### Key Contributions
- Designed and optimized part of the **IM Lead-Collection Bot** (nighttime customer service), successfully launched on Meituan App.
- Fine-tuned **bge-large-zh-v1.5 embedding model**, improving FAQ recall by **+15%**.
- Optimized **response model (SFT)** with real dialogues, semi-automatic LLM data, and fallback responses, raising accuracy **39% → 83%**.
- Explored **CPT+SFT** training for 14B model with domain-specific KB, outperforming a 72B SFT-only model while reducing inference cost.
- Built diverse samples from bad cases to iteratively improve **intent recognition** and **hallucination detection**.
