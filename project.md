---
title: "Reproducible Research Course Project 2"
author: "Mark Chang"
date: "2026-10-19"
output:
  html_document:
    keep_md: true
---

## Introduction / Synopsis

This project involves exploring the U.S. National Oceanic and Atmospheric Administration's (NOAA) storm database. We will answer several questions related to a subset of the data in this database. 

## Data

The data for this project comes from NOAA; it is [downloadable](https://d396qusza40orc.cloudfront.net/repdata%2Fdata%2FStormData.csv.bz2) as a bzip2 compressed file.

Information on how the variables are constructed can be found from the following links :-

- National Weather Service [Storm Data Documentation](https://d396qusza40orc.cloudfront.net/repdata%2Fpeer2_doc%2Fpd01016005curr.pdf)
- [National Climatic Data Center Storm Events](https://d396qusza40orc.cloudfront.net/repdata%2Fpeer2_doc%2FNCDC%20Storm%20Events-FAQ%20Page.pdf)

The events in the database start in the year 1950 and end in November 2011. Less data is available in the earlier years of the database.

## Assignment

Set to show R code


``` r
library(data.table)
library(ggplot2)
library(knitr)
opts_chunk$set(echo=TRUE)
```

### Loading and preprocessing the data


``` r
# Windows
#setwd("C:/Users/mchang/Projects/ProgrammingAssignment7")

# Mac
setwd("/Users/mchang/Projects/ProgrammingAssignment7")

path <- getwd()
datasetpath <- file.path(path,"dataset")
datafilename <- "dataFiles.zip"

# Download file
url <- "https://d396qusza40orc.cloudfront.net/repdata%2Fdata%2FStormData.csv.bz2"
#download.file(url, file.path(path, datafilename))
#unzip(zipfile = datafilename, exdir = datasetpath)
```



