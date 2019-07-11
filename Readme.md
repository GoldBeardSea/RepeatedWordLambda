# Java Lambda Repeated Word

## Description

This repo represents the source of a jar living in a lambda function. 

The lambda functions listens for a string query at https://kq0j7zmuu3.execute-api.us-east-2.amazonaws.com/prod?queryString= 

Anything after the = will be submitted as a string to maxWord. 

The maxWord function  is case sensitive but accounts for standard punctuation. If no queryString is specified in the url it will return null. 

### Problems

An interesting problem I encountered was having to drop down my runtime environment because I was using a later build of java. 
I had to insert sourceCompatibility = 1.8 and targetCompatibility=1.8.