#  Profitable App Profiles for the App Store & Google Play

##  Project Overview
This project analyses mobile app data from the Apple App Store and Google Play Store to identify app categories with strong user demand and monetisation potential.

The business scenario assumes a company that develops **free mobile applications** and generates revenue primarily through **in-app advertising**. Since ad revenue depends heavily on user engagement and install volume, the objective is to determine which types of apps are most likely to attract large audiences.

---

#  Objectives
- Clean and prepare app store datasets for analysis
- Identify the most common app genres on each platform
- Measure user demand using installs and ratings as proxies
- Compare demand against market competition
- Recommend an app category with strong business potential

---

#  Datasets Used

## Google Play Store
- Dataset: `googleplaystore.csv`
- Platform: Android

### Key Variables
- App category
- Installs
- Reviews
- Price

---

## Apple App Store
- Dataset: `AppleStore.csv`
- Platform: iOS

### Key Variables
- Genre
- Rating counts
- Price

---

#  Technologies & Skills Used
- Python (base Python only — no pandas)
- CSV handling
- Loops and conditional logic
- Dictionaries and lists
- Frequency tables
- Data cleaning
- Business analysis

---

#  Data Cleaning & Preparation

## 1. Removed Corrupted Records
The Google Play dataset contained a malformed row with inconsistent column length. This row was removed to maintain dataset integrity.

## 2. Removed Duplicate Apps
Duplicate applications were identified in the Google Play dataset.

For each duplicated app, only the entry with the highest review count was retained to preserve the most complete record.

## 3. Filtered Free Applications
Since the business model relies on advertising revenue, only free applications were included in the analysis.

## 4. Filtered English-Language Apps
A character-based filtering function was used to retain English-language applications targeting a broad global audience.

---

#  Analysis Performed

## 1. Genre Frequency Analysis
Calculated the percentage distribution of app categories and genres across both platforms to understand market composition.

## 2. Weighted Demand Analysis
Instead of relying only on genre frequency, app popularity was measured using:

- **Average installs per category** (Android)
- **Average rating counts per genre** (iOS)

This approach provides a stronger estimate of user demand by accounting for both popularity and competition levels.

---

#  Key Findings

## 🔹 Android (Google Play)

| Category | Avg Installs | Apps |
|---|---:|---:|
| Communication | 38.3M | 288 |
| Video Players | 24.6M | 160 |
| Social | 23.3M | 236 |
| Photography | 17.8M | 262 |
| Productivity | 16.7M | 346 |

### Key Insight
Although Communication and Social apps attract extremely large audiences, these categories are highly saturated and dominated by major platforms such as WhatsApp, YouTube, and Instagram.

Productivity apps demonstrated strong install numbers while offering more realistic entry opportunities for smaller developers.

---

## 🔹 iOS (Apple App Store)

| Genre | Avg Ratings | Apps |
|---|---:|---:|
| Reference | 67.4K | 20 |
| Music | 56.5K | 67 |
| Social Networking | 53.1K | 143 |
| Weather | 47.2K | 31 |

### Key Insight
Reference apps showed the highest average engagement while maintaining relatively low competition, suggesting a strong market opportunity.

---

#  Final Recommendation

Based on the analysis, the strongest opportunity would be to develop a:

##  Productivity or Educational Reference App

This recommendation is based on:
- Strong user demand
- Lower market saturation
- Cross-platform viability
- Long-term engagement potential
- Strong monetisation opportunities through ads or subscriptions

Highly competitive categories such as social networking and gaming were avoided due to market dominance by established platforms.

---

#  Key Takeaways
- User demand is more important than raw genre frequency
- High-install categories are not always the best business opportunities
- Balancing demand and competition is critical for product strategy
- Productivity and reference-based applications offer attractive market potential for smaller entrants

---

# Author

Steven Tapscott
