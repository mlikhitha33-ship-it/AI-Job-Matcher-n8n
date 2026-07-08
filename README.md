# AI Job Matcher

AI Job Matcher is a workflow automation project built with n8n that helps job seekers(students) find relevant opportunities using AI.
Instead of manually searching through hundreds of job postings, this workflow automatically searches for jobs, evaluates how well they match a candidate's skills, filters the best opportunities, and delivers the results in a structured format.

## What It Does

* Reads candidate skills and job preferences from Google Sheets
* Fetches job listings using the JSearch API
* Uses Groq LLMs to evaluate job-candidate fit
* Assigns a match score to each job
* Filters high-quality matches
* Saves results to Google Sheets
* Sends an email summary of recommended jobs

## Workflow

```
Daily Trigger
    ⬇️
Load Candidate Profile
    ⬇️
Fetch Job Listings
    ⬇️
Process Job Data
    ⬇️
AI-Based Job Matching (Groq)
    ⬇️
Filter Best Matches
    ⬇️
Save Results to Google Sheets
    ⬇️
Send Email Summary
```

## Tech Stack

* n8n
* Groq (Llama Models)
* Google Sheets
* Gmail
* JSearch API (RapidAPI)
* JavaScript

## Getting Started

1. Import the workflow into your n8n instance
2. Configure your Google Sheets credentials
3. Configure your Gmail credentials
4. Add your Groq API key
5. Add your RapidAPI JSearch credentials
6. Run the workflow

## Required Credentials

* Groq API Key
* Google Sheets OAuth2
* Gmail OAuth2
* RapidAPI JSearch API Key

## Why I Built This

Job searching can be repetitive and time-consuming. I wanted to explore how AI and workflow automation could be combined to automatically identify opportunities that align with a candidate's skills and career goals.

This project demonstrates workflow automation, API integrations, AI-powered decision making, and practical use of Large Language Models in a real-world scenario.

## Future Enhancements

* Resume parsing
* Dynamic location-based searches
* LinkedIn integration
* Support for multiple LLM providers
* ATS compatibility analysis
* Job matching dashboard

## License

This project is open-source and available for learning and experimentation.

