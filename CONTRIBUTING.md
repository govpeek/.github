# Contributing to Gov Peek

🎉 Thanks for your interest in contributing to **Gov Peek**!  
This project exists to make government information more accessible, transparent, and timely. Your contributions will help citizens worldwide stay informed.

---

## 🚀 How to Contribute

### 1. Reporting Issues
- Use the [GitHub Issues](../../issues) tab to report bugs, request features, or suggest improvements.
- Be clear and provide as much detail as possible (screenshots, logs, examples).

### 2. Adding a New Government Source
One of our biggest needs is expanding coverage across more countries and regions.

1. Identify an **official government source** (website, RSS, press release page, etc.).  
2. Create a scraper script (preferably with **Scrapy** or **Playwright**) following the `scrapers/` directory structure.  
3. Normalize the data into our common format:
   ```json
   {
      "id": "uuid", 
      "id_type": "uuid-v4", 
      "country": {
         "name": "Kenya",
         "code": "KE"
      },
      "source": {
         "name": "Ministry of Finance",
         "url": "https://mof.gov.ke"
      },
      "language": {
         "original": "sw",
         "translated": "en"
      },
      "title": "New tax policy announced",
      "url": "https://gov.ke/tax-news",
      "content": "...full article in original language...",
      "summary": "Government announced new tax rules effective next month.",
      "tags": ["economy", "finance", "policy"],
      "category": "Economy",
      "priority": "normal",
      "dates": {
         "published_local": "2025-09-01T10:30:00+03:00",
         "published_utc": "2025-09-01T07:30:00Z",
         "scraped_at": "2025-09-01T10:35:12Z",
         "updated_at": "2025-09-01T10:35:12Z"
      },
      "metadata": {
         "source_type": "website", 
         "scraper_version": "1.0.0",
         "content_type": "article"
      },
      "ai_processing": {
         "summarized": true,
         "translated": true,
         "sentiment": "neutral",
         "keywords": ["tax", "policy", "Kenya"]
      },
      "status": "active"

   }


4. Add tests and documentation for your scraper.
5. Submit a Pull Request.

### 3. Improving AI Summarization

* Help fine-tune the **HuggingFace summarization pipeline**.
* Contribute keyword extraction / translation improvements.
* Suggest or integrate open-source LLMs.

### 4. Enhancing Frontend / Mobile

* Web (React + Tailwind): Improve UI/UX of the dashboard.
* Mobile (Flutter): Add push notification and offline features.

---

## 📝 Pull Request Process

1. Fork the repository and create a branch:

   ```bash
   git checkout -b feature/add-new-scraper
   ```
2. Commit your changes with clear messages.
3. Ensure your code passes linting and tests.
4. Open a Pull Request (PR) with a description of your changes.

---

## 📜 Code of Conduct

We are a community-driven project.

* Be respectful.
* No harassment, hate speech, or discriminatory behavior.
* Help build a safe, welcoming environment.

---

## 📄 License

By contributing, you agree that your contributions will be licensed under the same license as the project:
**Creative Commons Attribution-NonCommercial 4.0 (CC BY-NC 4.0)**

---

💡 *Together, we can make governments more transparent and empower citizens worldwide!*
