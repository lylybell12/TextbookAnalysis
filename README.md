# Textbook Analysis (second semester progress)
Text mining and sentiment analysis of adjectives and verbs that surround masculine (he/him/his/himself), feminine (she/her/hers/herself) pronouns and top 50 proper nouns. The goal is to use this text-mining algorithm to assess the effects of sexism in academic content to uncover underlying influences in gender and STEM enrollment disproportionality. 

## How to start the analysis
1. Download and open folder on RStudio
2. Run all code on an R notebook

## Project Overview
- Produced a text mining algorithm to compare the significance of words surrounding pronouns via analysis on R using the `tidytext` package
- Sentiment value was extracted from the verbs and adjectives surrounding feminine/masculine pronouns and proper nouns using `AFINN` lexicon
- Sentiment severity was calculated using the frequency and the sentiment value of a word
- Run ANOVA testing on negative and positive words
- The word comparison between gender pronouns were then visualized for facilitated analysis using `ggplot2` package
- No statistical influence of variables on sentiment severity of words. But there are skews in the usage of some words (in accordance with previous research on Fairy-tales)
- Skewed words are not statistically influential

## Assumptions
- Although gender is non-binary we only considered male and female pronouns for simplicity and ignored neutral pronouns such as ‘they/them.’
- Top 50 most common proper nouns were used
- Dataset contained 20 textbooks and 10 articles 

## Bigram Visualizations

### Pronoun Separation Bigram (sample)
![alt_text](https://github.com/lylybell12/FairyTalesAnalysis/blob/main/visualizations/IntermediateBigram.PNG)

### Dimentionality Reduction Bigram (sample)
![alt_text](https://github.com/lylybell12/FairyTalesAnalysis/blob/main/visualizations/ReductionBigram.PNG)

## Bargraphs Comparing Sentiment Severity

### Sentiment Seversity for Masculine-Associated words
![alt_text](https://github.com/lylybell12/TextbookAnalysis/blob/main/TextbookAnalysisVisuals/SentimentSeverityMales.png)

### Sentiment Seversity for Feminine-Associated words
![alt_text](https://github.com/lylybell12/TextbookAnalysis/blob/main/TextbookAnalysisVisuals/SentimentSeverityFemales.png)

## ANOVA Testing

### Tesing for Negative Words
![alt_text](https://github.com/lylybell12/TextbookAnalysis/blob/main/TextbookAnalysisVisuals/ANOVANEG.png)

### Tesing for Positive Words
![alt_text](https://github.com/lylybell12/TextbookAnalysis/blob/main/TextbookAnalysisVisuals/ANOVAPOS.png)

