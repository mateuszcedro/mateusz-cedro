# Mateusz Cedro
## About Me
I’m a second-year PhD student in **Explainable AI** at the **University of Antwerp (Belgium)**, supervised by [Prof. David Martens](https://scholar.google.com/citations?user=gbce1doAAAAJ&hl=en).

My current focus is on:
- **Mechanistic Interpretability** — understanding AI model behaviour by investigating internal components (individual neurons, attention heads, layers, activations) and reverse-engineering learned computational circuits to explain how and why models produce specific outputs.
- **AI Alignment** — aligning model objectives and behaviours with human values and safety constraints.
- **Concept Discovery in Large AI Models** — understanding the **concepts learned by large AI downstream models**, including concepts that may be **beyond current human understanding** (see e.g. [Schut et al., 2025](https://www.pnas.org/doi/10.1073/pnas.2406675122)).

I care about building transparent, reliable ML systems and turning model internals into understandable, human-legible explanations.

- 📄 Publications: [Google Scholar](https://scholar.google.com/citations?user=srXiChUAAAAJ&hl=en)
- 🧑‍🏫 Supervisor: [Prof. David Martens](https://scholar.google.com/citations?user=gbce1doAAAAJ&hl=en)
- 🧑‍🔬 Former advisor: [Prof. Przemyslaw Biecek](https://scholar.google.com/citations?hl=en&user=Af0O75cAAAAJ)
- 📍 Antwerp, Belgium

> Always happy to connect on collaborations around interpretability, alignment, and concept discovery.

## My projects
### Mechanistic Interpretability - Counterfactual circuits behind “Yes/No” decisions in Llama
**Doc:** ➡️ [Key Takeaways & Write-up](https://docs.google.com/document/d/1vl4r1zME4O-xJyCbhn2_OQ3wzJUynhxm5nxplA6XGuA/edit?usp=sharing)

**What this investigates:**  
Trade-off prompts like *“Do you accept **X** euros to wait an additional **Y** minutes?”* on **Llama-3.2-3B-Instruct**, analyzing token-level behavior for **Yes/No**. It is a mechanistic interpretability follow-up on [Cash or Comfort? How LLMs Value Your Inconvenience](https://arxiv.org/pdf/2506.17367) (Cedro et al., 2025)

**Core findings:**
- A single **MLP output layer (21)** steers “No”: **mean-ablation flips** model decisions from *No → Yes*.
- Within that layer, **neuron 8190** strongly pushes toward “No”; **zero-ablating it flips** the decision (acts as a **counterfactual neuron**).
- **MLP layers** dominate **logit attributions** for “Yes/No” over attention heads.
- **Interference emerges a few layers later**: probability shifts appear ~**layers 24+** after the ablation.
- Behavior shows **systematic anomalies**: rejections at **powers of 10** (€10, €100, €1,000), occasional **greediness** (accepting €0.10 for 600 minutes), and **no freebie dilemma**.

**Why it matters:**  
Points to compact, targetable circuits for preference-like judgments; suggests concept-level control via sparse, layer-localised edits.


### Vision Transformer (ViT)
- [Building Vision Transformer (ViT) from Scratch with PyTorch - replication of *An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale* (Dosovitskiy et al., 2020) research paper](https://github.com/mateuszcedro/mateuszcedro/blob/main/Deep%20Learning%20in%20PyTorch/Vision%20Transformer%20(ViT)%20from%20scratch%20with%20PyTorch.ipynb)

![ViT](https://raw.githubusercontent.com/mateuszcedro/mateusz-cedro/main/Deep%20Learning%20in%20PyTorch/img/vit.png)

### Explainable AI (XAI)
- [Explainable AI - Explanation of XGBoost & SVM models of Brain Stroke disease prediction](https://github.com/mateuszcedro/mateusz-cedro/blob/main/Explainable%20AI/XAI_Shap_BrainStroke_notebook.ipynb)

![XAI_BrainStroke4](https://github.com/mateuszcedro/mateusz-cedro/blob/main/Explainable%20AI/xai_4.png)
![XAI_BrainStroke1](https://github.com/mateuszcedro/mateusz-cedro/blob/main/Explainable%20AI/xai_1.png)
![XAI_BrainStroke2](https://github.com/mateuszcedro/mateusz-cedro/blob/main/Explainable%20AI/xai_2.png)

### Generative AI
- [Generative Adversarial Networks (GANs)](https://github.com/mateuszcedro/mateusz-cedro/blob/main/Generative%20AI/GAN.ipynb)

![gan_img](https://github.com/mateuszcedro/mateusz-cedro/blob/main/Generative%20AI/gan_imgs/GAN_img.png)

- Segment Anything Model (SAM) by Meta AI on Medical Images

### Deep Learning
- [Computer Vision Classification Model and XAI Explanations with PyTorch](https://github.com/mateuszcedro/mateusz-cedro/blob/main/Deep%20Learning%20in%20PyTorch/XAI-ResNet50-notebook.ipynb)
- [Computer Vision Classification Model from Scratch with PyTorch](https://github.com/mateuszcedro/mateusz-cedro/blob/main/Deep%20Learning%20in%20PyTorch/Computer%20Vision%20Classification%20Model%20from%20Scratch%20with%20PyTorch.ipynb)

### Machine Learning
- [Time-series predictions with LSTM Model in PyTorch](https://github.com/mateuszcedro/mateusz-cedro/blob/main/Machine%20Learning%20in%20PyTorch/LSTM%20Time-Series%20Model%20in%20PyTorch.ipynb)

![lstm](https://github.com/mateuszcedro/mateusz-cedro/blob/main/Machine%20Learning%20in%20PyTorch/imgs/time-series%20LSTM.png)

- [Multiclass Neural Network Classification Model from Scratch with PyTorch](https://github.com/mateuszcedro/mateusz-cedro/blob/main/Machine%20Learning%20in%20PyTorch/Neural%20Network%20Multiclass%20Classification%20Model%20from%20Scratch%20with%20PyTorch.ipynb)

![multiclass1](https://github.com/mateuszcedro/mateusz-cedro/blob/main/Machine%20Learning%20in%20PyTorch/imgs/Multiclass_1.png)
![multiclass2](https://github.com/mateuszcedro/mateusz-cedro/blob/main/Machine%20Learning%20in%20PyTorch/imgs/Multiclass_2.png)

- [Binary Neural Network Classification Model from Scratch with PyTorch](https://github.com/mateuszcedro/mateusz-cedro/blob/main/Machine%20Learning%20in%20PyTorch/Neural%20Network%20Binary%20Classification%20Model%20from%20Scratch%20with%20PyTorch.ipynb)
- [Linear Regression Model from Scratch with PyTorch](https://github.com/mateuszcedro/mateusz-cedro/blob/main/Machine%20Learning%20in%20PyTorch/Linear%20Regression%20Model%20from%20Scratch%20with%20PyTorch.ipynb)

### Advanced Data Visualisation
- [Advanced Visualisation](https://github.com/mateuszcedro/mateusz-cedro/blob/main/Visualisation/Advanced%20Visualisation.md)

![Adv_Viz1](https://github.com/mateuszcedro/mateusz-cedro/blob/main/Visualisation/Plots/s10.png)
![Adv_Viz2](https://github.com/mateuszcedro/mateusz-cedro/blob/main/Visualisation/Plots/s3.png)

### Natural Language Processing
- [Sentiment Analysis & Topic Modeling](https://htmlpreview.github.io/?https://github.com/mateuszcedro/mateusz-cedro/blob/main/NLP/Sentiment%20Analysis%20%26%20Topic%20Modeling.html)
- [Clustering & Topic Modeling](https://htmlpreview.github.io/?https://github.com/mateuszcedro/mateusz-cedro/blob/main/NLP/Clustering%20%26%20Topic%20Modeling.html)


<!---
mateuszcedro/mateuszcedro is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
