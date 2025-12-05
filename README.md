**Dataset of literature related to ancient, mediaeval & modern India** 🌐

## 📖 Overview

This repository collects metadata about literature from three broad periods of Indian history — **ancient**, **mediaeval**, and **modern** — in separate JSON data files. The goal is to provide a centralized, structured dataset to help researchers, students, and enthusiasts explore historical Indian literature across eras.

## 📂 Repository Contents

| File / Folder | Description |
|---------------|-------------|
| `ancient.json` | Metadata of literature works from ancient India (e.g. classical, Vedic, early historical texts) |
| `mediaeval.json` | Metadata of literature works from mediaeval India (e.g. medieval, regional, classical works) |
| `modern.json` | Metadata of modern Indian literature (post-colonial and contemporary works) |
| `LICENSE` | License file — this repository is licensed under GPL-3.0. |
| `README.md` | This file: project overview, usage, license, etc. |

> **Note:** Each JSON file contains a list of entries; each entry captures metadata such as title, author (if available), period / era, language, and other relevant fields (see an example below).

## 🛠️ Example Entry (in JSON)

```json
{
  "title": "Example Title",
  "author": "Author Name",
  "period": "Mediaeval",
  "language": "Sanskrit",
  "notes": "Additional information if any"
}
````

*(Actual fields may differ; check the JSON files directly for exact schema.)*

## 🔎 How to Use / Explore

You can use this dataset in several ways:

* Load the JSON files in your favorite programming language (Python, JS, etc.) to filter by period, language, author, etc.
* Combine the dataset with other metadata (e.g. publication date, translations) to build bibliographies, catalogs, or digital-library tooling.
* Extend the dataset by submitting new literature entries via a pull request.

```python
# Example (Python)
import json

with open('ancient.json', 'r', encoding='utf-8') as f:
    ancient_works = json.load(f)

print(len(ancient_works), "ancient works loaded.")
for work in ancient_works[:5]:
    print(work.get('title'), "-", work.get('author'))
```

## 🤝 Contributing

Contributions are welcome! If you’d like to add more literature entries, please follow these steps:

1. Fork the repository.
2. Add the new entry in the appropriate JSON file (ancient.json / mediaeval.json / modern.json), following the existing schema.
3. (Optional) If your data includes additional fields (e.g. original language script, transliteration, publication info), include a comment or rationale.
4. Commit your changes and open a pull request.

Please ensure entries are as accurate and complete as possible (author, period, language, etc.), and avoid duplicates.

## 📄 License

This project is licensed under the [GPL-3.0 License](LICENSE).

By using or contributing to this dataset, you agree to abide by the terms of the license.

## 💡 Why This Project Exists

* Historical and literary research often requires collating scattered information across many resources; this dataset aims to simplify and centralize that metadata.
* Facilitate better accessibility of Indian literary heritage — users can easily filter and search through literature across ages and languages.
* Encourage community-driven growth: this is envisioned as a living dataset that grows over time through contributions.

## 📬 Contact / Maintainers

If you find errors or wish to propose major changes (e.g. schema updates), feel free to open an issue or pull request.
For specific queries, you can reach out via GitHub discussions / issues on this repository.

---

Thank you for your interest in historic_literature_india — we hope it becomes a useful resource for everyone exploring India's vast literary heritage! 🙏
