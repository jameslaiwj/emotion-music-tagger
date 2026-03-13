## 🎵 Emotion-Based Music Tagging Tool for Indie Artists
### From Studio to Screen: A Roadmap for Indie Artists to Land Film & TV Placements
__General Assembly Data Analytics Capstone | James Lai | February 2026__

---
## 🎯 The Opportunity
Indie artists create great music. The problem is getting it heard and paid for.

Spotify's 2024 royalty changes introduced a 1,000 stream threshold for tracks to generate recorded royalties, redistributing payments toward professional artists. For indie artists with large catalogs, many tracks will never reach this threshold through streaming alone.

__Sync Licensing offers a direct alternative:__ one placement can earn $500 to $5,000 regardless of stream count. But without emotion tags, catalogs remain invisible to music supervisors who search by mood.

This project bridges that gap using open-source machine learning and publicly available Spotify audio data from Kaggle.

---
## ❓ Research Question
> Can open-source machine learning replicate commercial emotion tagging at >= 85% accuracy?

---
## 💡 Solution
A Random Forest Classifier trained on ~278,000 labeled songs to predict single-precision emotion tags __(Sad, Happy, Energetic, Calm)__ across any music catalog, regardless of release year or genre.

The goal is not to challenge existing models, but to apply audio feature analysis to a real-world problem: helping indie artists tag their catalogs for sync licensing opportunities, at zero cost.

---
## 📊 Value Proposition
__🎸 For Indie Artists:__
- ⏱️ Tag 1,000 songs in under 2 hours vs 110+ hours manually
- 💰 $0 cost vs commercial alternatives where pricing requires direct engagement or enterprise plans (e.g. Cyanite.ai, free tier is limited to 5 songs per month)
- 🗂️ Works on any catalog regardless of release year
- 🔓 Full control over emotion categories, no vendor lock-in

---
__🏭 For the industry:__
- 🔍 Music supervisors find songs faster through better-tagged databases
- 📈 Sync platforms increase catalog discoverability
- 🌍 Democratises access to tools currently reserved for major labels

---
## 🔬 Methodology Notes & Assumptions
- 110+ hours based on average 3 to 4 minute average song length per 1,000 song catalog, accounting for listening, breaks, spreadsheet updates and spot-checking
- Under 2 hours includes model runtime (~1 minute) plus human review of flagged tracks
- Outliers retained in analysis to preserve genre diversity

---
## 🛠️ Tech Stack
| __Tool__ | __Usage__ | 
| :--- | :--- | 
| Python (Pandas, Scikit-learn, Matplotlib) | Data pipeline, modelling, visualisation |
| Tableau | Interactive dashboard |
| Kaggle Datasets | Training and validation data |

---
## 📁 Dataset
- __Training__: [278K Emotion Labeled Spotify Songs](https://www.kaggle.com/datasets/abdullahorzan/moodify-dataset/data)
  License: CC BY 4.0
- __Validation__: [Spotify_1Million_Tracks](https://www.kaggle.com/datasets/amitanshjoshi/spotify-1million-tracks) License: ODbL, contents © Original Authors

---
## 🤖 Model
__Random Forest Classifier__, selected over Logistic Regression for robustness to outliers, feature importance transparency and __91% classification accuracy__.

---
## 📈 Dashboard
Interactive Tableau Dashboard with human-in-the-loop validation (Perfect / Acceptable / Error confidence tiers).

👉 [View Dashboard on Tableau Public](https://public.tableau.com/app/profile/jameslaiwj/viz/Tableau_Interactive_Dashboard-Server/1_EmotionDistribution)

---
## 📂 Repository Contents
- 📓 Jupyter Notebook: Data Pipeline, feature engineering and model training
- 📑 Presentation PDF: From Studio to Screen (Full capstone slides)

---
## 📜 Data Source Acknowledgement
- 278K Emotion Labeled Spotify Songs: Licensed under CC BY 4.0. Source: Kaggle
- 1M Spotify Tracks: ODbL License, contents © Original Authors. Source: Kaggle

> ⚠️ $\color{#D97706}{\text{This project is for educational purposes only.}}$

---
## 🚀 Next Steps
Migration to Librosa following Spotify API access restrictions in November 2024, maintaining feature parity for continued free audio analysis.

## 🤝 Connect
- 💼 LinkedIn: [James Lai](https://www.linkedin.com/in/jameslaiwj/)
- 📊 Tableau Public: [James Lai](https://public.tableau.com/app/profile/jameslaiwj/vizzes)
- 🌐 Portfolio: [James Lai](https://jameslaiwj.github.io)
