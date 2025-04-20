# 🏦 Bank Customer Reviews Analysis — Excel Power Query Project

This project demonstrates a full Excel Power Query workflow applied to a real-world customer review dataset from Kaggle. The goal was to clean, transform, enrich, and automate the processing of bank review data to prepare it for meaningful analysis.

---

## 📁 Project Structure


---

## 📊 Dataset Overview

This project uses the [Bank Customer Reviews Dataset](https://www.kaggle.com/datasets/dhavalrupapara/banks-customer-reviews-dataset) by **Dhaval Rupapara** on Kaggle. It contains over 1000 user-generated reviews and ratings about various banks.

### Key Fields:
- `author`: Reviewer's name  
- `date`: Date of the review  
- `address`: Reviewer's location  
- `bank`: Name of the bank  
- `rating`: User rating (1–5 stars)  
- `review`: Full review text  
- `rating_title_by_user`: User's summary title of the rating  
- `useful_count`: Number of helpful votes  
- Plus engineered fields like: `Review_Length`, `Review_Sentiment`, `year`, `city_bank`, and split title columns

---

## ✅ Transformation Steps

### Part 1: Import & Initial Setup
- Loaded CSV via Power Query as `Bank_Reviews_Raw`
- Promoted headers, set data types
- Saved as connection only

### Part 2: Cleaning & Prep
- Duplicated as `Bank_Reviews_Cleaned`
- Removed nulls, trimmed spaces
- Replaced missing values
- Split `Review_Title` → `title_tag`, `title_headline`

### Part 3: Feature Engineering
- Created `Review_Length` (word count)
- Added `Review_Sentiment` (Positive/Neutral/Negative)
- Extracted `year` and created `city_bank` column

### Part 4: Advanced Transformations
- Duplicated into `Bank_Reviews_Final`
- Renamed columns, added `Detailed`/`Short` classification
- Calculated optional impact metrics

### Part 5: Save Final Output
- Exported final table to `cleaned_reviews.xlsx`

### Part 6: Folder Import + Function (Optional)
- Imported multiple CSVs from a folder
- Used `Transform Sample File` to apply same logic
- Output combined as `combined_reviews.xlsx`

---

## 🧰 Tools & Techniques Used

- Microsoft Excel Power Query (M Language)
- Column splitting, trimming, replacing, conditional logic
- Column from examples
- Folder import with automatic function generation
- Custom and calculated columns

---

## 🔍 Use Case

This project simulates a real-world scenario in which analysts automate the processing of ongoing customer reviews from various sources. It showcases the ability to clean, transform, and combine multiple datasets efficiently using Excel.

---

## 📈 Outputs

- `cleaned_reviews.xlsx`: Final cleaned review dataset
- `combined_reviews.xlsx`: Merged data from multiple review files

---

## 📚 Dataset Source

- [Kaggle - Bank Customer Reviews Dataset by Dhaval Rupapara](https://www.kaggle.com/datasets/dhavalrupapara/banks-customer-reviews-dataset)

---


