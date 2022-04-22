+++
author = "Ramona E.J. Spence"
title = "Tech Events API"
date = "2022-02-14"
description = "Open Source project organized by Code for Greenville"
tags = [
    "api", "project",
]
+++


Finding tech-related meetups that are in your area can be a bit of a pain when they're often split among platforms. Code for Greenville aims to solve that problem for the Upstate of South Carolina by bringing these events to one place and automatically updating it with our [Events API](https://github.com/codeforgreenville/upstate_tech_cal_service).<!--more--> 

The API is built in Flask, a Python framework and is used by a couple of different organizations. [Hack Greenville](https://hackgreenville.com/), Greenville's community of "hackers", techies, builders and tinkerers uses this events API to fill its calendar with relevant events. 

Taking advantage of Code for Greenville's [organizations API](https://github.com/codeforgreenville/OpenData/blob/master/ORGANIZATIONS_API.md), the Events API creates a list of tech organizations, such as [Women Who Code Greenville](https://www.womenwhocode.com/greenville) and [freeCodeCamp](https://www.fcc-greenville.com/), that are hosting events on Meetup and Eventbrite. 

With the data from the organizations API, we can query Meetup and Eventbrite's APIs to build a list of online and in-person events that holds all of the details of each, including when they are, where they are (if in-person), what organization is putting on the event, and much more.

The events API makes this data available in a colloquial (only it understands which fields represent what) JSON format by default. However, if it's specified in the request, the data is also available in JSON+LD format. 

# Notes:

Tech Events API:
* What is the Tech Events API 
    * Open-source, 
    * a Flask application that serves data to an API endpoint
    * contains a script to update a local list of Events, this script gets called on by a PHP cronjob every so often
* What does the API do 
    * Uses Org API to retrieve organizations IDs
    * Uses IDs to request events from Meetup.com and Eventbrite
    * Formats the respective response data to match API's colloquial JSON format
* What does the API do, not technically or literally, but what does it do for people, the community, etc?
    * 
* Who/what projects consume this API 
* How has it progressed  

