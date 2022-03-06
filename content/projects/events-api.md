+++
author = "Ramona E.J. Spence"
title = "Tech Events API"
date = "2022-02-14"
description = "Open Source project organized by Code for Greenville"
tags = [
    "api", "project",
]
+++


This Code for Greenville project collects and formats information on tech tech related meetup and eventbrite events serving the data in a standardized format.  <!--more-->
The application first aggregates a list of organizations that host their events on Meetup and Eventbrite from Code for Greenville's [Organizations API](https://github.com/codeforgreenville/OpenData/blob/master/ORGANIZATIONS_API.md) and uses the data found there to query Meetup and Eventbrite APIs for the organizations' event data. THat data gets formated in one standard way except when the API is specifically asked to return the data in JSON+LD content type, which gives the data context and gives search engines a way to understand the data. 


