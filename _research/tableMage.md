# ChatDA

## Background
The effective advancement of evidence-based medicine relies on the seamless integration of clinical domain expertise with rigorous data analysis. However, a significant barrier exists because many clinicians lack formal training in statistics and data science, which often leads to a reliance on external analysts and slows the translation of data into actionable medical interventions. While large language models (LLMs) offer a potential solution by acting as conversational data assistants, their deployment in healthcare is hindered by severe privacy risks. Standard AI agents that generate code typically require direct access to raw patient data, which can lead to the exposure of sensitive information or the risk of re-identification even when data is de-identified. There is a need for tools that empower clinicians to perform advanced analytics while maintaining the standards of data protection.

## Overview of ChatDA
**Chat Data Analyst (ChatDA)** is an AI agent specifically designed for the conversational analysis of de-identified clinical tabular data. To address the privacy limitations of standard models, ChatDA introduces a "tools-only" analysis mode. In this mode, the underlying LLM is restricted from accessing raw, individual-level patient records. Instead, all computations are performed locally through a specialized toolkit built on **TableMage**, a low-code Python package for clinical data science. The tools return only aggregated, population-level insights—such as summary statistics, regression coefficients, and performance metrics—to the LLM. This architecture ensures that individual-level data remains within the local environment while still allowing clinicians to perform complex tasks like data transformation, statistical testing, and machine learning modeling through natural language.

## Paper
**Tool-wielding language model-based agent offers conversational exploration of clinical tabular data**

## Selected Important Results
ChatDA was benchmarked against leading AI agents, including OpenAI's Advanced Data Analysis (ADA), showing superior performance in data analysis workflows. On the DataAnalysisQA benchmark (introduced in this paper), ChatDA outperformed all other evaluated agents. The agent also demonstrated narrower confidence intervals across evaluation runs, addressing the common problem of output variability in LLMs. ChatDA also achieved a strong performance in retaining engineered features between analysis steps, nearly doubling the performance of several code-writing agents. In an analysis of 1,419 knee arthroplasty patients, ChatDA successfully identified the joint line convergence angle as a significant predictor for surgical procedure selection (total knee arthroplasty vs. unicompoartmental knee arthroplasty) with a single uninterrupted session.

<p style="text-align: justify">
</p>
<div style="text-align: center;">
  <img src="/images/ChatDA-Figure1-R1.jpg" alt="drawing" width="500"/>
</div>

## Method Tutorial and Code Availability
TableMage is available on [GitHub](https://github.com/YMa-lab/TableMage). A tutorial is available on [readthedocs](https://tablemage.readthedocs.io/en/latest/demo.html#).