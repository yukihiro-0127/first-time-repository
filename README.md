# LexiCore

LexiCore is a professional English learning experience designed for global enterprise work.

## Data addition workflow

All flashcard and quiz content lives in `data/vocab.json`.

### Format

```json
{
  "cards": [
    {
      "id": "exec-001",
      "en": "I want to flag the delivery risk before it escalates. Please confirm the mitigation path.",
      "ja": "納期リスクが悪化する前に共有します。対応方針の判断をお願いします。",
      "level": 4,
      "category": "Executive Communication",
      "tags": ["risk", "escalation", "mitigation", "timeline"]
    }
  ]
}
```

### Rules for adding data

- **Keep difficulty high**: sentences must reflect enterprise or consulting-grade English.
- **Match the existing keys**: `id`, `en`, `ja`, `level`, `category`, `tags`.
- **Levels**: use integers `3` to `5` (3 = advanced, 5 = most advanced).
- **Categories**: must be one of the 10 UI categories:
  1. Executive Communication
  2. Stakeholder Alignment
  3. Consulting & Problem Solving
  4. IT Architecture & Systems
  5. Cloud & Platform
  6. Delivery & Operations
  7. Risk & Change Management
  8. Project & Execution
  9. Negotiation & Contract
  10. Casual but Professional
- **Tags**: include multiple tags such as `risk`, `assumption`, `alignment`, `trade-off`, `ownership`,
  `dependency`, `mitigation`, `escalation`, `timeline`, `deliverable`.

After updating `data/vocab.json`, reload the page to pick up new content.
