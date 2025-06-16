# OCR Asset Tag Extractor

Uses PaddleOCR to extract asset tag numbers from images and classify them by suffix (e.g. `LPTP` = laptop). Outputs a CSV file.

---

## How It Works

1. Reads images from `data/raw_images/`
2. Extracts text using PaddleOCR
3. Filters tags starting with `DA`
4. Classifies by suffix using `suffix_map.json`
5. Saves to `output/extracted_asset_tags_{date}.csv`

---

## Folder Structure

```
asset_tag_extractor/
├── notebooks/
│ └── OCR_Asset_Tag_Extractor.ipynb
├── data/
│ ├── raw_images/
│ └── suffix_map.json
├── output/
│ └── extracted_asset_tags.csv
├── requirements.txt
└── README.md
```

---

