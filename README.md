# SurveyForge: On the Outline Heuristics, Memory-Driven Generation, and Multi-dimensional Evaluation for Automated Survey Writing

<p align="center">
  <i>
  Code, demos, and benchmarks are all available now!
  </i>
  <br>
  <a href="https://arxiv.org/abs/xxxx.xxxxx">
      <img src="https://img.shields.io/badge/arXiv-Paper-red.svg?logo=arxiv" alt="arxiv paper">
  </a>
  <a href="https://huggingface.co/papers/xxxx.xxxxx">
    <img src="https://img.shields.io/badge/Huggingface-🤗-yellow?style=flat" alt="huggingface paper">
  </a>
  <!-- <a href="https://github.com/IAAR-Shanghai/SurveyX">
    <img src="https://img.shields.io/github/stars/IAAR-Shanghai/SurveyX?style=flat&logo=github&color=yellow" alt="github stars">
  </a> -->
    <!-- <img src="https://img.shields.io/github/last-commit/IAAR-Shanghai/SurveyX?display_timestamp=author&style=flat&color=green" alt="last commit"> -->
  </a>
  </a>
</p>

🤩Tired of chaotic structures and inaccurate references in AI-generated survey paper? **SurveyForge** is here to revolutionize your research experience!

## Introduction

<p align="center">
  <img src="./assets/framework_surveyforge.png" width="95%">
  <!-- <div>The overview of SURVEYFORGE. The framework consists of two main stages: Outline Generation and Content Writing. In the Outline Generation stage, SURVEYFORGE utilizes heuristic learning to generate well-structured outlines by leveraging topic-relevant literature and structural patterns from existing surveys. In the Content Writing stage, a memory-driven Scholar Navigation Agent (SANA) retrieves high-quality literature for each subsection and LLM generates the content of each subsection. Finally, the content is synthesized and refined into a coherent and comprehensive survey.
</div> -->
</p>

Survey papers are vital in scientific research, especially with the rapid increase in research publications. Recently, researchers have started using LLMs to automate survey creation for improved efficiency. However, LLM-generated surveys often fall short compared to human-written ones, particularly in outline quality and citation accuracy. To address this, we introduce **SurveyForge**, which first creates an outline by analyzing the structure of human-written outlines and consulting domain-related articles. Then, using high-quality papers retrieved by our scholar navigation agent, **SurveyForge** can automatically generate and refine the content of the survey.

Moreover, to achieve a comprehensive evaluation, we construct **SurveyBench**, which includes 100 human-written survey papers for win-rate comparison and assesses AI-generated survey papers across three dimensions: reference, outline, and content quality.

## 🤔How to try out SurveyForge?

* You can clone our source code and deploy it locally. Make sure you've got a GPU ready for loading the embedding model and an API set up for calling the LLM. Please refer to the [guidelines](code_doc.md) for more details
* If you're just curious about how the generated survey paper look, **please kindly send us an email or open an issue** in the repository to inform us of the **survey topic** you intend to generate. At this stage, this is the best way for us to showcase the capabilities of SurveyForge. Moving forward, we are actively working to enhance our API capacity and aim to make SurveyForge publicly accessible in the near future. Thank you for your understanding and support!

⏱️Surveyforge only takes about 10 minutes to generate a review paper. There may be a wait time as the number of users increases, so submit your topic early!

🌟Don’t forget to click the STAR to track if your survey is ready for launch!

## 🕵️‍♂️How do I know if the Survey is good or not?

We offer **SurveyBench**, a benchmark for **academic research** and **evaluating the quality of AI-generated surveys.**

[SurveyBench Download](https://huggingface.co/datasets/U4R/SurveyBench)

Currently , SurveyBench consists of approximately 100 human-written survey papers across 10 distinct topics, carefully curated by doctoral-level researchers to ensure thematic consistency and academic rigor. The supported topics and the core references corresponding to each topic are as follows:

| Topics                                                   | # Reference |
| -------------------------------------------------------- | :---------: |
| Multimodal Large Language Models                         |     912     |
| Evaluation of Large Language Models                      |     714     |
| 3D Object Detection in Autonomous Driving                |     441     |
| Vision Transformers                                      |     563     |
| Hallucination in Large Language Models                   |     500     |
| Generative Diffusion Models                              |     994     |
| 3D Gaussian Splatting                                    |     330     |
| LLM-based Multi-Agent                                    |     823     |
| Graph Neural Networks                                    |     670     |
| Retrieval-Augmented Generation for Large Language Models |     608     |

More support topics coming soon!

### 🧑‍💻You can evaluate the survey by:

```
cd SurveyBench && python test.py --is_human_eval
```

Note set `is_human_eval` True for human survey evaluation, False for generated surveys.

If you want to evaluate your method on SurveyBench, please follow the format:

```
generated_surveys
|-- 3D Gaussian Splatting
    |-- exp_1
        |-- ref.json
    |-- exp_2
        |-- ref.json
...
|-- Graph Neural Networks
...
```

## 📝Examples

| Topics                                                   | Links |
| -------------------------------------------------------- | :---: |
| Multimodal Large Language Models                         |      |
| Evaluation of Large Language Models                      |      |
| 3D Object Detection in Autonomous Driving                |      |
| Vision Transformers                                      |      |
| Hallucination in Large Language Models                   |      |
| Generative Diffusion Models                              |      |
| 3D Gaussian Splatting                                    |      |
| LLM-based Multi-Agent                                    |      |
| Graph Neural Networks                                    |      |
| Retrieval-Augmented Generation for Large Language Models |      |
