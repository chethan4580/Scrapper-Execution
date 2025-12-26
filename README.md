# Overview

This project implements a lightweight, rule-based web scraper that converts a company website URL into a structured Company Information Record.

The focus of this task is not to build a perfect scraper, but to demonstrate the ability to:

* Handle ambiguity in real-world data
* Extract only reliable, observable information
* Produce clean, structured output
* Clearly log limitations instead of hallucinating data

The scraper is intentionally simple, deterministic, and easy to reason about, prioritizing correctness and transparency over complexity.

# Dependencies

The project requires the following Python libraries:

* requests
* beautifulsoup4

Install the dependencies using:


* pip install requests beautifulsoup4

# How to Run

* Ensure Python 3.x is installed
* Install the required dependencies

Run the scraper from the terminal:


* python scraper.py


Enter a company website URL when prompted.

# Example Command

* Input: URL()
* Enter company website URL: https://www.zoho.com

# Sample Output

```json
{
  "identity": {
    "company_name": "Zoho | Cloud Software Suite for Businesses",
    "website_url": "https://www.zoho.com",
    "tagline": null
  },
  "business_summary": {
    "what_they_do": "A unique and powerful software suite to transform the way you work. Designed for businesses of all sizes, built by a company that values your privacy. Run your entire business on Zoho with our unified cloud software, designed to help you break down silos between departments and increase organizational efficiency.",
    "primary_offerings": [],
    "target_customer_segments": []
  },
  "evidence_proof": {
    "key_pages_detected": [
      "Home",
      "Products"
    ],
    "signals_found": [],
    "social_links": {
      "twitter": "https://twitter.com/ZohoBooks",
      "instagram": "https://www.instagram.com/zoho_books/",
      "youtube": "https://www.youtube.com/channel/UC12OzqYu2z-D6mVJCTjQvwg",
      "linkedin": "https://www.linkedin.com/showcase/zoho-books/"
    }
  },
  "contact_location": {
    "emails": [
      "brandon@zillium.com",
      "sales@zohocorp.com",
      "support.usa@zohobooks.com"
    ],
    "phones": [],
    "address": null,
    "contact_page_url": null
  },
  "team_hiring_signals": {
    "careers_page_url": null,
    "roles_or_departments_mentioned": []
  },
  "metadata": {
    "timestamp_of_scrape": "2025-12-25 16:52:46",
    "pages_visited": [
      "https://www.zoho.com",
      "https://www.zoho.com/privacy-commitment.html?src=zindex",
      "https://www.zoho.com/signup.html?src=zindex",
      "https://www.zoho.com/all-products.html?src=zindex",
      "https://www.zoho.com/crm/?ireft=nhome&src=fa",
      "https://www.zoho.com/mail/?ireft=nhome&src=fa",
      "https://www.zoho.com/books/?ireft=nhome&src=fa",
      "https://www.zoho.com/people/?ireft=nhome&src=fa",
      "https://www.zoho.com/desk/?ireft=nhome&src=fa",
      "https://www.zoho.com/time/?src=zindex"
    ],
    "errors_or_fallbacks_used": []
  }
}

