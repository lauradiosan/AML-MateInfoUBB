# Advanced Machine Learning 2026-2027 


## Lectures

1. Lecture 1

2. Lecture 2

...


## About projects

The project you have to do is an opportunity to explore an Artificial Intelligence (AI) problem in the context of real data. The project will be evaluated both during the semester and at the end of the semester, when each team will have to present to the teaching staff the corresponding iterations of the application and the related technical report.

**Suggested topics:**
<!-- 
<details>
    <summary> 1. Title  </summary>

**Aim** 

**Data**

**Bibliografy**

</details> -->

<details>
    <summary> 1. AI Radiology Assistant for Virtual Biopsy of Lung Cancer  </summary>

**Aim** Develop an intelligent multi-agent system that supports radiologists in the early assessment of lung cancer from CT scans. 
The project should evolve through several stages:
- Build a baseline classifier for tumor characterization.
- Develop a multi-task model that simultaneously predicts: malignancy risk; tumor subtype; actionable biomarkers.
- Investigate advanced architectures based on Vision Transformers and deformable attention.
- Build a RAG system able to retrieve relevant medical evidence from scientific articles and clinical guidelines.
- Develop a team of agents (e.g.Image Analysis Agent; Biomarker Prediction Agent; Literature Retrieval Agent; Clinical Reasoning Agent; Report Generation Agent)
The final result should simulate the behavior of a junior radiology decision-support assistant.

**Data** Primary datasets:
- LIDC-IDRI - Lung CT Scans with radiologist annotations [link](https://www.cancerimagingarchive.net/collection/lidc-idri/)

- LNDb - Lung Nodule Database (European cohort; includes malignancy likelihood scores) [link](https://lndb.grand-challenge.org/)

**Bibliography**
1. Crawshaw, M. (2020). Multi-task learning with deep neural networks: A survey. arXiv preprint arXiv:2009.09796.

2. Zhang, Y., & Yang, Q. (2021). A survey on multi-task learning. IEEE transactions on knowledge and data engineering, 34(12), 5586-5609.

3. Silva, F.A. et al. LNDb: A Lung Nodule Database on Computed Tomography. IEEE Transactions on Medical Imaging, 2020

</details>

<details>
    <summary> 2. Federated Multi-Agent Breast Cancer Diagnosis from Mammographic Images </summary>

**Aim** Develop a federated AI system capable of learning from distributed mammography datasets while preserving privacy. The project should investigate:
CNN baseline models, 
Vision Transformers and hybrid CNN-ViT architectures, 
Explainable AI techniques, 
Federated Learning approaches, 
Multi-agent collaboration among hospitals.

The final architecture may include: Local Hospital Agent, Federated Coordinator Agent, Explainability Agent, Quality Control Agent, Report Generation Agent.
THe project should assess: predictive performance, communication cost, model robustness, explainability quality.

**Data**
- MIAS
- CBIS-DDSM
- INBreast

**Bibliografy**

</details> 

<details>
    <summary> 3. AI-Enabled Cardiac Digital Twin from Wearable Sensors </summary>

**Aim** Develop an intelligent cardiac digital twin that integrates wearable ECG measurements, physiological modeling and autonomous diagnostic agents. 
The project should investigate: ECG classification, signal denoising, time-series transformers, digital twin modeling, multi-agent monitoring systems.
Possible architecture: Signal Monitoring Agent; Arrhythmia Detection Agent; Physiological Prediction Agent; Twin Calibration Agent; Clinical Recommendation Agent.

**Data**
Physionet ECG datasets.
Wearable ECG records.
Smartwatch physiological signals.
MIT-BIH Arrhythmia Database.

**Bibliografy**
Bhavsar et al., Digital Biomarkers Using Smartwatch Data, 2021.
Del-Valle-Soto et al., Wearables and Biometric Applications, 2024.
Thangtodoaraj et al., Cardiovascular Care with Digital Twin Technology, 2024.
Simonian et al., Mitral Valve Digital Twin, 2025.
Lim et al., Time Series Transformer, 2021.

</details> 




**Project components**
- short description 
- team (max 3 members)
- problem solving by AI/ML-based algorithms and the application development 
    - Problem definition (details about inputs and outputs)
    - Exploratory data analysis
    - AI development and performance evaluation 
    - Improvements 
- documentation (technical report)
- final presentation

**Performance of the AI models**
1. Performance
    - qualitative (errors, accuracy, precision, IoU, Dice, etc.)
    - complexity (time, space/memory, FLOPs, hardware resources, etc.)
2. Explainability
3. Sustainability
4. Ethics, transparency, contestability

**Application development**
- using any programming language and technologies 
- codebases must be submitted [here](https://classroom50.org/LauraDiosan-CS/aml-2026-2027/assignments/aml-project/accept), before deadlines


**Technical report**
- must follows this template [link](Report/texModel/model.tex) and the recommended structure [link](Report/readme.md). 
- latex sources and pdf file must be pushed in the previous repo (a folder for app, a folder for documentation)


**Final presentation**
- teaser (a short video presentation)
- slides (or other presentation support)
- project defense (oral presentation of aprox. 15 minutes based on the prepared slides/support)


**Evaluation**
- [criteria and points](Eval/readme.md)
