# Advanced Machine Learning 2026-2027 


## Lectures

1 - intro & adminstrative details

2 - Machine Learning - recap 

3 - Generative AI - Transformer-based models for processing textual, visual, audio, code data

4 - Diffusion models  

5 - Reinforcement Learning 

6 - Agents 

7 - RAG

8 - Agentic AI

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
    <summary> 1. Mosaic of Evidence: Multi-Agent AI for Lung Cancer Virtual Biopsy and Clinical Decision Support  </summary>

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
    <summary> 2. Women's Health Intelligence: A Federated Multi-Agent Framework for Breast Cancer Detection </summary>

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


<details>
    <summary> 4. LLM Security Guardian: OWASP Top 10 for LLM Applications Checker (Owner: Laura Cernau, Marsh)    </summary>

**Aim** More and more applications embed large language models through chatbots, RAG pipelines, agents and copilots. These integrations add new kinds of vulnerabilities that traditional static analysis tools don't detect, such as prompt injection, leaked system prompts and over-privileged agents. The OWASP Top 10 for LLM Applications catalogues these risks, but checking a codebase against it is still largely manual. 

Design an AI-driven solution that analyses a code repository and reports whether it follows the OWASP Top 10 for LLM Applications. For each violation or weakness, it should give the file and line, an explanation, the severity, and a suggested fix. 
Detect risks such as:  
- Prompt injection: user input concatenated into prompts without separation or sanitisation 
- Sensitive information disclosure: secrets, PII or internal data sent to the model or returned in responses 
- Supply chain: unpinned or unverified models, plugins and dependencies 
- Improper output handling: LLM output passed directly to eval, SQL, shell commands or HTML rendering 
- Excessive agency: agents with broad tool permissions, write or delete access, or no human approval step 
- System prompt leakage: credentials or business logic embedded in system prompts 
- Vector and embedding weaknesses: RAG stores without access control or tenant isolation 
- Unbounded consumption: missing rate limits, token caps or timeouts 

Support several common stacks, for example:  
- Python (LangChain, LlamaIndex, OpenAI or Anthropic SDKs) 
- TypeScript or Node.js (Vercel AI SDK, LangChain.js) 

Produce output as:  
- A structured report (SARIF, JSON or Markdown) 
- A compliance scorecard per OWASP category 

Advanced exploration: 
- Integrate the checker into a GitHub merge request workflow to:  
    - Scan only the changed code and comment inline on risky lines 
    - Block merges when critical findings are present 
- Generate remediation patches automatically, such as input guards, output encoding or permission scoping. 
- Build a small deliberately vulnerable LLM app as a benchmark and measure detection rates. 
- Compare rule-based detection (Semgrep or CodeQL rules) with LLM-based semantic analysis, and with a hybrid of the two. 
- Add dynamic testing: generate adversarial prompts against the running app to confirm whether static findings can actually be exploited. 

