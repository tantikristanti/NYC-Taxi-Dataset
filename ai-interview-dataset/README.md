## 🤖 AI Interview Dataset

This dataset contains curated interview questions and answers for technical roles in artificial intelligence, including AI Engineering, Machine Learning, Natural Language Processing, Computer Vision, Data Engineering, and Data Science.

**Releases**

* Data Science technical QA: https://github.com/tantikristanti/Datasets/releases/download/v1.0.0-ds-qa-alpha/ds-qa-technical.json
* Data Science theory QA: https://github.com/tantikristanti/Datasets/releases/download/v1.0.0-ds-qa-alpha/ds-qa-theory.json


## 🖼️ **Folder Structure**

```
ai-interview-dataset/
├── data/
│   ├── qa/                         # Interview questions and answers (Json)
│   │   └── json/                   # Json files are available for download in releases
│   │   │   └── qa-*-*.json         
│   ├── images/                     # Visual explanations
│   │   ├── *.png
│   ├── formulas/                   # Mathematical expressions 
│   │   ├── *.tex
│   ├── codes/                      # Executable code snippets
│   │   ├── python/
│   │   │   └── *.py
│   │   ├── java/
│   │   │   └── *.java
│   │   └── sql/
│   │       └── *.sql
│   ├── articles/                   # Source articles
│   │   ├── *.pdf
│   └── metadata/
│       ├── sources.json
└── README.md
```

## 📄 **JSON Structure**

```json
{
  "questions": [
    {
      "question_id": "qa-nlp-0001",
      "question_title": "NLP-theory",
      "question_text": "Explain the difference between BERT and GPT architectures.",
      "answer_text": "BERT is bidirectional and uses masked language modeling...",
      "resources": {
        "images": [
          {
            "file_name": "bert_vs_gpt.png",
            "description": "Architecture comparison diagram"
          },
          {
            "file_name": "attention_flow.jpg",
            "description": "Attention mechanism flow"
          }
        ],
        "formulas": [
          {
            "file_name": "attention_formula.tex",
            "rendered_name": "attention_formula.png",
            "description": "Self-attention mathematical formulation"
          }
        ],
        "codes": [
          {
            "language": "python",
            "code": "for i in range(1, 101):\n\n    if i % 3 == 0",
            "description": "Basic transformer implementation"
          }
        ],
        "articles": [
          {
            "type": "paper",
            "path": "articles/attention_paper.pdf",
            "description": "Original Attention Is All You Need paper"
          }
        ]
      }
    }
  ],
  "metadata": {
    "source": "URL to GitHub repo",
    "has_images": true,
    "has_formulas": true,
    "has_codes": true,
    "has_articles": true,
    "paths": {
      "relative_to_dataset_root": true,
      "base_directory": "ai-interview-dataset",
      "resource_structure": {
        "images": "/data/images/",
        "formulas": "/data/formulas/",
        "codes": "/data/codes/",
        "articles": "/data/articles/"
      }
    }
  }
}
```

**Dataset Contents**

This dataset includes:

* Technical questions covering fundamentals, theory, and applied problem-solving.
* Answers and solution explanations, including conceptual breakdowns and code examples where applicable.
* Role-specific categories (AI, ML, NLP, CV, Data Engineering, Data Science).
* Difficulty levels (e.g., beginner, intermediate, advanced).
* Additional fields such as topic tags, company context (where available), and question sources.

**Data Sourcing**

The data is compiled and curated from publicly available sources including technical platforms (e.g., LeetCode, Glassdoor), community GitHub repositories, and curated interview preparation guides. All sources are credited in the repository's `references` section.

**Additional Resources**

For more context and study materials, please refer to:

* **Question Taxonomy & Study Guide**: A structured breakdown of topics and recommended learning paths.
* **Solution Code Repositories**: Links to external repos containing implemented solutions.
* **Contributing Guidelines**: Instructions on how to propose new questions or improve existing answers.

**Publication Schedule**

This is a static, versioned collection. Updates are released as new versions when significant additions or improvements are made.

**Disclaimer**

This dataset is provided "as-is" for educational and preparation purposes. Questions and answers are sourced from public domains and may not reflect the exact content of any specific company's interview process.

---

## References

1. [Data Science Interviews, Alexey Grigorev](https://github.com/alexeygrigorev/data-science-interviews).
2. [160+ Data Science Interview Questions, Alexey Grigorev, 2020](https://medium.com/data-science-insider/160-data-science-interview-questions-14dbd8bf0a08).
