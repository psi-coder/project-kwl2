# Remake: KWL Project
Got bored today and decided to make some Evil Plans for Remaking the KWL Project from the ground up.

## Wishlist: Data Harvesting
- Create separate Spring Boot modules for each type of harvesting
- Use Spring Boot + Whatever Framework for scraping sites (check out Nutch)
- Scraper should harvest and store data without processing its contents

## Wishlist: Data Processing
- Use Spring Cloud Dataflow instead of Pentaho
- Use a Spark Cluster for Stream Processing
- Use a Hadoop Cluster for large batch jobs
- Use a Messaging Bus for Asyn Workflow
- Possibility of using TensorFlow for analyzing sites for data

## Wishlist: Platform
- Use Spring Boot as the main framework
- Use Spring Data for Mongo: less code means less bugs, more productivity
- Use Spring HATEOAS for exposing data: way less code than having to manually write every endpoint
- Separate Master Data and Metrics
- Use a Gateway Server
- Use OAuth2: huge security risk with writing up our own security framework
- Use Reactive endpoints for Server-to-Server communication

## Wishlist: Front End
- Use ReactJS + Flux instead of Angular as the app framework

# The Plan
- Figure out the following technologies
```
Spring Cloud DataFlow
Spring Security OAuth2
Kafka
Spark
Hadoop
Nutch
TensorFlow
```
- Start with the Master Data and Auth Server
- Harvest and Process iTunes Data
- Harvest Data from APIs
- Implement Scraper

# The Unknowns
- How to schedule batch jobs (check DataFlow)
- Smart way to scale up on scraping sites: we wont survive having to code a new script everytime we add a new site
