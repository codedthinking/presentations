---
title: "Interviewing Your Data: Getting Data"
author: 
 - Miklós Koren
aspectratio: 54
---

# Tidy data
## Data vs story
Contrary to the aphorism, data is *not* the plural of anecdote.
- known structure
- known collection method

## Benefits of (more) data
- Less subject to selection/recall bias.
- Statistical learning can be applied.

## Drawbacks of (more) data
- Harder to work with.
- Harder to interpret/relate to.
- May give false sense of knowledge.

## Tidy data
1. Every row is an observation (case, record)
2. Every column is a variable (feature, attribute)
3. Every cell contains a single value

## Spreadsheet as a canvas
![](assets/messy-data.png)

## Same content in tidy form
![](assets/tidy.png)

## Benefits
- Machine readable
- Can select columns (=variables)
- Can filter rows (=observations)
- Can sort rows
- Can join rows

# Spreadsheets
## Learn to love your spreadsheet editor
- Beware of Excel! Good alternatives: Libre Office, Open Office, Google Sheets.

## Useful steps
- filter
- sort
- vlookup


# Where to find data?
# How to get it?
# HTTP and HTML

## What's in a URL?
![How URLs work by Julia Evans](https://wizardzines.com/comics/how-urls-work/how-urls-work.png)

## What's HTTP?
![by Julia Evans](https://wizardzines.com/comics/whats-http/whats-http.png)

# API, CSV, XML and JSON

# Scraping
## 
scraping = crawling + parsing

## Four steps of a scraping project
1. Recon
2. Crawl
3. Parse
4. Store

## Recon
1. Locate the interesting documents and tables
2. Note the structure of URLs and tables
3. Explore `robots.txt` and terms of use
4. Explore robot protection

# Exercise
