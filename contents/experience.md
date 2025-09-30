## 💼 Internship Experience

[🇨🇳 中文](#-算法实习生) | [🇺🇸 English](#-algorithm-intern)

---

### **算法实习生**

#### **2025年5月 – 2025年9月 | 字节跳动 ｜ Data-推荐**

##### 主要贡献
**项目一：头条push文案审核模型**
- 设计并构建文案审核benchmark，明确评估维度与指标，产出高质量训练与测试数据集，训练Doubao-1.5-Pro模型，在测试集上P@R=0.8达到83.2%，误伤率显著下降至10.8%。
- 使用CoT+SFT混合训练策略，引入八段式CoT数据提升模型复杂推理能力，平均带来3.8%的Precision提升和2.8%的误伤率下降，最终推动模型成功上线。

**项目二：多模态表征预训练**
- 融合推荐、搜索、内容审核等场景的多源异构数据，构建千万级规模的多模态训练样本；扩展模型输入能力，使其支持最长8k的文本序列和8帧图像输入，增强对长文本和视频类内容的建模能力。
- 采用VLM作为backbone，引入双向注意力机制并将每个token的隐状态通过mean pooling作为序列嵌入；采用两阶段训练策略：第一阶段通过无监督对比学习建立基础语义表征，第二阶段结合高质量pair数据与困难负样本挖掘，进一步提升多模态对齐与判别能力。
- 多模态检索任务上，NDCG@10指标上从71.2%提升至80.4%；推荐CTR任务中，AUC指标提升2.1%；多模态分类任务中，P@R=0.5由17.5%提升至19.0%。

---

#### **2025年1月 – 2025年5月 | 百度 ｜ 文心一言**

##### 主要贡献
- 提出高质量多模态偏好数据自动合成方案，设计多轮过滤机制：query-caption重合度筛选、图片重要信息掩码与回复采样、pair打分过滤（基于奖励模型或人工标注），提升数据质量。
- 合成数据效果显著：正负样本经人工标注准确率达99%+；DPO实验中，优化后模型相较base模型在GSB指标上达成38.5% : 61.5% : 0优势分布。

---

#### **2024年10月 – 2025年1月 | 美团 ｜ 核心本地商业**

##### 主要贡献
- 负责IM留资机器人（夜间智能客服）部分链路的设计与优化，并推动产品成功上线至美团APP。
- 针对业务场景构建数据微调的embedding模型 (bge-large-zh-v1.5)，使FAQ整体召回率提升15%。
- 负责回复模型SFT的迭代优化，整合真实历史对话、LLM半自动生成对话、兜底话术等数据，对话准确率由39%提高至83%。
- 探索CPT+SFT的回复模型(14B)训练方式，结合真实对话与医美知识库并进行过滤，表现优于只做SFT的72B模型，降低了线上推理成本。
- 基于线上及自测的bad case，构建多样化训练样本，迭代优化意图识别和幻觉检测等其他核心模块。

---

### **Algorithm Intern**

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
