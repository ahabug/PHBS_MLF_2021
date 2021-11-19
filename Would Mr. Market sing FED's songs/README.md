# Would Mr. Market sing FED's songs?  -- Sentiment Analysis on the FOMC's documents

This is a group project of [PHBS_MLF_2021](https://github.com/PHBS/MLF).

## Team members 

Collaborators in this project are graduate students of quantitative finance and financial management from Peking University HSBC Business School:  

| Name                                          | Student ID |
| --------------------------------------------- | ---------- |
| [Wenchang Zhang](https://github.com/zwc00098) | 2001212425 |
| [Yu Lei](https://github.com/ahabug)           | 2001212276 |

## Project description

FOMC, part of the Federal Reserve Bank (FED) of the United States, the head of monetary policy in the US, is in charge of making and communicating policy decisions. When FED wants to perform QE (quantitative easing), it is FOMC that operates.  Intuitively, Mr. market follows the statements posted by FOMC closely. Once an FOMC meeting has been held, three critical documents are formed: statements, minutes, and transcripts. When the meeting concludes on the day, a statement is released, and this is when Mr. Market reacts and readjusts itself to any action / no action from FOMC. Three weeks later, minutes of the meeting are released, including some critical discussions during the meeting. Furthermore, after five years, the full transcript of the FOMC meeting will be released. 

FOMC wants to inform the public of their intentions and thoughts while withholding potentially volatile information for later release dates. Considering the period and text length, we wonder about the gap between the statements and minutes and how the market responds to the FOMC's documents, including statements, minutes, and federal reserve speeches. Would Mr. Market sing the FED's songs?

To explore, disentangle the sentiment contained in FOMC's documents, we initialized this project based on the dataset we obtained from the FOMC website and Yahoo Finance: 

| Project  |                           Details                            |
| :------: | :----------------------------------------------------------: |
| **Goal** | exploring how market responses to the FED's newly published documents |
| **Data** | [FOMC statements and minutes](https://www.federalreserve.gov/monetarypolicy/fomccalendars.htm); [Speeches of Federal Reserve Officials](https://www.federalreserve.gov/newsevents/speeches.htm); [Yahoo Finance](https://finance.yahoo.com/) |

## Task

1. Measuring the distance of minutes and statements [Measuring the Distance.ipynb](https://github.com/ahabug/PHBS_MLF_2021/blob/master/Would%20Mr.%20Market%20sing%20FED's%20songs/Measuring%20the%20Distance.ipynb)
2. Fit ML models with the market reaction as y variable (**we consider speeches full text as x variable due to sample size, similarly hereinafter**) [Fitting the model.ipynb](https://github.com/ahabug/PHBS_MLF_2021/blob/master/Would%20Mr.%20Market%20sing%20FED's%20songs/Fitting%20the%20model.ipynb)
3. Identify the most important vector (and corresponding word/phrase) with feature selection/extraction  [Identifying the most important vector.ipynb](https://github.com/ahabug/PHBS_MLF_2021/blob/master/Would%20Mr.%20Market%20sing%20FED's%20songs/Fit%20the%20model.ipynb)

## Result (some graphs)

<img src=".\graph\minutes.png" alt="minutes"  />

<img src=".\graph\statements.png" alt="minutes"  />

<img src=".\graph\minutes_words.png" alt="minutes_words"  />

<img src=".\graph\statements_words.png" alt="statements_words"  />
<img src=".\graph\distance.png" alt="distance"  />
<img src=".\graph\topic_vis.png" alt="topic_vis"  />

<img src=".\graph\speeches.png" alt="speeches"  />

<img src=".\graph\VIX.png" alt="VIX"  />

## Conclusion

1. We notice that the distance between the minutes and statements goes in waves and drops down step by step. Comparing the distance between minutes and statements and the Federal Fund Rate, we surprisingly find consistent movement. Also, it seems that the distance changes first. We infer that when there exists conflict among FOMC, the distance of minutes and statements increases, signaling that it is time to raise the Federal Funds rate.
1. It seems that the market had penetrated the FED's mind. We cannot predict precisely the market reaction based on the newly published FED document. The result is much worse than what we expected, which is similar to random guessing. Intuitively, the monetary policy is endogenous for the market, so the chances are that the market has a fair expectation for the FED's actions.
2. However, it doesn't mean that the market is inefficient. We can predict the market with high accuracy according to the minutes of the FOMC meeting. Unfortunately, the minutes are not public until three weeks after the meeting. (Hence, we ignore this part in our repo.) We should always respect Mr. Market! :vulcan_salute:

## Reference 

1. Jung, A. (2016). Have minutes helped to predict fed funds rate changes?. *Journal of Macroeconomics*, *49*, 18-32.x
2. Kusner, M., Sun, Y., Kolkin, N., & Weinberger, K. (2015, June). From word embeddings to document distances. In *International conference on machine learning* (pp. 957-966). PMLR.
3. Zhang, Y., & Wallace, B. (2015). A sensitivity analysis of (and practitioners' guide to) convolutional neural networks for sentence classification. arXiv preprint arXiv:1510.03820.
4. Röder, M., Both, A., & Hinneburg, A. (2015, February). Exploring the space of topic coherence measures. In Proceedings of the eighth ACM international conference on Web search and data mining (pp. 399-408).
5. Sievert, C., & Shirley, K. (2014, June). LDAvis: A method for visualizing and interpreting topics. In Proceedings of the workshop on interactive language learning, visualization, and interfaces (pp. 63-70).
