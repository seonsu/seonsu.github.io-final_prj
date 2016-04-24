---
title       : Coursera Data Science Capstone - Final Project
subtitle    : April 23, 2016
author      : Seon Su Kim
job         : This project predicts the next word as the user types in a word or phrase.
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Introduction

- This presentation file was produced as a part of the requirement for Data Science Capstone Course.

- The data used in this project is a large corpus of text documents from swiftkey (https://swiftkey.com/en).

- The goal of the project is to build a predictive text model combined with a shiny app UI that will predict the next word as the user types a sentence similar to the way most smart phone keyboards are implemented today using the technology of Swiftkey.

- This presentation explains the prediction model and the shiny app that was developed.

---  

## Getting & Cleaning the Data

- The Swiftkey Corpus from the link was used in this project.

- https://d396qusza40orc.cloudfront.net/dsscapstone/dataset/Coursera-SwiftKey.zip

- The data was downloaded and read into R. The sample data was then cleaned as a preparation for the analysis which includes converting to lowercase, removing punctuations, links, numbers, white spaces and special characters.

- A shiny app is then developed to predict the next word that comes after a word or phrase being typed in.

---

## The Prediction Algorithm

- The sample is cleaned to remove numbers, punctuations,links, white spaces, bad words and special characters.

- The Text Mining package library in R is used to build the base for the prediction of this project.

- A unigram, bigram and trigram were built from the data and the data is used to predict the next word based on the word or phrase typed by the user.

---

## The Application

- A Shiny application was developed based on the next word prediction model described previously as shown below. 

- You fist, type a phrase in the box below. And then, you will see the predicted next word of your phrase.

- The link to the app is http://ssk992.shinyapps.io/shiny/

