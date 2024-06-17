# Coarse-to-Fine Personalized LLM Impressions for Streamlined Radiology Reports

## Table of Contents

- [Introduction](#introduction)
- [Research Problem](#research-problem)
- [Goals of Analysis](#goals-of-analysis)
- [Methodology](#methodology)
- [Data](#data)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Introduction

In radiology, creating the "Impression" section of reports is critical for clinical decision-making but is also a significant contributor to radiologist burnout due to its time-intensive nature. This project introduces a novel approach leveraging open-sourced pre-trained Large Language Models (LLMs) to automate and personalize the crafting of radiological impressions. Utilizing a coarse-to-fine methodology, this strategy begins by generating a preliminary impression based on imaging findings and patient data, which is then refined to align with the individual radiologist's stylistic preferences through advanced machine learning techniques.

## Research Problem

The "Findings" section of a radiology report presents observations made during the examination of imaging studies. The "Impression" section offers a synthesized interpretation of these findings, aiding in clinical decision-making and patient management. Recognizing the substantial time investment radiologists allocate to crafting impressions, this project leverages open-sourced pre-trained LLMs to expedite the generation of personalized impressions, ensuring factual correctness and stylistic alignment.

## Goals of Analysis

The project proposes fine-tuning a selection of open-sourced pre-trained LLMs using radiology reports sourced from the University of Chicago Medicine. The objective is to generate high-quality impressions that are both factually accurate and tailored to individual preferences. The study explores LLMs such as LLaMA 3B, LLaMA 7B, and Mistral 7B, employing reinforcement learning from human feedback (RLHF) to achieve personalization and factual accuracy.

## Methodology

This project leverages a fine-tuning approach to adapt pre-trained LLMs for generating personalized radiology report impressions. Key methodologies include:

- **Model Selection:** Exploring LLM architectures including LLaMA (3B, 7B) and Mistral (7B) for a balance between computational efficiency and output quality.
- **Personalization:** Using Reinforcement Learning from Human Feedback (RLHF) to tailor impressions to individual radiologists' stylistic preferences.
- **Data Integration:** Combining clinical data with imaging findings to enhance context and factual accuracy.
- **Encoder-Decoder Framework:** Utilizing transformers and graph neural networks to encode complex interdependencies among medical entities.
- **Evaluation:** Beyond conventional NLP metrics, assessments include clinical utility and physician reviews to ensure practical applicability.

## Data

The dataset comprises 789,278 anonymized radiology reports from UChicago Medicine, including clinical patient information, unstructured textual findings, and structured impression sections. The dataset spans eight modalities, with CT scans constituting approximately 90%. The dataset's quality and scope provide a significant advantage over prior studies.

## Features

- **Automated Impression Generation:** Streamlines the radiology reporting process.
- **Personalization:** Aligns generated impressions with individual radiologists' writing styles.
- **Factual Accuracy:** Ensures generated impressions are accurate and reliable.

## Installation

To install and run this project locally, follow these steps:

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/repository-name.git
    ```
2. Navigate to the project directory:
    ```bash
    cd repository-name
    ```
3. Install the dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

To use the project, run the following command:

```bash
python main.py
