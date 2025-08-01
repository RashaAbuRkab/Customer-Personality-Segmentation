# Customer Personality Segmentation

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Status](https://img.shields.io/badge/Status-Completed-green.svg)

## Table of Contents
- [Overview](#overview)
- [Business Objectives](#business-objectives)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [Installation and Setup](#installation-and-setup)
- [Results and Insights](#results-and-insights)
- [Business Recommendations](#business-recommendations)
- [Contributing](#contributing)
- [Contact](#contact)
- [License](#license)

## Overview
This project leverages **K-Means Clustering** to segment 2240 customers of a retail company based on their demographic and purchasing behaviors. By analyzing attributes like income, spending patterns, and campaign responses, the project provides actionable insights to enhance personalized marketing, improve customer retention, and optimize resource allocation.

## Business Objectives
- Develop targeted marketing campaigns to boost conversion rates.
- Create retention strategies for high-value customers.
- Optimize inventory, pricing, and store layouts based on customer segments.

## Technologies Used
| Category          | Technologies                     |
|-------------------|----------------------------------|
| Programming       | Python                           |
| Data Analysis     | Pandas, NumPy, Scikit-learn      |
| Visualization     | Matplotlib, Seaborn, Yellowbrick |
| Tools             | Jupyter Notebook, Git, GitHub    |

## Project Structure
```
Customer-Personality-Segmentation/
├── Customer_Personality_Segmentation.ipynb  # Main Jupyter Notebook with code
├── Customer_Personality_Segmentation.csv   # Dataset
├── README.md                              # Project documentation
└── requirements.txt                       # Dependencies
```

## Installation and Setup
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/RashaAbuRkab/Customer-Personality-Segmentation.git
   cd Customer-Personality-Segmentation
   ```
2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
3. **Run the Notebook**:
   ```bash
   jupyter notebook Customer_Personality_Segmentation.ipynb
   ```
4. **Dataset**: Place `Customer_Personality_Segmentation.csv` in the project directory.

## Results and Insights
- **Exploratory Data Analysis (EDA)**:
  - Treated 24 missing `Income` values using median imputation (~$51,363).
  - Identified strong correlations between income and spending (e.g., 0.58 for wines and meat).
  - Visualized distributions with histograms, boxplots, and correlation heatmaps.
- **Clustering**:
  - Selected 4 clusters using Elbow Plot and Silhouette Score (k=4, score: 0.240).
  - Cluster profiles:
    | Cluster | Income | Spending (Wines, Meat) | Purchase Frequency | Key Traits |
    |---------|--------|------------------------|--------------------|------------|
    | 0       | ~$35,000 | Low (~$20, ~$15) | Low (~2 web, ~3 store) | Budget-conscious, price-sensitive |
    | 1       | ~$75,000 | High (~$650, ~$450) | High (~5 web, ~8 store) | Affluent, premium shoppers |
    | 2       | ~$55,000 | Moderate (~$450, ~$120) | Moderate (~6 web, ~7 store) | Family-oriented, balanced |
    | 3       | ~$70,000 | High (~$500, ~$400) | High (~6 web, ~8 store) | Store-focused, high-spending |

- **Visualizations**: Boxplots and barplots highlight distinct spending and purchasing behaviors.

## Business Recommendations
- **Cluster 0 (Low-Spending)**: Offer discounts and low-cost loyalty programs to increase engagement.
- **Cluster 1 (High-Spending)**: Promote premium products and VIP memberships for retention.
- **Cluster 2 (Moderate-Spending)**: Target families with bulk discounts and seasonal offers.
- **Cluster 3 (Store-Focused)**: Enhance in-store promotions to leverage store preference.
- **General**:
  - Prioritize marketing budgets for Clusters 1 and 3 for maximum ROI.
  - Stock premium products for Clusters 1 and 3, affordable options for Cluster 0.
  - Refine campaign messaging to focus on exclusivity (Cluster 1), value (Cluster 3), and family benefits (Cluster 2).

## Contributing
Contributions are welcome! Fork the repository, create a branch, and submit a pull request with your changes. Ensure code follows PEP 8 guidelines and includes clear documentation.

## Contact
- **GitHub**: [RashaAbuRkab](https://github.com/RashaAbuRkab)
- **LinkedIn**: [Rasha Abu Rkab](https://www.linkedin.com/in/rashaaburkab)
- **Email**: rashaaburkab@gmail.com

## License
This project is licensed under the [MIT License](LICENSE).
