# Awesome-LLM-SoftwareTesting

A collection of papers and resources about the utilization of large language models (LLMs) in software testing.

Software testing is a critical task that is essential for ensuring the quality and reliability of software products. As software systems become increasingly complex, new and more effective software testing techniques are needed. Recently, large language models (LLMs) have emerged as a breakthrough technology in natural language processing and artificial intelligence. These models are capable of performing various coding-related tasks, including code generation and code recommendation. Therefore, the use of LLMs in software testing is expected to yield significant improvements. On one hand, software testing involves tasks such as unit test generation that require code understanding and generation. On the other hand, LLMs can generate diverse test inputs to ensure comprehensive coverage of the software being tested. In this repository, we present a comprehensive review of the utilization of LLMs in software testing. We have collected 102 relevant papers and conducted a thorough analysis from both software testing and LLMs perspectives, as summarized in Figure 1.

![Figure 1. Structure of the contents in this paper](https://raw.githubusercontent.com/LLM-Testing/llm-testing.github.io/main/figures/1.png)

We hope this repository can help researchers and practitioners to get a better understanding of this emerging field. If this repository is helpful for you, please help us by citing this paper:

```
@article{Wang2023SoftwareTW,
  title={Software Testing with Large Language Model: Survey, Landscape, and Vision},
  author={Junjie Wang and Yuchao Huang and Chunyang Chen and Zhe Liu and Song Wang and Qing Wang},
  journal={ArXiv},
  year={2023},
  volume={abs/2307.07221},
  url={https://api.semanticscholar.org/CorpusID:259924919}
}
```

## Table of Contents📇
- [Awesome-LLM-SoftwareTesting](#awesome-llm-softwaretesting)
  - [News](#news)
  - [Overview](#overview)
    - [From software testing perspective](#from-software-testing-perspective)
    - [From LLM perspective](#from-llm-perspective)
  - [Related Surveys](#related-surveys)
  - [Unit test case generation](#unit-test-case-generation)
  - [Test oracle generation](#test-oracle-generation)
  - [System test input generation](#system-test-input-generation)
  - [Bug analysis](#bug-analysis)
  - [Debug](#debug)
  - [Program repair](#program-repair)

## News🎉
This project is under development. You can hit the **STAR** and **WATCH** to follow the updates.

- Our LLM for mobile GUI testing paper: [*Make LLM a Testing Expert: Bringing Human-like Interaction to Mobile GUI Testing via Functionality-aware Decisions*](https://arxiv.org/abs/2310.15780) is accepted by ICSE 2024. Note that, it is a follow-up work of [*Chatting with GPT-3 for Zero-Shot Human-Like Mobile Automated GUI Testing*](https://arxiv.org/abs/2305.09434).
- Our LLM for text input fuzzing paper: [*Testing the Limits: Unusual Text Inputs Generation for Mobile App Crash Detection with Large Language Model*](https://arxiv.org/abs/2310.15780) is accepted by ICSE 2024. 
- Our LLM for crash reproduction paper: [*CrashTranslator: Automatically Reproducing Mobile Application Crashes Directly from Stack Trace*](https://arxiv.org/abs/2310.07128) is accepted by ICSE 2024.
- Our LLM for semantic text input generation paper: [*Fill in the Blank: Context-aware Automated Text Input Generation for Mobile GUI testing*](https://ieeexplore.ieee.org/document/10172490) is published in ICSE 2023.
- Our roadmap paper：[*Software Testing with Large Language Models: Survey, Landscape, and Vision*](https://arxiv.org/abs/2307.07221) is now public.

## Overview🔭

### From software testing perspective

![Figure 2. Distribution of testing tasks with LLMs](https://raw.githubusercontent.com/LLM-Testing/llm-testing.github.io/main/figures/2.png)

We find that LLMs have proven to be efficient in the mid to late stages of the software testing lifecycle. During the mid-phase of software testing, LLMs have been successfully applied for various test case preparation tasks, including the generation of unit test cases, test oracle generation, and system test input generation. In later phases, such as the bug fix phase and the preparation of test reports/bug reports, LLMs have been utilized for tasks like bug analysis, debugging, and repair.

### From LLM perspective

<div align=center>
    <img src="https://raw.githubusercontent.com/LLM-Testing/llm-testing.github.io/main/figures/3.png"/>
</div>


In our collected studies, the LLM most frequently employed is ChatGPT, widely recognized and popular for its exceptional performance across various tasks. The second most commonly used LLM is Codex, trained on an extensive code corpus, aiding researchers in coding-related tasks. Ranked third is CodeT5, an open-source LLM capable of conducting pre-training and fine-tuning with domain-specific data, thereby achieving better performance.

![Figure 4. Distribution about how LLM is used (prompt engineering)](https://raw.githubusercontent.com/AwesomeLLMSoftwareTesting/awesomellmsoftwaretesting.github.io/main/figures/4.png)

In our collected studies, 38 studies utilize the LLMs through pre-training or fine-tuning schema, while 64 studies employ the [prompt engineering](https://www.promptingguide.ai/) to communicate with LLMs to steer its behavior for desired outcomes without updating the model weights. Among them, 51 studies involve [zero-shot learning](https://www.promptingguide.ai/techniques/zeroshot), and 25 studies involve [few-shot learning](https://www.promptingguide.ai/techniques/fewshot). There are also studies involving the [chain-of-thought](https://www.promptingguide.ai/techniques/cot) (7 studies), [self-consistency](https://www.promptingguide.ai/techniques/consistency) (1 study), and [automatic prompt](https://www.promptingguide.ai/techniques/ape) (1 study).

![Figure 5. Distribution about other techniques incorporated with LLMs](https://raw.githubusercontent.com/AwesomeLLMSoftwareTesting/awesomellmsoftwaretesting.github.io/main/figures/5.png)

In our collected studies, 67 of them utilize LLMs to address the entire testing task, while 35 studies incorporate additional techniques. These techniques include mutation testing, differential testing, syntactic checking, program analysis, statistical analysis, etc. .

## Related Surveys🗎
- [Large Language Models for Software Engineering A Systematic Literature Review](https://arxiv.org/abs/2308.10620) (in Arxiv)
- [Large Language Models for Software Engineering Survey and Open Problems](https://arxiv.org/abs/2310.03533) (in Arxiv)
- [Large Language Models Meet NL2Code A Survey](https://aclanthology.org/2023.acl-long.411/) (in ACL 2023)

## Unit test case generation
- [Unit Test Case Generation with Transformers and Focal Context](https://arxiv.org/abs/2009.05617) (in Arxiv)
- [Codet: Code Generation with Generated Tests](https://openreview.net/pdf?id=ktrw68Cmu9c) (in ICLR 2023)
- [Interactive Code Generation via Test-Driven User-Intent Formalization](https://arxiv.org/abs/2208.05950) (in Arxiv)
- [A3Test: Assertion-Augmented Automated Test Case Generation](https://arxiv.org/abs/2302.10352) (in Arxiv)
- [An Empirical Evaluation of Using Large Language Models for Automated Unit Test Generation](https://arxiv.org/abs/2302.06527) (in Arxiv)
- [An Initial Investigation of ChatGPT Unit Test Generation Capability](https://dl.acm.org/doi/10.1145/3624032.3624035) (in SAST 2023)
- [Automated Test Case Generation Using Code Models and Domain Adaptation](https://arxiv.org/abs/2308.08033) (in Arxiv)
- [Automatic Generation of Test Cases based on Bug Reports: a Feasibility Study with Large Language Models](https://arxiv.org/abs/2310.06320) (in Arxiv)
- [Can Large Language Models Write Good Property-Based Tests?](https://arxiv.org/abs/2307.04346) (in Arxiv)
- [CAT-LM Training Language Models on Aligned Code And Tests](https://ieeexplore.ieee.org/document/10298372) (in ASE 2023)
- [ChatGPT vs SBST: A Comparative Assessment of Unit Test Suite Generation](https://arxiv.org/abs/2307.00588) (in Arxiv)
- [ChatUniTest: a ChatGPT-based Automated Unit Test Generation Tool](https://arxiv.org/abs/2305.04764) (in Arxiv)
- [CODAMOSA: Escaping Coverage Plateaus in Test Generation with Pre-trained Large Language Models](https://ieeexplore.ieee.org/document/10172800) (in ICSE 2023)
- [Effective Test Generation Using Pre-trained Large Language Models and Mutation Testing](https://arxiv.org/abs/2308.16557) (in Arxiv)
- [Exploring the Effectiveness of Large Language Models in Generating Unit Tests](https://arxiv.org/abs/2305.00418) (in Arxiv)
- [How Well does LLM Generate Security Tests?](https://arxiv.org/abs/2310.00710) (in Arxiv)
- [No More Manual Tests? Evaluating and Improving ChatGPT for Unit Test Generation](https://arxiv.org/abs/2305.04207) (in Arxiv)
- [Prompting Code Interpreter to Write Better Unit Tests on Quixbugs Functions](https://arxiv.org/abs/2310.00483) (in Arxiv)
- [Reinforcement Learning from Automatic Feedback for High-Quality Unit Test Generation](https://arxiv.org/abs/2310.02368) (in Arxiv)
- [Unit Test Generation using Generative AI: A Comparative Performance Analysis of Autogeneration Tools](https://arxiv.org/abs/2312.10622) (in Arxiv)

## Test oracle generation
- [Generating Accurate Assert Statements for Unit Test Cases Using Pretrained Transformers](https://dl.acm.org/doi/abs/10.1145/3524481.3527220) (in AST 2022)
- [Learning Deep Semantics for Test Completion](https://ieeexplore.ieee.org/document/10172620/) (in ICSE 2023)
- [Using Transfer Learning for Code-Related Tasks](https://dl.acm.org/doi/10.1109/TSE.2022.3183297) (in TSE 2022)
- [Retrieval-Based Prompt Selection for Code-Related Few-Shot Learning](https://ieeexplore.ieee.org/abstract/document/10172590) (in ICSE 2023)

## System test input generation
- [Automated Conformance Testing for JavaScript Engines via Deep Compiler Fuzzing](https://dl.acm.org/doi/10.1145/3453483.3454054) (in PLDI 2021)
- [Fill in the Blank: Context-aware Automated Text Input Generation for Mobile GUI Testing](https://ieeexplore.ieee.org/document/10172490/) (in ICSE 2023)
- [Large Language Models are Pretty Good Zero-Shot Video Game Bug Detectors](https://arxiv.org/abs/2210.02506) (in Arxiv)
- [Slgpt: Using Transfer Learning to Directly Generate Simulink Model Files and Find Bugs in the Simulink Toolchain](https://dl.acm.org/doi/10.1145/3463274.3463806) (in EASE 2021)
- [Augmenting Greybox Fuzzing with Generative AI](https://arxiv.org/abs/2306.06782) (in Arxiv)
- [Automated Test Case Generation Using T5 and GPT-3](https://ieeexplore.ieee.org/document/10112971/) (in ICACCS 2023)
- [Automating GUI-based Software Testing with GPT-3](https://ieeexplore.ieee.org/document/10132233/) (in ICSTW 2023)
- [AXNav: Replaying Accessibility Tests from Natural Language](https://arxiv.org/abs/2310.02424) (in Arxiv)
- [Can ChatGPT Advance Software Testing Intelligence? An Experience Report on Metamorphic Testing](https://arxiv.org/abs/2310.19204) (in Arxiv)
- [Efficient Mutation Testing via Pre-Trained Language Models](https://arxiv.org/abs/2301.03543) (in Arxiv)
- [Large Language Models are Edge-Case Generators:Crafting Unusual Programs for Fuzzing Deep Learning Libraries](https://arxiv.org/abs/2304.02014) (in ICSE 2024)
- [Large Language Models are Zero Shot Fuzzers: Fuzzing Deep Learning Libraries via Large Language Models](https://dl.acm.org/doi/abs/10.1145/3597926.3598067) (in ISSTA 2023)
- [Large Language Models for Fuzzing Parsers (Registered Report)](https://dl.acm.org/doi/10.1145/3605157.3605173) (in FUZZING 2023)
- [LLM for Test Script Generation and Migration: Challenges, Capabilities, and Opportunities](https://arxiv.org/abs/2309.13574) (in Arxiv)
- [Make LLM a Testing Expert: Bringing Human-like Interaction to Mobile GUI Testing via Functionality-aware Decisions](https://arxiv.org/abs/2310.15780) (in ICSE 2024)
- [PentestGPT: An LLM-empowered Automatic Penetration Testing Tool](https://arxiv.org/abs/2308.06782) (in Arxiv)
- [SMT Solver Validation Empowered by Large Pre-Trained Language Models](https://ieeexplore.ieee.org/document/10298442/) (in ASE 2023)
- [TARGET: Automated Scenario Generation from Traffic Rules for Testing Autonomous Vehicles](https://arxiv.org/abs/2305.06018) (in Arxiv)
- [Testing the Limits: Unusual Text Inputs Generation for Mobile App Crash Detection with Large Language Model](https://arxiv.org/abs/2310.15657) (in ICSE 2024)
- [Understanding Large Language Model Based Fuzz Driver Generation](https://arxiv.org/abs/2307.12469) (in Arxiv)
- [Universal Fuzzing via Large Language Models](https://arxiv.org/abs/2308.04748) (in ICSE 2024)
- [Variable Discovery with Large Language Models for Metamorphic Testing of Scientific Software](https://dl.acm.org/doi/10.1007/978-3-031-35995-8_23) (in SANER 2023)
- [White-box Compiler Fuzzing Empowered by Large Language Models](https://arxiv.org/abs/2310.15991) (in Arxiv)

## Bug analysis
- [Itiger: an Automatic Issue Title Generation Tool](https://dl.acm.org/doi/10.1145/3540250.3558934) (in FSE 2022)
- [CrashTranslator: Automatically Reproducing Mobile Application Crashes Directly from Stack Trace](https://arxiv.org/abs/2310.07128) (in ICSE 2024)
- [Cupid: Leveraging ChatGPT for More Accurate Duplicate Bug Report Detection](https://arxiv.org/abs/2308.10022) (in Arxiv)
- [Employing Deep Learning and Structured Information Retrieval to Answer Clarification Questions on Bug Reports](https://arxiv.org/abs/2304.12494) (in Arxiv)
- [Explaining Software Bugs Leveraging Code Structures in Neural Machine Translation](https://dl.acm.org/doi/10.1109/ICSE48619.2023.00063) (in ICSE 2023)
- [Prompting Is All Your Need: Automated Android Bug Replay with Large Language Models](https://arxiv.org/abs/2306.01987) (in ICSE 2024)
- [Still Confusing for Bug-Component Triaging? Deep Feature Learning and Ensemble Setting to Rescue](https://ieeexplore.ieee.org/abstract/document/10174001) (in ICPC 2023)

## Debug
- [Detect-Localize-Repair: A Unified Framework for Learning to Debug with CodeT5](https://aclanthology.org/2022.findings-emnlp.57/) (in EMNLP 2022)
- [Large Language Models are Few-shot Testers: Exploring LLM-based General Bug Reproduction](https://ieeexplore.ieee.org/document/10172763/) (in ICSE 2023)
- [A Preliminary Evaluation of LLM-Based Fault Localization](https://arxiv.org/abs/2308.05487) (in Arxiv)
- [Addressing Compiler Errors: Stack Overflow or Large Language Models?](https://arxiv.org/abs/2307.10793) (in Arxiv)
- [Can LLMs Demystify Bug Reports?](https://arxiv.org/abs/2310.06310) (in Arxiv)
- [Dcc --help: Generating Context-Aware Compiler Error Explanations with Large Language Models](https://arxiv.org/abs/2308.11873v2) (in SIGCSE 2024)
- [Explainable Automated Debugging via Large Language Model-driven Scientific Debugging](https://arxiv.org/abs/2304.02195) (in Arxiv)
- [Large Language Models for Test-Free Fault Localization](https://arxiv.org/abs/2310.01726) (in ICSE 2024)
- [Large Language Models in Fault Localisation](https://arxiv.org/abs/2308.15276) (in Arxiv)
- [LLM4CBI: Taming LLMs to Generate Effective Test Programs for Compiler Bug Isolation](https://arxiv.org/abs/2307.00593) (in Arxiv)
- [Nuances are the Key: Unlocking ChatGPT to Find Failure-Inducing Tests with Differential Prompting](https://ieeexplore.ieee.org/document/10298538/authors) (in ASE 2023)
- [Teaching Large Language Models to Self-Debug](https://arxiv.org/abs/2304.05128) (in Arxiv)
- [A study on Prompt Design, Advantages and Limitations of ChatGPT for Deep Learning Program Repair](https://arxiv.org/abs/2304.08191) (in Arxiv)

## Program repair
- [Using Transfer Learning for Code-Related Tasks](https://dl.acm.org/doi/10.1109/TSE.2022.3183297) (in TSE 2022)
- [Retrieval-Based Prompt Selection for Code-Related Few-Shot Learning](https://ieeexplore.ieee.org/abstract/document/10172590) (in ICSE 2023)
- [A study on Prompt Design, Advantages and Limitations of ChatGPT for Deep Learning Program Repair](https://arxiv.org/abs/2304.08191) (in Arxiv)
- [Examining Zero-Shot Vulnerability Repair with Large Language Models](https://ieeexplore.ieee.org/document/10179324/) (in SP 2023)
- [Automated Repair of Programs from Large Language Models](https://dl.acm.org/doi/10.1109/ICSE48619.2023.00128) (in ICSE 2023)
- [Fix Bugs with Transformer through a Neural-Symbolic Edit Grammar](https://arxiv.org/abs/2204.06643) (in Arxiv)
- [Practical Program Repair in the Era of Large Pre-trained Language Models](https://dl.acm.org/doi/10.1109/ICSE48619.2023.00129) (in ICSE 2023)
- [Repairing Bugs in Python Assignments Using Large Language Models](https://arxiv.org/abs/2209.14876) (in Arxiv)
- [Towards JavaScript Program Repair with Generative Pre-trained Transformer (GPT-2)](https://ieeexplore.ieee.org/abstract/document/9809071) (in APR 2022)
- [An Analysis of the Automatic Bug Fixing Performance of ChatGPT](https://ieeexplore.ieee.org/document/10189263/) (in APR 2023)
- [An Empirical Study on Fine-Tuning Large Language Models of Code for Automated Program Repair](https://ieeexplore.ieee.org/document/10298532/) (in ASE 2023)
- [An Evaluation of the Effectiveness of OpenAI's ChatGPT for Automated Python Program Bug Fixing using QuixBugs](https://ieeexplore.ieee.org/document/10295323/) (in iSemantic 2023)
- [An Extensive Study on Model Architecture and Program Representation in the Domain of Learning-based Automated Program Repair](https://ieeexplore.ieee.org/document/10189328) (in APR 2023)
- [Can OpenAI's Codex Fix Bugs? An Evaluation on QuixBugs](https://ieeexplore.ieee.org/abstract/document/9809175/) (in APR 2022)
- [CIRCLE: Continual Repair Across Programming Languages](https://dl.acm.org/doi/10.1145/3533767.3534219) (in ISSTA 2022)
- [Coffee: Boost Your Code LLMs by Fixing Bugs with Feedback](https://arxiv.org/abs/2311.07215) (in Arxiv)
- [Copiloting the Copilots: Fusing Large Language Models with Completion Engines for Automated Program Repair](https://dl.acm.org/doi/abs/10.1145/3611643.3616271) (in FSE 2023)
- [Domain Knowledge Matters: Improving Prompts with Fix Templates for Repairing Python Type Errors](https://arxiv.org/abs/2306.01394) (in ICSE 2024)
- [Enhancing Genetic Improvement Mutations Using Large Language Models](https://link.springer.com/chapter/10.1007/978-3-031-48796-5_13) (in SSBSE 2023)
- [FixEval: Execution-based Evaluation of Program Fixes for Programming Problems](https://ieeexplore.ieee.org/document/10189234) (in APR 2023)
- [Fixing Hardware Security Bugs with Large Language Models](https://arxiv.org/abs/2302.01215) (in Arxiv)
- [Fixing Rust Compilation Errors using LLMs](https://arxiv.org/abs/2308.05177) (in Arxiv)
- [Framing Program Repair as Code Completion](https://dl.acm.org/doi/10.1145/3524459.3527347) (in ICSE 2022)
- [Frustrated with Code Quality Issues? LLMs can Help!](https://arxiv.org/abs/2309.12938) (in Arxiv)
- [GPT-3-Powered Type Error Debugging: Investigating the Use of Large Language Models for Code Repair](https://dl.acm.org/doi/10.1145/3623476.3623522) (in SLE 2023)
- [How Effective Are Neural Networks for Fixing Security Vulnerabilities](https://dl.acm.org/doi/10.1145/3597926.3598135) (in ISSTA 2023)
- [Impact of Code Language Models on Automated Program Repair](https://dl.acm.org/doi/10.1109/ICSE48619.2023.00125) (in ICSE 2023)
- [Inferfix: End-to-end Program Repair with LLMs](https://dl.acm.org/doi/10.1145/3611643.3613892) (in FSE 2023)
- [Keep the Conversation Going: Fixing 162 out of 337 bugs for \$0.42 each using ChatGPT](https://arxiv.org/abs/2304.00385) (in Arxiv)
- [Neural Program Repair with Program Dependence Analysis and Effective Filter Mechanism](https://arxiv.org/abs/2305.09315) (in Arxiv)
- [Out of Context: How important is Local Context in Neural Program Repair?](https://arxiv.org/abs/2312.04986) (in ICSE 2024)
- [Pre-trained Model-based Automated Software Vulnerability Repair: How Far are We?](https://ieeexplore.ieee.org/abstract/document/10232867) (in IEEE Transactions on  Dependable and Secure Computing.)
- [RAPGen: An Approach for Fixing Code Inefficiencies in Zero-Shot](https://arxiv.org/abs/2306.17077) (in Arxiv)
- [RAP-Gen: Retrieval-Augmented Patch Generation with CodeT5 for Automatic Program Repair](https://dl.acm.org/doi/10.1145/3611643.3616256) (in FSE 2023)
- [STEAM: Simulating the InTeractive BEhavior of ProgrAMmers for Automatic Bug Fixing](https://arxiv.org/abs/2308.14460) (in Arxiv)
- [Towards Generating Functionally Correct Code Edits from Natural Language Issue Descriptions](https://arxiv.org/abs/2304.03816) (in Arxiv)
- [VulRepair: a T5-based Automated Software Vulnerability Repair](https://dl.acm.org/doi/10.1145/3540250.3549098) (in FSE 2022)
- [What Makes Good In-Context Demonstrations for Code Intelligence Tasks with LLMs?](https://ieeexplore.ieee.org/document/10298329/) (in ASE 2023)
