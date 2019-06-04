# Wrangling Messy Tweets
## By Jeremy Sung
## Objective
This project explores the tweets of a Twitter account "WeRateDogs" ([@dog_rates](https://twitter.com/dog_rates)), a.k.a. [WeRateDogs](https://en.wikipedia.org/wiki/WeRateDogs). This Twitter rates dogs with humorous comments about the dog. It has over 7 million followers since its debut and has received international media coverage.

I exercised data wrangling rules and cleaning techniques in Python on messy data. The data can, then, serve in-depth visualizations and trustworthy analyses.

## Dataset Overview
The WeRateDogs Twitter archival dataset in this project is a filtered (enhanced) version of tweets which contain ratings, dog name, and dog "stage", such as doggo, floofer, pupper and puppo, etc. This leaves about 2,356 out of 5,000+ tweets in the process. It serves as the base of the analyses. This dataset is supplemented by an Image Predictions file (loaded as a Pandas DataFrame) and additional online data retrieved via TWEET API from twitter.
- Enhanced Twitter Archive
- Additional Data retrieved via the Twitter API
- Image Predictions File

This messy data requires quite a few cleaning before it can be used in any meaningful analyses. I applied Tidy data rules along with some industry best practices to prepare the data ready for next step.

## Some of the challenges with these data include:
- Ratings, dog name and dog stages may not be correct. That is, I need to assess and clean at least 8 quality issues and at least 2 tidiness issues in this dataset.
- `Retweet count` and `favorite count` are two of the notable column omissions. This additional data can be gathered by anyone from Twitter's API. I'm going to leverage the tweet IDs within the WeRateDogs Twitter archive to query Twitter's API and gather this valuable data, etc. More details are elaborated in the [Quality Issues](#quality_issues) and [Tidying Data](#tidying_data) sections.
