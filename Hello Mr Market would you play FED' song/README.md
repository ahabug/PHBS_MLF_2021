# Hello Mr Market would you play FED's song? Sentiment Analysis on Central Bank Statement

This is a group project of [PHBS_MLF_2021](https://github.com/PHBS/MLF).

## Navigation

| Report | Code | Data & Model |
| :----- | ---- | ------------ |
|        |      |              |

[TOC]

## Team members 

Collaborators in this project are graduate students of quantitative finance and financial management from Peking University HSBC Business School:  

| Name                                          | Student ID |
| --------------------------------------------- | ---------- |
| [Wenchang Zhang](https://github.com/zwc00098) | 2001212425 |
| [Yu Lei](https://github.com/ahabug)           | 2001212276 |

## Project description

Social network sentiments and news sentiment have been widely used to drive market movements in real-time. Dozens of companies have established live statement analysis feed for trading purposes. However, we find a time lag during analyzing the Federal Open Market Committee (FOMC) minutes. 

FOMC, part of the Federal Reserve Bank (FED) of the United States, the head of monetary policy in the US, is in charge of making and communicating policy decisions. When FED wants to perform QE (quantitative easing), it is FOMC that operates.  It is not surprising that Mr. market follows the statements posted by FOMC closely. Once an FOMC meeting has been held, three critical documents are generated: statements, minutes, and transcripts. When the meeting concludes on the day, a statement is released, and this is when Mr. Market reacts and readjusts itself to any action / no action from FOMC. Three weeks later, minutes of the meeting are released, including some critical discussions during the meeting. Furthermore, after five years, the full transcript of the FOMC meeting will be released. 

FOMC wants to inform the public of their intentions and thoughts while withholding potentially volatile information for later release dates. Considering the period and text length, we wonder about the distance between the statements and minutes and whether the sentiment in FOMC minutes can have a longer-term impact on Mr. Market. The chances are that Mr. Market is only responding to FED live statements for a few days and loses his memory, and moves on to other key economic factors as non-farm payrolls, CPI, and PMI. 

In order to explore, disentangle the sentiment contained in FOMC statements and minutes, we initialized this project based on the dataset we obtained from the FOMC website and Yahoo Finance: 

|       Project        |                           Details                            |
| :------------------: | :----------------------------------------------------------: |
|       **Goal**       |      To find trading signals contained in FOMC minutes       |
|       **Data**       | [FOMC statements and minutes](); Stock index price and interest rates from [Yahoo Finance](https://finance.yahoo.com/) |


## Task, significance and process

## Data exploration

## Data cleaning

## Baseline and XXX models

## Conclusion

## Reference 

1. Jung, A. (2016). Have minutes helped to predict fed funds rate changes?. *Journal of Macroeconomics*, *49*, 18-32.
