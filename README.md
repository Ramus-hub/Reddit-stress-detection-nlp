# Reddit Stress Detection Using NLP

This repository explores how stress is expressed in Reddit posts and whether stressed content can be identified using data mining and natural language processing techniques. The project analyzes text-based signals such as emotional language, sentiment indicators, and user engagement patterns to understand how stress appears in online discussions.

The motivation behind this work is that people often express stress online before seeking help offline. By studying these signals at scale, the project aims to uncover recurring patterns while remaining explicit about the limitations and ethical risks of automated emotional inference.

## Project Scope

The project focuses exclusively on Reddit data and does not attempt to make clinical or diagnostic claims. Stress detection is treated as a probabilistic classification task based on language patterns, not as an assessment of mental health conditions.

Key goals include:
- Exploring linguistic and emotional markers associated with stress
- Applying classification and clustering techniques to text data
- Identifying common themes in stress-related posts
- Evaluating model confidence and uncertainty

## Data Sources

- **Dreaddit Dataset (Hugging Face)**  
  A labeled dataset of Reddit posts annotated for stress-related content, containing text and lexical emotion features.

- **Reddit API (PRAW)**  
  Additional posts and comments collected directly from Reddit using the official API, including subreddit context and engagement metrics such as score.

All data used in this project is publicly available and text-only.

## Stakeholders and Impact

This project affects multiple groups:
- Reddit users whose posts are analyzed, often written without the expectation of automated interpretation
- Moderators and platform operators who may use similar tools to triage content
- Researchers and data scientists studying large-scale online behavior
- Indirect readers who encounter Reddit content through search engines
- Users of AI-powered search and assistant systems that reuse Reddit data in summarized form

Because Reddit content often reaches far beyond the platform itself, errors or bias introduced during analysis can propagate through downstream systems. For this reason, transparency and scope limitation are core design principles of this work.

## Limitations and Bias

- Reddit users are not representative of the general population
- Language patterns are platform-specific and culturally dependent
- Text-only analysis cannot capture tone, sarcasm, or non-verbal cues reliably
- Models may confuse venting or humor with genuine stress
- Results are time-dependent and may reflect short-term events

Predictions with low confidence are treated as uncertain rather than forced into binary labels.

## Ethical Considerations

This project does not attempt to diagnose individuals or provide mental health advice. Outputs should be interpreted as exploratory signals, not ground truth. Any real-world deployment would require safeguards, disclaimers, and human oversight.
