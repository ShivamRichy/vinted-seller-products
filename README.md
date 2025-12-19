# Vinted Seller Products Scraper
> A robust data extraction tool that collects detailed product listings from Vinted seller profiles. It helps analysts, resellers, and researchers turn seller catalogs into structured, actionable data with minimal effort.


<p align="center">
  <a href="https://bitbash.dev" target="_blank">
    <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/scraper.png" alt="Bitbash Banner" width="100%"></a>
</p>
<p align="center">
  <a href="https://t.me/Bitbash333" target="_blank">
    <img src="https://img.shields.io/badge/Chat%20on-Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram">
  </a>&nbsp;
  <a href="https://wa.me/923249868488?text=Hi%20BitBash%2C%20I'm%20interested%20in%20automation." target="_blank">
    <img src="https://img.shields.io/badge/Chat-WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="WhatsApp">
  </a>&nbsp;
  <a href="mailto:sale@bitbash.dev" target="_blank">
    <img src="https://img.shields.io/badge/Email-sale@bitbash.dev-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail">
  </a>&nbsp;
  <a href="https://bitbash.dev" target="_blank">
    <img src="https://img.shields.io/badge/Visit-Website-007BFF?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Website">
  </a>
</p>




<p align="center" style="font-weight:600; margin-top:8px; margin-bottom:8px;">
  Created by Bitbash, built to showcase our approach to Scraping and Automation!<br>
  If you are looking for <strong>vinted-seller-products</strong> you've just found your team — Let’s Chat. 👆👆
</p>


## Introduction
This project extracts comprehensive product information from Vinted seller profile pages across multiple regions.
It solves the challenge of manually tracking seller inventories, pricing, and engagement metrics.
It is built for resellers, market researchers, data analysts, and automation-focused developers.

### Seller Catalog Intelligence
- Collects structured product data from individual seller profiles
- Supports multiple country domains and localized listings
- Handles pagination and item limits reliably
- Produces clean, analysis-ready datasets

## Features
| Feature | Description |
|----------|-------------|
| Multi-country support | Works across all major Vinted country domains. |
| Pagination control | Scrape specific pages or control product volume per request. |
| Rich product fields | Captures pricing, images, condition, visibility, and engagement metrics. |
| Summary statistics | Generates seller-level insights like totals and averages. |
| Input validation | Ensures clean inputs and predictable results. |
| Error resilience | Handles missing data and network issues gracefully. |

---

## What Data This Scraper Extracts
| Field Name | Field Description |
|-------------|------------------|
| sellerUrl | Original seller profile URL. |
| country | Country domain used for extraction. |
| page | Page number scraped. |
| perPage | Items per page configuration. |
| productId | Unique product identifier. |
| title | Product title or name. |
| price | Price object with amount and currency. |
| currency | Currency code. |
| brand | Brand name if available. |
| size | Size information if available. |
| condition | Product condition label. |
| description | Seller-provided product description. |
| photos | Array of product image URLs. |
| url | Direct product page link. |
| isVisible | Visibility status of the item. |
| isSold | Indicates if the item is sold. |
| isReserved | Indicates if the item is reserved. |
| createdAt | Product creation timestamp. |
| updatedAt | Last update timestamp. |
| viewCount | Number of product views. |
| favouriteCount | Number of times favorited. |
| category | Product category if available. |
| timestamp | Data extraction timestamp. |

---

## Example Output

    [
          {
            "sellerUrl": "https://www.vinted.pt/member/74292334",
            "country": "pt",
            "page": 1,
            "perPage": 20,
            "productId": 6778683487,
            "title": "Casaco, cardigan amarelo. Tam S /M.",
            "price": {
              "amount": "7.5",
              "currency_code": "EUR"
            },
            "currency": "EUR",
            "brand": null,
            "size": null,
            "condition": "New without tags",
            "description": "Beautiful yellow cardigan in excellent condition...",
            "photos": [
              "https://images1.vinted.net/example1.jpeg",
              "https://images1.vinted.net/example2.jpeg"
            ],
            "url": "https://www.vinted.pt/items/6778683487",
            "isVisible": true,
            "isSold": false,
            "isReserved": false,
            "createdAt": "2024-01-15T10:30:00Z",
            "updatedAt": "2024-01-20T14:22:00Z",
            "viewCount": 156,
            "favouriteCount": 44,
            "category": "Women's Clothing",
            "timestamp": "2025-07-31T07:39:40.189Z"
          }
        ]

