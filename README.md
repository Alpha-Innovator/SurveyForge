[![arXiv](https://img.shields.io/badge/arXiv-2303.06880-b31b1b.svg)](https://arxiv.org/abs/2303.06880)
[![GitHub issues](https://img.shields.io/github/issues/Alpha-Innovator/SmartSurvey)](https://github.com/Alpha-Innovator/SmartSurvey/issues)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://github.com/Alpha-Innovator/SmartSurvey/pulls)


# SurveyForge: On the Outline Heuristics, Memory-Driven Generation, and Multi-dimensional Evaluation for Automated Survey Writing

## Abstract

Survey paper plays a crucial role in scientific research, especially given the rapid growth of research publications. Recently, researchers have begun using LLMs to automate survey generation for better efficiency. However, the quality gap between LLM-generated surveys and those written by human remains significant, particularly in terms of outline quality and citation accuracy. To close these gaps, we introduce **SurveyForge**, which first generates the outline by analyzing the logical structure of human-written outlines and referring to the retrieved domain-related articles. Subsequently, leveraging high-quality papers retrieved from memory by our scholar navigation agent, **SurveyForge** can automatically generate and refine the content of the generated article.

Moreover, to achieve a comprehensive evaluation, we construct SurveyBench, which includes 100 human-written survey papers for win-rate comparison and assesses AI-generated survey papers across three dimensions: reference, outline, and content quality.
Experiments demonstrate that **SurveyForge** can outperform previous works such as AutoSurvey. We present several examples of auto-generated survey papers produced by **SurveyForge** at [Survey Demo](https://anonymous.4open.science/r/survey_example-7C37).

&ensp;
<p align="center">
  <img src="./assets/framework_surveyforge" width="85%">
  <div>The overview of SURVEYFORGE. The framework consists of two main stages: Outline Generation and Content Writing. In the Outline Generation stage, SURVEYFORGE utilizes heuristic learning to generate well-structured outlines by leveraging topic-relevant literature and structural patterns from existing surveys. In the Content Writing stage, a memory-driven Scholar Navigation Agent (SANA) retrieves high-quality literature for each subsection and LLM generates the content of each subsection. Finally, the content is synthesized and refined into a coherent and comprehensive survey.
</div>
</p>


## Web Demo
Due to the limitation on API call frequency, if you want to use our SurveyForge to generate papers, please email us or open an issue in the repository.

## SurveyBench
SurveyBench consists of approximately 100 human-written survey papers across 10 distinct topics, carefully curated by doctoral-level researchers to ensure thematic consistency and academic rigor.
.
