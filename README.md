# Yelp Dataset Analysis & Visualization

![Yelp Logo](https://logos-world.net/wp-content/uploads/2020/11/Yelp-Logo.png)

## 📊 Project Overview

This project explores the Yelp review dataset to uncover insights about user behavior, business performance, and geographical trends. Using data visualization and statistical analysis, we reveal patterns that can help businesses improve their services and users make better decisions.

## 🔍 Key Findings

- Higher ratings (4★ and 5★) are significantly more common than negative ones, with 4-star being the most frequent rating
- Users write substantially longer reviews for negative experiences compared to positive ones
- Restaurants, shopping, and food services dominate the Yelp platform
- Clear patterns in check-in activity emerge across different days and times
- U.S. cities show grid-like business distributions, while European cities display more organic patterns

## 📋 Table of Contents

- [Dataset Description](#dataset-description)
- [Rating Distribution](#rating-distribution)
- [Business Categories](#business-categories)
- [Review Analysis](#review-analysis)
- [Geographical Insights](#geographical-insights)
- [Check-in Patterns](#check-in-patterns)
- [User Behavior Analysis](#user-behavior-analysis)
- [Business Case Study](#business-case-study)
- [Sentiment Analysis](#sentiment-analysis)
- [Technology Stack](#technology-stack)
- [Setup and Installation](#setup-and-installation)
- [Future Work](#future-work)

## 💾 Dataset Description

The analysis utilizes Yelp's comprehensive dataset containing:

| File | Description |
|------|-------------|
| `yelp_business.csv` | Business data including location, ratings, categories |
| `yelp_business_hours.csv` | Operating hours for businesses |
| `yelp_checkin.csv` | User check-ins at businesses |
| `yelp_review.csv` | Full text reviews, ratings, and votes |
| `yelp_tip.csv` | Short tips left by users |
| `yelp_user.csv` | User profiles and statistics |

## ⭐ Rating Distribution

![Rating Distribution](screenshots/rating_distribution.png)

Our analysis of 174,567 businesses shows:
- 4-star ratings are most common (19.2%)
- 3.5-star ratings follow closely (18.4%)
- 5-star ratings represent 15.8% of businesses
- Only 2.2% of businesses have the lowest 1-star rating

This positive skew reflects both user behavior and business survivorship bias.

## 🏪 Business Categories

![Top Categories](screenshots/top_categories.png)

The most represented business categories are:
1. Restaurants (19,469)
2. Shopping (13,712)
3. Food (10,656)
4. Home Services (6,885)
5. Nightlife (6,798)

With 59,106 unique categories overall, Yelp's ecosystem covers a remarkably diverse range of businesses.

## 📝 Review Analysis

### Review Length vs. Rating

![Review Length Rating Correlation](screenshots/review_length_rating.png)

A clear trend emerges: negative reviews tend to be significantly longer than positive ones. Users writing 1-2 star reviews feel compelled to explain their dissatisfaction in detail, while satisfied customers keep their praise concise.

### Monthly Vote Trends

![Vote Trends](screenshots/vote_trends.png)

The analysis of "useful," "funny," and "cool" votes shows:
- "Useful" votes consistently outpace other categories
- All vote types show similar seasonal patterns
- Peak voting activity occurred in 2016-2017
- Steady growth over time with occasional spikes

## 🗺️ Geographical Insights

### Global Distribution

![Global Map](screenshots/global_map.png)

Yelp businesses are heavily concentrated in North America, with notable presence in Europe and scattered coverage elsewhere.

### Regional Focus

![North America](screenshots/north_america.png)
![Europe](screenshots/europe.png)

The density maps reveal concentrated business clusters in major urban areas.

### City-Level Analysis

![Las Vegas & Phoenix](screenshots/las_vegas_phoenix.png)
![Stuttgart & Edinburgh](screenshots/stuttgart_edinburgh.png)

The comparison between U.S. and European cities reveals fascinating urban planning differences:
- Las Vegas and Phoenix show clear grid patterns reflecting planned urban development
- Stuttgart and Edinburgh display organic, irregular distributions reflecting centuries of historical growth

## ⏰ Check-in Patterns

![Check-in Variations](screenshots/checkin_variations.png)

Check-in data reveals predictable patterns:
- Weekends show significantly higher activity
- Peak hours occur between 5-7 PM across all days
- The lowest activity occurs between 2-6 AM
- Each day follows a similar curve with weekend amplification

These patterns provide valuable insights for business scheduling and promotional timing.

## 👤 User Behavior Analysis

### User Engagement Distribution

![User Review Distribution](screenshots/user_review_distribution.png)

User engagement follows a classic power law distribution:
- ~70% of users write only 1-2 reviews
- A small minority of power users contribute disproportionately
- The top reviewer wrote 3,569 reviews, while the median user writes just 1

This insight helps understand platform dynamics and identify influential users.

## 🍽️ Business Case Study

### Top 5-Star Businesses

![Top 5-Star Businesses](screenshots/top_5star.png)

"Gen Korean BBQ House" leads with 871 five-star reviews, followed by "Bacchanal Buffet" (547) and "Earl of Sandwich" (545).

### Word Cloud Analysis

![Gen Korean BBQ House Word Cloud](screenshots/word_cloud.png)

Most frequent terms in reviews for the top business:
- food (670 occurrences)
- great (623)
- service (550)
- place (549)
- korean (446)

## 💭 Sentiment Analysis

### Positive vs. Negative Words

![Positive Words](screenshots/positive_words.png)
![Negative Words](screenshots/negative_words.png)

Sentiment analysis reveals:
- Positive reviews emphasize words like "good," "great," "best," "love"
- Negative reviews focus on "bad," "problem," "terrible," "worst"
- Emotional intensity is stronger in negative reviews

## 💻 Technology Stack

- **Python**: Core programming language
- **Pandas & NumPy**: Data manipulation
- **Matplotlib & Seaborn**: Static visualizations
- **Folium**: Interactive maps
- **NLTK & TextBlob**: Text processing and sentiment analysis
- **WordCloud**: Text visualization

## 🚀 Setup and Installation

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/yelp-dataset-analysis.git
   ```

2. Install required packages:
   ```
   pip install -r requirements.txt
   ```

3. Download the Yelp dataset and place files in the `/data` directory

4. Run the Jupyter notebook:
   ```
   jupyter notebook Yelp_View.ipynb
   ```

## 🔮 Future Work

- Develop predictive models for business success based on location and category
- Create a recommendation system using review content and user preferences
- Analyze temporal trends in business openings/closings by category
- Expand sentiment analysis to detect specific aspects (food quality, service, price)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Yelp for providing the dataset
- Contributors to the Python data science ecosystem

---

*Created by [Hang Wang]
