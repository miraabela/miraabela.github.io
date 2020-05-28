---
layout: essay
type: essay
title: InternBit Related Work
date: 2019-05-27
published: true
labels:
summary: InternBit Related Work
---

## Building an Internship Recommendation System

In the first article, Building an Internship Recommendation System, there are four parts to Nangia’s process: collecting data, cleaning data, analyzing data, and making recommendations. 
In the Introduction he brings up three different models for recommendation systems: knowledge based, collaborative filtering, and content based. Knowledge based uses information from the user such as their  preferences to suggest items. Collaborative filtering recommends items that similar users to the current user have read. Content based filtering uses information known about the item itself to recommend similar items. He outlines two methods to evaluate his recommendation system: the first is an A/B test, and the second relies on clicks.

He uses the BeautifulSoup python library in the scraping section to collect links and collect data from the pages. He uses the Pandas python library for data cleaning and NLP processing of the data. He uses NLP techniques to create a similarity matrix to create the recommendations. 

### Relation to InternBit

I envision InternBit as having content based recommendations, such as recommend new internships based on what the student favorites. I see NLP being used to determine tags and keywords for each internship listing, then having a system of weighted keywords that are tallied onto when a student favorites the internship. 
My method would be similar to a bag of words and having weighted keywords. For example, each student has a list of tags they are associated with, such as skill names, computer science fields like “machine learning”, and each of them have points associated with them based on the student’s profile (previous classes, opportunities, interests, career goals). 
For scraping, Internet needs to use a javascript scraping library instead of BeautifulSoup. Since many websites will be scraped instead of just one, there needs to be a way to normalize or standardize the scraped data so that all the data from each website can be compared in a standard way. The columns need to be defined and the same for all websites.
For cleaning, we need to find an NLP library for javascript to clean the data for InternBit. We would need to define the phrases and repetitive keyword that need to be removed. There might be some amount of overlap when scraping multiple websites, so checking for duplicate listings is necessary after formatting the data in a standard way. 

## AI-Based Recommendation System

In order for InternBit to be independent of Radgrad, a student just needs to fill out their profile / questionnaire to get a view of what their skills, interests, and career goals are. This article doesn’t go into the technical details of how they did it, so I clicked the references to read the full paper. In the paper, they define competence as having soft and hard skills. The hard skills are the learned skills from school. The soft skills include communication, social interaction, respecting other opinions, and proposing new ideas. RadGrad doesn’t really have a way to measure soft skills, but we can measure the hard skills based on the classes. A lot of job postings have soft skills required such as communication, so I am wondering how a student can specify they communicate well in InternBit. Another example is how can a student express they are creative, if a job posting requires creativity. That wouldn’t come from the list of skills if we only parse the courses a student took. Maybe these tags can be added to opportunities they did in the past, such as graphic design. So then we would need to additionally think about these soft skills as we add tags to the Opportunities that will be parsed from a student’s profile. 