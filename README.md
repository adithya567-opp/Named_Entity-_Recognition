 NER Comparison Using spaCy Models

This project compares the Named Entity Recognition (NER) performance of spaCy's small, medium, and large English models on a sample historical text. The focus is on extracting entities of types: `DATE`, `PERSON`, and `EVENT`.

## 🔧 Models Used

- `en_core_web_sm` – Small
- `en_core_web_md` – Medium
- `en_core_web_lg` – Large

Implemented in **Google Colab** using **spaCy** and **pandas**.

## 📁 Contents
ner_comparison/
├── ner_comparison.ipynb # Main notebook
├── models/
│ ├── small_model_output.csv
│ ├── medium_model_output.csv
│ └── large_model_output.csv
├── analysis/ # Notes on output differences
│ └── ner_comparison_analysis.md
├── README.md
└── requirements.txt

Key Takeaways

- **Larger models** detect more accurate and context-aware entities.
- **Small model** misses complex cases and occasionally mislabels.
- Common error: All models tagged "Chapter" headings as `EVENT`.

---

 How to Run

1. Open `ner_comparison.ipynb` in Colab.
2. Install models:
   ```bash
   !python -m spacy download en_core_web_sm
   !python -m spacy download en_core_web_md
   !python -m spacy download en_core_web_lg
3. Run all cells.