**Bibliografy**
- Fourati, L. C., Awad, M., Ben Ali, M., & Jaafar, W. (2026). Large language models for cyberattack defense: a critical survey: L. Fourati et al. Knowledge and Information Systems, 68(1), 113 [link](https://dl.acm.org/doi/10.1007/s10115-026-02736-y).
- Wang, X., Huang, K., Liang, B., Li, H., & Du, X. (2026, March). Shadows in the Code: Exploring the Risks and Defenses of LLM-based Multi-Agent Software Development Systems. In Proceedings of the AAAI Conference on Artificial Intelligence (Vol. 40, No. 44, pp. 37970-37978) [link](https://dl.acm.org/doi/10.1609/aaai.v40i44.41134).
</details>


<details>
    <summary> 5. Compliance-as-Code AI Auditor Checking Applications Against Policies and Regulations (e.g., EU AI Act) </summary>


**Aim** Organisations must show that their applications comply with a growing set of regulations, such as the EU AI Act and GDPR, and with internal policies such as data retention, security standards and responsible AI guidelines. These rules are written in natural language, but evidence of compliance is spread across code, configuration, infrastructure, documentation and logs. As a result, compliance checks tend to be manual, infrequent and disconnected from the development lifecycle. 

Design a system that takes a policy or regulation as input and checks whether an application complies with it. The system should break the policy down into verifiable requirements, collect evidence from the application, and produce an auditable compliance report that links every requirement to evidence or to a gap. 
Scope ideas: 
- Ingest policies from:  
    - Regulatory texts (e.g., EU AI Act articles and annexes) 
    - Internal company policies and standards 
    - Checklists or control frameworks 
- Translate requirements into checkable rules, for example:  
    - Classifying the system by risk level (prohibited, high-risk, limited-risk, minimal-risk) 
    - Transparency: are users informed that they are interacting with an AI system, and is AI-generated content labelled? 
    - Record-keeping: are model decisions and inputs logged and retained appropriately? 
    - Human oversight: is there a mechanism for a human to review, override or stop the system? 
    - Data governance: is training and input data documented, and is personal data handled lawfully? 
    - Technical documentation: does it exist and is it up to date? 
- Collect evidence from:  
    - Source code and configuration 
    - Infrastructure-as-code (Terraform, Kubernetes manifests) 
    - Architecture documentation and ADRs 
    - Model cards, data sheets and READMEs 
- Express rules in formats such as:  
    - Open Policy Agent (Rego) 
    - Structured YAML or JSON rule definitions 
    - Natural-language rules evaluated by an LLM with evidence citations 

**Advanced exploration:** 
- Run compliance checks continuously in CI/CD, flagging when a change introduces a gap (for example, removing a logging call or adding a new AI feature without disclosure). 
- Generate missing compliance artefacts automatically, such as a draft technical documentation section or a risk assessment template. 
- Handle policy evolution: when a regulation or internal policy is updated, identify which applications and requirements are affected. 
- Compare deterministic policy-as-code checks with LLM-based interpretation of ambiguous requirements, and design a human-in-the-loop step for borderline cases. 
- Make the system itself trustworthy: explainable verdicts, traceable evidence, and no hallucinated compliance claims. 

</details>

<details>
    <summary> 6. DeXMed: A Multi-Agent Ecosystem for Collaborative Clinical Intelligence</summary>  

**Aim** DeXMed is a planned orchestration and clinical workflow platform in which each medical specialization is an independently deployable clinical AI service. The target architecture separates four concerns: 
- Presentation: a Clinical Web Application for doctors, specialists and patients 
- Orchestration: the DeXMed Orchestrator, which manages clinical workflows, coordinates access to patient information, invokes AI services and aggregates their results 
- Shared Patient Context: a General Patient Database holding patient information shared across the platform 

Medical Intelligence: independent Medical AI Services, one per specialization, starting with ORL and Breast Cancer 

The central architectural goal is extensibility. A new specialization (e.g., Cardiology) must be addable as a new service without changing the core platform, and specialization-specific logic must never leak into the orchestrator. 

Desired outcome: Propose and implement the DeXMed platform from this target architecture. This means: 
- Refining the architecture into concrete design decisions (technologies, APIs, data models, deployment) 
- Building a working end-to-end prototype with all four layers and the two initial AI services 
- Showing that the platform is extensible by adding a third specialization with no changes to the core 

Scope ideas: 
- Clinical Web Application:  
    - Doctor/specialist views: create and manage clinical workflows, review, validate or reject AI-assisted findings 
    - Patient views: see their medical record and the recommendations their doctors have validated 
    - Role-based access: doctors, specialists and patients see different data and actions 
    - Communicates only with the orchestrator 
- DeXMed Orchestrator:  
    - Clinical workflow management (e.g., a workflow engine or explicit state machine) 
    - A specialization plugin contract: a standard API, capability manifest, and input/output schemas 
    - Dynamic registration and discovery of AI services, with no specialization hard-coded 
    - Controlled access to patient data: each AI service receives only what it needs 
    - Aggregation of results from several specializations into one clinical view 
- General Patient Database:  
    - Data model for shared patient context, ideally based on interoperable standards 
    - A clear separation from specialization-specific data, which stays inside each AI service 
- Medical AI Services:  
    - ORL and Breast Cancer services implementing the plugin contract 
    - The AI logic can be based on public models and datasets. 
    - Findings returned with confidence levels and explanations to support the doctor's review 
- Use synthetic or publicly available anonymised data. 

**Advanced exploration:**
- Write architecture fitness functions that run in CI and fail the build when a boundary is violated, such as the web app calling an AI service directly, a dependency between two specializations, or specialization logic appearing in the orchestrator. 
- Provide a scaffolding template that generates a new specialization service already compliant with the plugin contract. 
- Make the platform resilient: timeouts, circuit breakers and graceful degradation when one specialization is unavailable. 
- Version the plugin contract so specializations can evolve independently. 
- Handle conflicting or overlapping findings from different specializations. 
- Add trustworthy-AI mechanisms: audit logs of every AI invocation, mandatory human validation before results reach patients, and traceability of model versions (relevant to the EU AI Act, GDPR and medical device regulation). 

</details>

<details>
    <summary> 7. Farma projects </summary>  
- Details [link](2026-2027\NagarroChallengesUBB.pdf)

</details>


**Project components**
- short description 
- team (max 3 members; each member should performed at least 2 PR for each stage of the project development - both app & technical report) 
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
- codebases must be:
    - presented in a live way to the supervisor (demo) 
    - submitted [here](https://classroom50.org/LauraDiosan-CS/aml-2026-2027/assignments/aml-project/accept), before deadlines


**Technical report**
- must follows this template [link](Report/texModel/model.tex) and the recommended structure [link](Report/readme.md). 
- latex sources and pdf file must be pushed in the previous repo (a folder for app, a folder for documentation) before the specified deadlines


**Final presentation**
- teaser (a short video presentation)
- slides (or other presentation support)
- project defense (oral presentation of aprox. 15 minutes based on the prepared slides/support)
- app demo 

**Evaluation**
- [criteria and points](Eval/readme.md)
