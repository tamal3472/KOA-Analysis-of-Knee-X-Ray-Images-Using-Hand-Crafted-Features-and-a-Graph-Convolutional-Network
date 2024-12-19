# KOA-Analysis-of-Knee-X-Ray-Images-Using-Hand-Crafted-Features-and-a-Graph-Convolutional-Network

**Abstract**—Knee osteoarthritis (KOA) is a common cause of
disability, especially in the elderly and obese, affecting large joints
such as the knee, hip, and spine. Manual diagnosis of knee images
is time-consuming and error-prone, highlighting the need for an
automated system. In addition, there is a limited exploration of
combining graphical models with hand-crafted features for KOA
detection. This study presents a new auto-combined approach for
KOA detection that integrates hand-crafted features with a graph
convolutional network (GCN) model. Furthermore, it addresses
challenges such as noise, artifacts, and low image quality using a
digital knee X-ray dataset, which includes 1,650 images across five
KOA grades (0-4). Advanced image preprocessing techniques, in-
cluding LAB color space transformation, histogram equalization
(HE), and fast non-local mean denoising (FNLM), were applied
while image quality was improved by preserving structural
details. Twenty-three artifact features covering morphological,
texture, and structural aspects were extracted and ranked based
on their relevance to KOA grade using ANOVA and correlation
analysis. The GCN model was built with graph convolution layers,
batch normalization, dropout regularization, and optimization
techniques for classification. The GCN model outperformed
other architectures, including graph neural networks (GNN) and
graph attention networks (GAT), achieving 0.92 accuracy, 0.9101
sensitivity, and 0.9003 F1-score with an optimal feature set of
11 features. In contrast, GNN and GAT models showed lower
performance metrics, demonstrating the effectiveness of the GCN
approach. Therefore, it can be claimed that this study highlights
the potential of integrating handcrafted features with graph-
based models to pave the way for KOA diagnosis.


## Dataset 

This study utilizes the publicly available dataset https://www.kaggle.com/datasets/tommyngx/digital-knee-xray?select=MedicalExpert-I, Digital
Knee X-ray, which contains 1,650 images of five grades,
including grade 0 (Normal), grade 1 (Doubtful), grade 2
(Mild), grade 3 (Moderate), and grade 4 (Severe). These images are 8-bit grayscale and were acquired using the PROTEC
PRS 500E X-ray machine. Two medical experts manually
annotated and labeled each knee X-ray image in the dataset
according to Kellgren and Lawrence’s grades.

<img width="2907" alt="Untitled (4)" src="https://github.com/user-attachments/assets/bfcb0670-9e3f-47f7-afc3-a521c66e1a43" />


## Metholodology

![Main Workflow](https://github.com/user-attachments/assets/58b620f0-a47a-40cc-b4b1-a1edddda26b4)
