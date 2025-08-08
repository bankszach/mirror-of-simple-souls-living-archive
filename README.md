
# 🪞 Mirror of Simple Souls — Living-Archive Edition  
**Marguerite Porete’s 14th-century mystical masterpiece — rebuilt for the 21st century with AI-native pipelines**  
*Readable. Critical. French. Digital-native.*

---

## ✨ What is This?

This is **not** just a translation.

It’s a **triple-format, AI-orchestrated living archive** of *Le Mirouer des simples âmes anienties* (*The Mirror of Simple Souls*) — the controversial, poetic dialogue by Marguerite Porete that got her burned at the stake in 1310.

Inside this repository lives:
- **Original Old French** text (public domain)
- **Readable English** — smooth, modern prose for everyone
- **Critical English** — line-faithful, scholarly precision for the purists
- All in **JSON-LD** format for libraries, linked data projects, and AI ingestion.

---

## 📦 JSON Structure Overview

```jsonc
{
  "@context": "https://schema.org",
  "@type": "Book",
  "name": "Mirror of Simple Souls — Living-Archive Edition",
  "author": { "@type": "Person", "name": "Marguerite Porete" },
  "translator": [
    { "@type": "Person", "name": "Zach Banks" }
  ],
  "hasPart": [
    {
      "@type": "Chapter",
      "position": 1,
      "name": "Book I",
      "hasPart": [
        {
          "@type": "Chapter",
          "position": 1,
          "text_fr": "...",
          "text_en_readable": "...",
          "text_en_critical": "..."
        }
      ]
    }
  ]
}
````

* **`text_fr`** — Original Old French text
* **`text_en_readable`** — Modern, fluid English translation
* **`text_en_critical`** — Scholarly, literal English translation
* Nested `hasPart` arrays keep the original book → chapter hierarchy intact.
* All nodes have stable metadata for citation, linked data, and AI retrieval.

---

## 🤖 AI Integration

This edition was created using a **purpose-built AI orchestration pipeline**:

1. **Schema Design** — Defined a JSON-LD schema encoding bibliographic metadata + Agent-to-Agent (A2A) protocol hooks.
2. **Data Extraction** — Single-file Python script to parse the Old French PDF into structured JSON.
3. **Dual Translation** — Automated via the OpenAI Python SDK with GPT-4o, using highly-tuned prompts:

   * *Readable* → modern, flowing, idiomatic English.
   * *Critical* → literal, scholarly, doctrinally precise English.
4. **Comparative QA** — AI-assisted comparison against major published English editions (Babinsky, Kirchberger, Van Woerkom) to verify fidelity and style.
5. **Format Exports** — Scripts generate Markdown and other formats for human-friendly browsing and publication.

---

## 🔥 Why It Matters

* **Dual-track design** — No other edition gives you modern readability *and* scholarly literalness in the same file.
* **Digital-native from birth** — Ready for AI tools, annotation platforms, and library integration.
* **Proof-of-concept** — Shows how AI pipelines can empower non-specialists to produce world-class literary work.

---

## 📂 Repository Contents

```
mirror-of-simple-souls-ai-edition/
├── mirror_original_fr.md       # Old French text (Markdown export)
├── mirror_en_readable.md       # Readable English (Markdown export)
├── mirror_en_critical.md       # Critical English (Markdown export)
├── Mirror-of-Simple-Souls_Living-Archive-Edition_v1_FR-EN_Zach-Banks.json
├── scripts/                    # Extraction + translation scripts
├── README.md
└── LICENSE
```

---

## 🛠 How to Use

### Quick View

You can browse:

* `mirror_original_fr.md` — Old French
* `mirror_en_readable.md` — Modern English
* `mirror_en_critical.md` — Scholarly English

### AI Experiments

* Load the JSON into a vector database (Pinecone, Weaviate) for semantic search.
* Use as a **parallel corpus** for training translation models.
* Annotate with commentary, footnotes, or multimedia.

---

## 📜 License

* **Old French** text: Public Domain.
* **English translations**: Licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

You’re free to share and adapt with attribution.

---

## 🌍 Get Involved

* Open an issue to report typos or inconsistencies.
* Submit pull requests with improvements, annotations, or format conversions (EPUB, HTML, TEI XML).
* Use it in your research and tag me — I want to see it in action.

---

## ⚡ Author

**Zach Banks**
Construction foreman → AI pipeline builder → accidental medieval translator.

> *“If AI can help me create this, imagine what you can do with it.”*

---

## 📣 Spread the Word

If you think this project is cool:

* ⭐ Star the repo
* Share it on LinkedIn/Twitter/Reddit
* Tell a scholar, librarian, or AI tinkerer

---

> 🪞 *The Mirror still speaks — now in a voice anyone can hear.*




