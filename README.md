# Amazon Product Scraper

[amazon-product-scraper](https://apify.com/logical_scrapers/amazon-product-scraper)

Amazon Product Scraperis a powerful actor that scrapes detailed product information from Amazon.com product pages. This scraper handles product details including title, price, features, images, and technical specifications.

## Product Details Output Data

| Field        | Description                | Example                                          |
| ------------ | -------------------------- | ------------------------------------------------ |
| name         | Product title              | "Apple iPhone 13 Pro Max"                        |
| asin         | Amazon's unique product ID | "B09G9HD6PD"                                     |
| style        | Product style/variant      | "256GB, Sierra Blue"                             |
| description  | Full product description   | "6.7-inch Super Retina XDR display..."           |
| stars        | Product rating out of 5    | "4.8 out of 5 stars"                             |
| rating_count | Number of ratings          | "12,345 ratings"                                 |
| features     | List of product features   | ["5G Capable", "A15 Bionic chip"...]             |
| images       | List of product image URLs | ["https://images-na.ssl-images-amazon.com/..."]  |
| info_table   | Technical specifications   | {"Brand": "Apple", "Model": "iPhone 13 Pro Max"} |

## Input

```json
{
  "urls": [
    "https://www.amazon.com/dp/B09G9HD6PD",
    "https://www.amazon.com/dp/B08L5TNJHG"
  ]
}
```

## Output Example

```json
{
  "name": "Apple 2023 MacBook Pro Laptop M3 Pro chip",
  "asin": "B0CWJB9ZC6",
  "style": "M3 Pro chip",
  "description": "SUPERCHARGED BY M3 PRO — The Apple M3 Pro chip with an 11-core CPU and 14-core GPU delivers exceptional performance for demanding workflows like manipulating gigapixel images or compiling code.",
  "stars": "4.5 out of 5 stars",
  "rating_count": "123 ratings",
  "features": [
    "SUPERCHARGED BY M3 PRO",
    "UP TO 18 HOURS OF BATTERY LIFE",
    "BRILLIANT PRO DISPLAY",
    "ADVANCED CAMERA AND AUDIO"
  ],
  "images": [
    "https://m.media-amazon.com/images/I/61lsexTCOhL._AC_SL1500_.jpg",
    "https://m.media-amazon.com/images/I/71Kq8oWn7bL._AC_SL1500_.jpg"
  ],
  "info_table": {
    "Brand": "Apple",
    "Model": "MacBook Pro",
    "CPU Manufacturer": "Apple",
    "Color": "Space Black",
    "Screen Size": "14.2 Inches",
    "Hard Disk Size": "512 GB"
  }
}
```

## Other Available Scrapers

## Available Scrapers

| Scraper Name             | Description                                                                     | Input Type         | Link                                                                      |
| ------------------------ | ------------------------------------------------------------------------------- | ------------------ | ------------------------------------------------------------------------- |
| Amazon Product Scraper   | Extracts detailed product information including specs, images, and pricing      | Product URLs       | [View Actor](https://apify.com/logical_scrapers/amazon-product-scraper)   |
| Amazon Search Scraper    | Scrapes product listings from search results                                    | Search URL         | [View Actor](https://apify.com/logical_scrapers/amazon-search-scraper)    |
| Amazon Review Scraper    | Extracts product reviews and ratings                                            | Product Review URL | [View Actor](https://apify.com/logical_scrapers/amazon-review-scraper)    |
| LinkedIn Profile Scraper | Extracts comprehensive profile data including experience, education, and skills | Profile URLs       | [View Actor](https://apify.com/logical_scrapers/linkedin-profile-scraper) |
| LinkedIn Company Scraper | Scrapes company details, employees, and updates                                 | Company URLs       | [View Actor](https://apify.com/logical_scrapers/linkedin-company-scraper) |
| TikTok Video Scraper     | Downloads TikTok videos with metadata and engagement metrics                    | Video URLs         | [View Actor](https://apify.com/logical_scrapers/tiktok-video-scraper)     |