---

## Directory Structure Tree

    vinted-seller-products-scraper/
    ├── src/
    │   ├── runner.js
    │   ├── extractors/
    │   │   ├── sellerParser.js
    │   │   └── productParser.js
    │   ├── validators/
    │   │   └── inputValidator.js
    │   ├── services/
    │   │   ├── pagination.js
    │   │   └── summaryStats.js
    │   └── config/
    │       └── settings.example.json
    ├── data/
    │   ├── sample-input.json
    │   └── sample-output.json
    ├── package.json
    └── README.md

---

## Use Cases
- **Online resellers** use it to monitor competitor inventories, so they can adjust pricing strategies faster.
- **Market researchers** use it to analyze seller behavior, so they can identify demand and trends.
- **Data analysts** use it to build datasets for pricing models, so they can improve forecasting accuracy.
- **E-commerce teams** use it to track seller performance, so they can benchmark against competitors.

---

## FAQs
**Does this work for all Vinted regions?**
Yes, it supports all major Vinted country domains and localized seller profiles.

**Can I scrape multiple pages of a seller’s catalog?**
Yes, pagination settings allow you to control page numbers and items per page.

**What happens if a seller has no visible products?**
The output will be empty, and summary data can be used to confirm availability.

**Is the extracted data consistent across runs?**
Yes, structured validation and parsing ensure stable and predictable outputs.

---

### Performance Benchmarks and Results

**Primary Metric:** Processes up to 20 products per page with consistent response times.

**Reliability Metric:** Maintains a high success rate across supported country domains.

**Efficiency Metric:** Optimized pagination minimizes redundant requests and resource usage.

**Quality Metric:** High data completeness with validated fields and minimal missing values.


<p align="center">
<a href="https://calendar.app.google/74kEaAQ5LWbM8CQNA" target="_blank">
  <img src="https://img.shields.io/badge/Book%20a%20Call%20with%20Us-34A853?style=for-the-badge&logo=googlecalendar&logoColor=white" alt="Book a Call">
</a>
  <a href="https://www.youtube.com/@bitbash-demos/videos" target="_blank">
    <img src="https://img.shields.io/badge/🎥%20Watch%20demos%20-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="Watch on YouTube">
  </a>
</p>
<table>
  <tr>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/MLkvGB8ZZIk" target="_blank">
        <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/review1.gif" alt="Review 1" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        "Bitbash is a top-tier automation partner, innovative, reliable, and dedicated to delivering real results every time."
      </p>
      <p style="margin:10px 0 0; font-weight:600;">Nathan Pennington
        <br><span style="color:#888;">Marketer</span>
        <br><span style="color:#f5a623;">★★★★★</span>
      </p>
    </td>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/8-tw8Omw9qk" target="_blank">
        <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/review2.gif" alt="Review 2" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        "Bitbash delivers outstanding quality, speed, and professionalism, truly a team you can rely on."
      </p>
      <p style="margin:10px 0 0; font-weight:600;">Eliza
        <br><span style="color:#888;">SEO Affiliate Expert</span>
        <br><span style="color:#f5a623;">★★★★★</span>
      </p>
    </td>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/m-dRE1dj5-k?si=5kZNVlKsGUhg5Xtx" target="_blank">
        <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/review3.gif" alt="Review 3" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        "Exceptional results, clear communication, and flawless delivery. <br>Bitbash nailed it."
      </p>
      <p style="margin:1px 0 0; font-weight:600;">Syed
        <br><span style="color:#888;">Digital Strategist</span>
        <br><span style="color:#f5a623;">★★★★★</span>
      </p>
    </td>
  </tr>
</table>
