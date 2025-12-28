# SunCountryAirlines Customer Analysis
## 📌 Project Purpose
This project aims to identify distinct customer segments by applying **K-Means clustering** and understand their booking and spending behaviors using airline transaction data, with the goal of **uncovering key drivers of customer value**. The findings are intended to support data-driven marketing and revenue decisions.

## 📊 Dataset Description
Used three main datasets derived from internal airline booking data:
- `sample_data_transformed.csv` – Original customer booking dataset with mixed categorical and numeric features
- `Clustering Data.csv` – Cleaned and encoded data with categorical variables converted to numerical values
- `final_dataframe_clusters.csv` – Final data frame with assigned cluster labels

**Customer Data Dictionary:**
| Column Name | Description |
|--------------|-------------|
| `uid` | Unique identifier for each customer |
| `age_group` | Categorized age range of the customer |
| `BookingChannel` | Method used for booking (Website, App, etc.) |
| `TripType` | Whether the customer booked a round-trip or one-way ticket |
| `UFlyMembership` | Indicates if the customer is a member of the loyalty program |
| `DaysPreBooked` | Number of days the booking was made in advance |
| `seasonality` | Which qaurter the flight was made |
| `BkdClassOfService` | What class of service (coach, first class, etc) the passenger booked |
| `TrvldClassOfService` | What class of service the passenger actually travelled on -- could be an upgrade |

## 🏷️ Methodology
### 1️⃣ Data Preprocessing
- Checked no missing values
- Standardized and normalized numerical fields
- Encoded categorical features for clustering

### 2️⃣ K-Means Clustering
- Applied the elbow method to determine the optimal number of clusters (K=5)
- Assigned customers to one of five clusters based on booking behavior and demographics
- Merged cluster labels into final dataset for analysis and visualization

### 3️⃣ Data Visualization
Visualized behavioral differences across clusters to understand customer characteristics, including:
- Age distribution
- Group size and booking channels
- Advance booking behavior and roundtrip preferences
- Travel seasonality across quarters (Q1–Q4)
- Spending patterns and loyalty program participation

## 🔍 Key Findings & Insights
### Segment 1: Big Spenders
- High average ticket spending despite low loyalty enrollment
- Contribute disproportionately to revenue
- Represent strong potential for retention and premium conversion
- **Strategy**: premium bundles, loyalty fast-track, retention incentives

### Segment 2: MSP Locals
- Largest customer segment by volume
- Primarily non-loyalty members traveling from Minneapolis–St. Paul
- High-impact target for loyalty program acquisition
- **Strategy**: location-based loyalty offers, targeted enrollment campaigns

### Segment 3: Loyal Customers
- Enrolled in Ufly loyalty program
- More likely to book directly through Sun Country’s website
- Exhibit higher repeat purchase and upgrade behavior
- **Strategy**: personalized rewards, tiered benefits, upselling opportunities

### Segment 4: Spontaneous Savers
- Highly price-sensitive and last-minute bookers
- Frequent ticket changes and low loyalty participation
- Respond well to flexible pricing and change-friendly policies
- **Strategy**: personalized rewards, tiered benefits, upselling opportunities

### Segment 5: Minneapolis Frequenters
- Younger travelers with frequent trips into MSP
- Low membership penetration despite high travel frequency
- Suitable for targeted local partnerships and membership incentives
- **Strategy**: flexible pricing, time-sensitive promotions, change-friendly policies

## 🚀 Business Implications
- **Customer segments show clear differences in behavior**
  - Booking patterns, price sensitivity, and loyalty usage vary across customer groups
  - A single, uniform marketing strategy is unlikely to be effective

- **Loyalty programs remain an important growth opportunity**
  - A large portion of frequent or high-spending customers are not enrolled in the loyalty program
  - Increasing loyalty participation may improve repeat purchases and customer retention

- **Booking channels influence overall performance**
  - Direct bookings support stronger customer relationships
  - Reliance on third-party platforms may increase distribution costs

- **Revenue growth depends on both acquisition and retention**
  - Different customer segments contribute value in different ways
  - Segment-specific strategies are needed to balance short-term demand and long-term growth
