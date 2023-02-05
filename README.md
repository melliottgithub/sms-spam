# Jupyter Notebook Summary

## Overview

This Jupyter notebook contains a script for performing an analysis of SMS text messages to determine if they are spam or not using a naive bayes prediction model

## Implementation Details

The model is developed using Python's popular NLP library, `nltk` and is trained on a labeled dataset of sample "spam" and "ham" messages. The model uses the Naive Bayes classifier to make predictions based on the input text. 

## How to use

To use the model, make a POST request to the endpoint `https://b7slwkrm25wuxx2lbgr6cuzise0zypvd.lambda-url.us-west-2.on.aws/` with the following JSON data: 

## Json Example
# 
    {"model": "sms-spam",
    "text": "WINNER!! As a valued network customer you have been selected to receive a reward!"}


## Curl Example
# 
    curl -X POST 'https://b7slwkrm25wuxx2lbgr6cuzise0zypvd.lambda-url.us-west-2.on.aws/' -H 'Content-Type: application/json' -H 'Accept: application/json' -d '{"model":"week3_solution","text":"WINNER!! As a valued network customer you have been selected to receive a reward!"}'

