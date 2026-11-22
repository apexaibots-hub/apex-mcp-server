# ApexAiBots Web Scraping & Data Intelligence MCP

Official Model Context Protocol (MCP) configuration giving **Claude Desktop**, **Cursor**, **Windsurf**, and custom AI agents instant access to **15+ zero-maintenance web scrapers and real-time data APIs** powered by Apify (`https://apify.com/apex_scrapers`).

## Included MCP Tools (15 Production Scrapers)

1. **DexScreener Multi-Chain DEX Liquidity Tracker Pro** — Real-time token liquidity, volume, and pairs across Solana, Base, Ethereum, and BSC.
2. **Sports Odds & Line Movement Live Scores Monitor Pro** — Live odds, spreads, totals, and line movements across NFL, NBA, MLB, NHL, and soccer.
3. **Website Tech Stack, CMS & SEO Metadata Auditor** — Detect frameworks, analytics, CDNs, and SEO tags on any domain.
4. **RSS, News & Blog Article Bulk Extractor** — Clean full-text article extraction from RSS/Atom feeds.
5. **Multi-Board Tech & Remote Jobs Salary Extractor** — Structured remote/tech job listings with salary ranges.
6. **E-Commerce Product Price, Stock & Review Tracker** — Extract live pricing, availability, and ratings from product pages.
7. **Local Business Contact & Lead Extractor** — Structured business names, addresses, phones, websites, and ratings by niche and city.
8. **YouTube Video Transcript, Caption & Metadata Bulk Extractor Pro** — Full transcripts, timestamps, and metadata for RAG and AI pipelines.
9. **Reddit Subreddit, Thread & Comment Sentiment Scraper Pro** — Subreddit posts, nested comments, and engagement metrics.
10. **Trustpilot Business Review & Sentiment Scraper Pro** — Verified customer reviews, star ratings, and sentiment data.
11. **Shopify Store Product Catalog & Variant Price Extractor Pro** — Complete product catalogs, variants, SKUs, and prices from any Shopify store.
12. **Apple App Store Reviews, Ratings & App Intelligence Scraper Pro** — App metadata, version history, and user reviews by country.
13. **Google Search Autocomplete & Long-Tail Keyword SEO Pro** — Real-time search suggestions and keyword expansion.
14. **GitHub Repository & Developer Intelligence Pro** — Repo stats, release tracking, and developer ecosystem data.
15. **Hacker News & YC Startup Intelligence Pro** — Front-page stories, Ask/Show HN threads, and startup trends.

## Quick Setup (Claude Desktop & Cursor)

Add the following block to your `claude_desktop_config.json` or `.cursor/mcp.json` file (replace `YOUR_APIFY_API_TOKEN` with your free or paid Apify API token):

```json
{
  "mcpServers": {
    "apexaibots-scrapers": {
      "command": "npx",
      "args": [
        "-y",
        "mcp-remote",
        "https://mcp.apify.com?actors=apex_scrapers/dexscreener-multi-chain-dex-liquidity-tracker-pro,apex_scrapers/sports-odds-line-movement-live-scores-monitor-pro,apex_scrapers/website-tech-stack-cms-seo-metadata-auditor,apex_scrapers/rss-news-blog-article-bulk-extractor,apex_scrapers/multi-board-tech-remote-jobs-salary-extractor,apex_scrapers/e-commerce-product-price-stock-review-tracker,apex_scrapers/local-business-contact-lead-extractor,apex_scrapers/youtube-video-transcript-caption-metadata-bulk-extractor-pro,apex_scrapers/reddit-subreddit-thread-comment-sentiment-scraper-pro,apex_scrapers/trustpilot-business-review-sentiment-scraper-pro,apex_scrapers/shopify-store-product-catalog-variant-price-extractor-pro,apex_scrapers/apple-app-store-reviews-ratings-app-intelligence-scraper-pro,apex_scrapers/google-autocomplete-keyword-seo-pro,apex_scrapers/github-repository-developer-intelligence-pro,apex_scrapers/hacker-news-yc-startup-intelligence-pro"
      ],
      "env": {
        "APIFY_TOKEN": "YOUR_APIFY_API_TOKEN"
      }
    }
  }
}
```

## Links
* **Apify Store Profile:** `https://apify.com/apex_scrapers`
* **n8n Automation Templates:** `https://github.com/apexaibots-hub/apify-n8n-automation-templates`
