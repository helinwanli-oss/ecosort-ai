# EcoSort AI: Local Waste & Recycling Assistant
Building AI course project

## Summary
EcoSort AI is a computer vision and text search application designed to help households correctly sort waste and recyclables. By combining AI classification with municipal sorting guidelines, it reduces contamination and promotes sustainability.

## Background
Incorrect waste sorting leads to millions of tons of recyclable material ending up in landfills due to contamination.
- **High Contamination Rates:** Residents are often uncertain about local municipal sorting rules.
- **Localized Rules:** Rules vary significantly between municipalities.
- **Motivation:** Improving household sorting accuracy increases municipal recycling efficiency and supports environmental sustainability.

## How is it used?
EcoSort AI is designed for residents and municipal sanitation personnel.
1. **Capture or Search:** The user takes a photo of an item or types a brief description.
2. **Classification & Guidance:** The system analyzes the input and returns the correct bin category and preparation steps.

![Recycling Illustration](https://images.unsplash.com/photo-1532996122724-e3c354a0b15b?auto=format&fit=crop&w=800&q=80)

## Data sources and AI methods
- **Data Sources:** Public waste datasets (like TrashNet) and open municipal data APIs.
- **AI Methods:** 
  - Convolutional Neural Networks (CNNs) for image recognition.
  - TF-IDF and Cosine Similarity for matching text descriptions.
  - k-Nearest Neighbors (k-NN) for baseline feature classification.

| Method | Target Task | Primary Advantage |
| :--- | :--- | :--- |
| CNN / MobileNet | Photo-based classification | High accuracy on visual inputs |
| TF-IDF Vectorizer | Text rule matching | Fast keyword and rule lookup |
| k-NN | Baseline prototype | Simple implementation and fast testing |

## Challenges
- **Material Ambiguity:** Composite materials are difficult to classify purely visually.
- **Contamination State:** The model cannot easily verify if an item has been adequately cleaned.
- **Regional Variations:** Rules differ across cities and countries.

## What next?
- Integrate barcode scanning using open product databases (e.g., Open Food Facts).
- Gamify waste sorting for local schools.
- Collaborate with local city waste councils.

## Acknowledgments
- Course project framework provided by [Building AI course](https://elementsofai.com) by Reaktor Innovations and the University of Helsinki.
- Waste classification dataset inspiration from the [TrashNet Dataset](https://github.com/garythung/trashnet) by Gary Thung and Mindy Yang.
- Photo by [Alfonso Navarro on Unsplash](https://unsplash.com/photos/q3_P668383o) / Unsplash License.
