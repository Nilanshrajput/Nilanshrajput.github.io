---
title: "Fine-tuning Bert for Patent Category Classification"
date: 2020-02-10
tags: [NLP, data scraping, BERT, Transformer, Deep Learning]
header:
  image: "/images/perceptron/percept.jpg"
excerpt: "NLP, data scraping, BERT, Transformer, Deep Learning"
mathjax: "true"
---

#  <span class="underline">Fine-tuning Bert for Patent Category Classification</span>

This project was for my entry in Advitiya IIT Ropar Hackathon, and it resulted in 1st Place Finish.

Problem Statement : To categorise a given Patent number with one category out of 4 (\`Alcoholic\`, \`Non-Alcoholic\`, \`Automotive\`, \`Non-Automotive\`).

Largely Extended a Google Patent Scraper Library for my use-case, for scrapping relevant details about a Patent from a given Patent number. Scrapped all of the data using this custom library. Scrapped from the google patent page data is saved in JSON format.

After this initial part of collecting data,the text data is pushed in the pipeline for cleaning, tokenizing and pre-processing to pass it into BERT using Hugging Face for fine tuning the model on patent data. Trained more than 15 models experimenting with hyperparameters, and finally submitted an result from an ensemble of 6 models.

**Model Details : 12-layer BERT model, with an uncased vocab.**
