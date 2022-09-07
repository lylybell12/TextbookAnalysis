# Textbook Analysis (second semester progress)
Text mining and sentiment analysis of adjectives and verbs that surround masculine (he/him/his/himself), feminine (she/her/hers/herself) pronouns and top 50 proper nouns. The goal is to use this text-mining algorithm to assess the effects of sexism in educational content to uncover underlying influences in gender and STEM enrollment disproportionality. 

## How to start the analysis
1. Download and open folder on RStudio
2. Run all code on an R notebook

## Project Overview
- Produced a text mining algorithm to compare the significance of words surrounding pronouns via analysis on R using the `tidytext` package. 
- Sentiment value was extracted from the verbs and adjectives surrounding feminine/masculine pronouns and proper nouns using `AFINN` lexicon. 
- Sentiment severity was calculated using the frequency and the sentiment value of a word. 
- Run ANOVA testing on negative and positive words
- The word comparison between gender pronouns were then visualized for facilitated analysis using `ggplot2` package.
- No statistical influence of variables on sentiment severity of words. But there are skews in the usage of some words (in accordance with previous research on Fairy-tales). 
      More “masculine”
        -  Best
        -  Great
      More “feminine”
      -   Pretty
      -   Cried
- Skewed words are not statistically influential.  

![image](https://user-images.githubusercontent.com/92882742/188776576-aaf1b1b6-7603-41d3-99dd-1f866debb897.png)


## Assumptions
- Although gender is non-binary we only considered male and female pronouns for simplicity and ignored neutral pronouns such as ‘they/them.’
- Top 50 most common proper nouns were used
- Dataset contained 20 textbooks and 10 articles 


## Bigram Visualizations

### Initial Bigram (sample)
![alt_text](https://github.com/lylybell12/FairyTalesAnalysis/blob/main/visualizations/InitialBigram.PNG)

### Pronoun Separation Bigram (sample)
![alt_text](https://github.com/lylybell12/FairyTalesAnalysis/blob/main/visualizations/IntermediateBigram.PNG)

### Dimentionality Reduction Bigram (sample)
![alt_text](https://github.com/lylybell12/FairyTalesAnalysis/blob/main/visualizations/ReductionBigram.PNG)

## Bargraphs Comparing Sentiment Severity

### Sentiment Seversity for Masculine-associated words
![alt_text](https://github.com/lylybell12/FairyTalesAnalysis/blob/main/visualizations/SSM.png)

### Sentiment Seversity for Feminine-associated words
![alt_text](https://github.com/lylybell12/FairyTalesAnalysis/blob/main/visualizations/SSF.png)
