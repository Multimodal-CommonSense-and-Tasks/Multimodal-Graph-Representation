# Interpretable Prototype-based Graph Information Bottleneck
Official Repository of "Interpretable Prototype-based Graph Information Bottleneck" accepted at NeurIPS 2023.

**Sangwoo Seo, Sungwon Kim, Chanyoung Park**

# Overview of Prototype-based Graph Information Bottleneck.
![architecture2_page-0001](./image_architecture.jpg)

# Paper description and Main Idea:
The success of Graph Neural Networks (GNNs) has led to a need for understanding their decision-making process and providing explanations for their predictions, which has given rise to explainable AI (XAI) that offers transparent explanations for black-box models. Recently, the use of prototypes has successfully improved the explainability of models by learning prototypes to imply training graphs that affect the prediction. However, these approaches tend to provide prototypes with excessive information from the entire graph, leading to the exclusion of key substructures or the inclusion of irrelevant substructures, which can limit both the interpretability and the performance of the model in downstream tasks. In this work, we propose a novel framework of explainable GNNs, called interpretable Prototype-based Graph Information Bottleneck (PGIB) that incorporates prototype learning within the information bottleneck framework to provide prototypes with the key subgraph from the input graph that is important for the model prediction. This is the first work that incorporates prototype learning into the process of identifying the key subgraphs that have a critical impact on the prediction performance. 

# Contribution
*  We propose an effective approach, PGIB, that not only improves the interpretability of the reasoning process, but also the overall performance in downstream tasks by incorporating the prototype learning in a process of detecting key subgraphs based on the IB framework. 
*  We provide theoretical background with our method that utilizes interpretable prototypes in the process of optimizing key subgraphs. 
*  Extensive experiments, including qualitative analysis, demonstrate that PGIB outperforms state-of-the-art methods in terms of both prediction performance and explainability.


# Run (Train & Evaluation)

```
python -m models.train_gnns
```

# Reference
If you find the code useful for your research, please consider citing
```bib
@misc{seo2023interpretable,
      title={Interpretable Prototype-based Graph Information Bottleneck}, 
      author={Sangwoo Seo and Sungwon Kim and Chanyoung Park},
      year={2023},
      eprint={2310.19906},
      archivePrefix={arXiv},
      primaryClass={cs.LG}
}
```

This work is heavily built upon the code from
* Zhang, Zaixi, et al. "Protgnn: Towards self-explaining graph neural networks." Proceedings of the AAAI Conference on Artificial Intelligence. Vol. 36. No. 8. 2022.
