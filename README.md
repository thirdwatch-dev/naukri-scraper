# Naukri Scraper

> Extract job listings from Naukri.com -- India's largest job portal with 100M+ resumes

[![Try on Apify](https://img.shields.io/badge/Try_on-Apify_Store-00C853?style=for-the-badge)](https://apify.com/thirdwatch)
[![Website](https://img.shields.io/badge/Website-thirdwatch.dev-000?style=for-the-badge)](https://thirdwatch.dev)

## What it does

Scrapes Naukri.com job listings with full descriptions, company ratings, salary data, and required skills. Achieves 100% description extraction rate. Supports all Indian cities, experience levels, and industry filters. Ideal for India job market research.

## Output fields

| Field | Type | Description |
|-------|------|-------------|
| title | String | Job title |
| company | String | Company name |
| location | String | City and state in India |
| salary | Object | Parsed salary (min, max, currency, period) |
| experience | String | Required experience range |
| description | String | Full job description |
| skills | Array | Required skills list |
| rating | Number | Company rating on Naukri |
| industry | String | Company industry |
| postedDate | String | When the job was posted |
| url | String | Direct link to listing |

## Input parameters

| Parameter | Type | Description |
|-----------|------|-------------|
| queries | Array | Job search keywords (e.g., "python developer") |
| location | String | Indian city (Mumbai, Bangalore, Delhi, etc.) |
| maxResults | Number | Maximum results per query |
| experience | String | Experience range filter |

## Example output

```json
{
  "title": "Senior Python Developer",
  "company": "Infosys",
  "location": "Bangalore, Karnataka",
  "salary": {
    "min": 1500000,
    "max": 2500000,
    "currency": "INR",
    "period": "yearly"
  },
  "experience": "5-8 years",
  "description": "Looking for a Senior Python Developer with Django and REST API experience...",
  "skills": ["Python", "Django", "REST APIs", "PostgreSQL", "AWS"],
  "rating": 3.9,
  "industry": "IT Services & Consulting",
  "postedDate": "1 day ago",
  "url": "https://www.naukri.com/job-listings-..."
}
```

## Pricing

| Plan | Price |
|------|-------|
| Pay per result | $0.002/result |
| Free tier | Available on Apify |

## Use cases

- India job market research and salary benchmarking
- Build Indian job aggregator platforms
- Track tech hiring trends in Bangalore, Mumbai, Delhi
- Competitive analysis of Indian employers
- Skills demand analysis across Indian IT industry

## Getting started

1. Go to the [Apify Store](https://apify.com/thirdwatch)
2. Find the **Naukri Scraper**
3. Enter job keywords and Indian city
4. Run and download results as JSON, CSV, or Excel

## Related scrapers by Thirdwatch

- [AmbitionBox Scraper](https://github.com/thirdwatch-dev/ambitionbox-scraper) -- India salary & reviews
- [CutShort Scraper](https://github.com/thirdwatch-dev/cutshort-scraper) -- India tech jobs
- [Indeed Scraper](https://github.com/thirdwatch-dev/indeed-scraper) -- Global job listings
- [LinkedIn Jobs Scraper](https://github.com/thirdwatch-dev/linkedin-jobs-scraper) -- LinkedIn jobs
- [JustDial Scraper](https://github.com/thirdwatch-dev/justdial-scraper) -- India business data

## About Thirdwatch

[Thirdwatch](https://thirdwatch.dev) builds production-ready web scraping APIs. 18 scrapers for jobs, e-commerce, reviews, social media, and business data.

## License

MIT
