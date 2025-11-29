---
layout: page
title: Research
permalink: /research/
---

The **Nordic AI Safety Lab** develops methods to understand and control AI systems. We believe that interpretability—understanding the internal mechanisms of AI—is essential for achieving meaningful control and ensuring safety.

## Research Areas

Our research is organized around six interconnected themes, following the research taxonomy established by the [International Association for AI Safety](https://www.iaseai.org):

### Interpretability & Transparency

Understanding how AI systems work internally is foundational to safety. We develop mechanistic interpretability methods and probes to trace and visualize the mechanisms underlying AI behavior, focusing on:
- Mechanistic interpretability of language models and neural agents
- Probing techniques to understand internal representations and their causal effects
- Methods for making AI decision-making processes transparent and auditable

**Publications:**

{% include publication.html
    title="Isolating Culture Neurons in Multilingual Large Language Models"
    authors="Danial Namazifard, Lukas Galke"
    venue="IJCNLP-AACL 2025"
    abstract="Language and culture are deeply intertwined, yet it is so far unclear how and where multilingual large language models encode culture. Here, we extend upon an established methodology for identifying language-specific neurons and extend it to localize and isolate culture-specific neurons, carefully disentangling their overlap and interaction with language-specific neurons. To facilitate our experiments, we introduce MUREL, a curated dataset of 85.2 million tokens spanning six different cultures. Our localization and intervention experiments show that LLMs encode different cultures in distinct neuron populations, predominantly in upper layers, and that these culture neurons can be modulated independently from language-specific neurons or those specific to other cultures. These findings suggest that cultural knowledge and propensities in multilingual language models can be selectively isolated and edited - promoting fairness, inclusivity, and alignment."
    code_url="https://github.com/namazifard/Culture_Neurons"
    year="2025"
    authorcopy_url="https://arxiv.org/abs/2508.02241"
%}

{% include publication.html
    title="Tokenization and Morphology in Multilingual Language Models: A Comparative Analysis of mT5 and ByT5"
    authors="Thao Anh Dang, Limor Raviv, Lukas Galke"
    venue="ICNLSP"
    year="2025"
    abstract="Morphology is a crucial factor for multilingual language modeling as it poses direct challenges for tokenization. Here, we seek to understand how tokenization influences the morphological knowledge encoded in multilingual language models. Specifically, we capture the impact of tokenization by contrasting a minimal pair of multilingual language models: mT5 and ByT5. The two models share the same architecture, training objective, and training data and only differ in their tokenization strategies: subword tokenization vs. character-level tokenization. Probing the morphological knowledge encoded in these models on four tasks and 17 languages, our analyses show that the models learn the morphological systems of some languages better than others and that morphological information is encoded in the middle and late layers. Finally, we show that languages with more irregularities benefit more from having a higher share of the pre-training data."
    paper_url="https://aclanthology.org/2025.icnlsp-1.24/"
%}

{% include publication.html
    title="Learning and communication pressures in neural networks: Lessons from emergent communication"
    authors="Lukas Galke, Limor Raviv"
    venue="Language Development Research 5(1)"
    year="2025"
    paper_url="https://doi.org/10.34842/3vr5-5r49"
    authorcopy_url="https://arxiv.org/abs/2403.14427"
%}

{% include publication.html
    title="Deep neural networks and humans both benefit from compositional language structure"
    authors="Lukas Galke, Yoav Ram, Limor Raviv"
    venue="Nature Communications 15:10816"
    year="2024"
    paper_url="https://rdcu.be/d5f2e"
    code_url="https://github.com/lgalke/easy2deeplearn"
    data_url="https://doi.org/10.5281/zenodo.14205452"
%}

{% include publication.html
    title="Morphology Matters: Probing the Cross-linguistic Morphological Generalization Abilities of Large Language Models through a Wug Test"
    authors="Anh Dang, Limor Raviv, Lukas Galke"
    venue="Cognitive Modeling and Computational Linguistics Workshop at ACL 2024"
    paper_url="https://aclanthology.org/2024.cmcl-1.15/"
%}

### Control & Containment

Interpretability insights enable better control mechanisms. We develop guardrails and containment strategies, working on:
- Interpretability-informed intervention techniques for steering AI behavior
- Guardrails and containment strategies for limiting unintended AI capabilities
- Safe deployment frameworks that leverage mechanistic understanding

**Publications:**

{% include publication.html
    title="Guarded Query Routing for Large Language Models"
    authors="Richard Šléher, William Brach, Tibor Sloboda, Kristián Košťál, and Lukas Galke"
    venue="ECAI"
    year="2025"
    authorcopy_url="https://arxiv.org/abs/2505.14524"
    project_url="https://gqr-bench.github.io"
    code_url="https://github.com/williambrach/gqr"
%}

### Agentic & Multi-Agent Safety

AI agents introduce unique safety challenges, especially when multiple agents interact. Our research addresses risks of deception, collusion, and miscoordination:
- Safety in emergent communication and coordination between AI agents
- Understanding and mitigating risks of deception and collusion in multi-agent systems
- Robustness and alignment in agentic systems

**Publications:**

{% include publication.html
    title="Super-additive Cooperation in Language Model Agents"
    authors="Filippo Tonini, Lukas Galke"
    venue="3rd International Conference on Frontiers of Artificial Intelligence, Ethics, and Multidisciplinary Applications (FAIEMA)"
    year="2025"
    authorcopy_url="https://arxiv.org/abs/2508.15510"
    project_url="https://github.com/pippot/Superadditive-cooperation-LLMs"
%}

### Safety Evaluation

Rigorous evaluation is critical for assessing AI safety properties. We develop benchmarks, metrics, and methods for dangerous capability evaluation:
- Benchmarks and metrics for interpretability and control
- Methods for evaluating dangerous capabilities before deployment
- Frameworks for continual safety assessment in evolving systems

**Publications:**

{% include publication.html
    title="Guarded Query Routing for Large Language Models"
    authors="Richard Šléher, William Brach, Tibor Sloboda, Kristián Košťál, and Lukas Galke"
    venue="ECAI"
    year="2025"
    authorcopy_url="https://arxiv.org/abs/2505.14524"
    project_url="https://gqr-bench.github.io"
    code_url="https://github.com/williambrach/gqr"
%}

### Uncertainty & Risk Quantification

Quantifying and managing uncertainty is essential for safe AI deployment. We develop methods for calibration, anomaly detection, out-of-distribution detection, and establishing safety margins:
- Open-world classification and detection of novel inputs
- Out-of-distribution detection in continual learning settings
- Methods for quantifying model uncertainty in safety-critical scenarios

**Publications:**

{% include publication.html
    title="POWN: Prototypical Open-world Node Classification"
    authors="Marcel Hoffmann, Lukas Galke, Ansgar Scherp"
    venue="Conference on Lifelong Learning Agents (CoLLAs)"
    year="2024"
    paper_url="https://lifelong-ml.cc/Conferences/2024/acceptedpapersandvideos/conf-2024-38"
    code_url="https://github.com/Bobowner/POWN"
%}

{% include publication.html
    title="Lifelong Learning on Evolving Graphs Under the Constraints of Imbalanced Classes and New Classes"
    authors="Lukas Galke, Iacopo Vagliano, Benedikt Franke, Tobias Zielke, Marcel Hoffmann, and Ansgar Scherp"
    abstract="Lifelong graph learning deals with the problem of continually adapting graph neural network (GNN) models to changes in evolving graphs. We address two critical challenges of lifelong graph learning in this work: dealing with new classes and tackling imbalanced class distributions. The combination of these two challenges is particularly relevant since newly emerging classes typically resemble only a tiny fraction of the data, adding to the already skewed class distribution. We make several contributions: First, we show that the amount of unlabeled data does not influence the results, which is an essential prerequisite for lifelong learning on a sequence of tasks. Second, we experiment with different label rates and show that our methods can perform well with only a tiny fraction of annotated nodes. Third, we propose the gDOC method to detect new classes under the constraint of having an imbalanced class distribution. The critical ingredient is a weighted binary cross-entropy loss function to account for the class imbalance. Moreover, we demonstrate combinations of gDOC with various base GNN models such as GraphSAGE, Simplified Graph Convolution, and Graph Attention Networks. Lastly, our k-neighborhood time difference measure provably normalizes the temporal changes across different graph datasets. With extensive experimentation, we find that the proposed gDOC method is consistently better than a naive adaption of DOC to graphs. Specifically, in experiments using the smallest history size, the out-of-distribution detection score of gDOC is 0.09 compared to 0.01 for DOC. Furthermore, gDOC achieves an Open-F1 score, a combined measure of in-distribution classification and out-of-distribution detection, of 0.33 compared to 0.25 of DOC (32% increase)."
    venue="Neural Networks 164"
    year="2023"
    paper_url="https://doi.org/10.1016/j.neunet.2023.04.022"
    authorcopy_url="https://pure.mpg.de/rest/items/item_3368482_4/component/file_3510107/content"
    data_url="https://doi.org/10.5281/zenodo.3764770"
    code_url="https://github.com/lgalke/lifelong-learning"
%}

### Sustainability & Resource Impact

AI safety extends beyond technical robustness to encompass environmental and societal sustainability.

{% include publication.html
    title="Continual Quantization-Aware Pre-Training: When to transition from 16-bit to 1.58-bit pre-training for BitNet language models?"
    authors="Jacob Nielsen, Peter Schneider-Kamp, and Lukas Galke"
    venue="ACL Findings"
    year="2025"
    abstract="Large language models (LLMs) require immense resources for training and inference. Quantization, a technique that reduces the precision of model parameters, offers a promising solution for improving LLM efficiency and sustainability. While post-training quantization methods typically achieve 4-8 bits per parameter, recent research suggests that training LLMs with 1.58 bits per weight parameter from scratch can maintain model accuracy while greatly reducing memory requirements and energy consumption at inference time. Here, we investigate a training strategy for quantization-aware pre-training, where the models are first trained with 16-bit precision and then transition into 1.58-bit quantization-aware training. Our results on 11 downstream tasks, show that this 16-to-1.58-bit training strategy is preferable over full 1.58-bit training and leaves models closer to those which have undergone 16-bit training. We further investigate the effects of retaining the optimizer state at the transition point and gradually phasing in quantization strength - finding that both techniques alleviate the magnitude of loss spikes, but also that these effects can be compensated through further training."
    paper_url="https://aclanthology.org/2025.findings-acl.694/"
%}

{% include publication.html
    title="When are 1.58 bits enough? A Bottom-up Exploration of Quantization-aware Training with Ternary Weights"
    authors="Jacob Nielsen, Lukas Galke, and Peter Schneider-Kamp"
    venue="18th International Conference on Agents and Artificial Intelligence (ICAART)"
    year="2025"
    abstract="Contemporary machine learning models, such as language models, are powerful, but come with immense resource requirements both at training and inference time. It has been shown that decoder-only language models can be trained to a competitive state with ternary weights (1.58 bits per weight), facilitating efficient inference. Here, we start our exploration with non-transformer model architectures, investigating 1.58-bit training for multi-layer perceptrons and graph neural networks. Then, we explore 1.58-bit training in other transformer-based language models, namely encoder-only and encoder-decoder models. Our results show that in all of these settings, 1.58-bit training is on par with or sometimes even better than the standard 32/16-bit models."
    authorcopy_url="https://arxiv.org/abs/2411.05882"
%}

