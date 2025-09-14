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
     "country": "Country Name",
     "source": "Official Department Name",
     "title": "Article Title",
     "date": "YYYY-MM-DD",
     "url": "https://example.gov/...",
     "content": "Full text of the news",
     "summary": "AI-generated summary",
     "tags": ["health", "economy"]
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
