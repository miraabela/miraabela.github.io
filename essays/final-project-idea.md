---
layout: essay
type: essay
title: "Final Project Idea"
date: 2019-03-26
labels:
  - Software Engineering
  - Meteor
---

# Overview
The Problem:
There is a high dropout rate in lower level ICS coursesr potential students because of lack of motivation and unawareness of resources available. New students have a false stigma of what computer science emcompasses. 

The Solution:
Easily accessible searchable and filterable database of opportunities available for ICS students in Hawaii that is categorized by: internships, clubs, volunteer opportunities, hackathons, jobs, projects, professional organizations, networking events, skill building. More awareness of opportunities will lead to a lower dropout rate, clear focus of career goals, and improve motivation. The landing page will be designed to be more appealing to freshman.


# Approach
 Mongo Database:
- Collection of Opportunities
- - Opportunity Document:
- - - Id (string), Name (string), Description (string), interestIDs(string array), Type (string array)
- Collection of Users
- - Id (string), firstName (string), lastName (string), email (string), password (string), interestsIDs (string array), opportunityIDs (string array), careerIDs (string array)
- Collection of Interests
- - id (string), Name (string), description (string)
- Collection of Careers
- - id (string), Name (string), description (string), interestIDs (string array)
 
# Overview of Pages
- Landing Page marketed towards freshman
- Profile: Add interests, See Saved Opportunities
- Explore: Search and Filter Opportunities by Type/Interest

# Use Cases
- New Freshman just getting to know and explore the ICS community and resources in Hawaii

# Beyond the basic
- Explore page visualized with mind maps?
- Notifications for event opportunities, internship application deadlines
- See other users with same interests
- Commenting System
