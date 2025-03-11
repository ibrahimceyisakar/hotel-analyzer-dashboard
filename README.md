# Hotel Finder Dashboard

A Streamlit-based interactive dashboard for analyzing and visualizing hotel data in Istanbul, Turkey. This dashboard is part of the [Hotel Finder](https://github.com/ibrahimceyisakar/hotel-finder/) project, which scrapes hotel data from obilet.com, analyzes it for value metrics, and visualizes the results. 

## Features

The dashboard provides comprehensive analysis of over 3,000 hotels in Istanbul with their daily prices, review scores, and features. It includes:

- **Value Overview**: Bar charts and scatter plots showing hotels ranked by value ratio (review score/price)
- **Price Analysis**: Histograms and box plots of hotel prices, including distribution by star rating
- **Review Analysis**: Distribution and comparison of review scores across different hotels
- **Feature Analysis**: Most common hotel features and their impact on review scores
- **Location Analysis**: Geographical distribution of hotels and distance-to-center analysis

## Dashboard Tabs

The interactive dashboard is organized into five main tabs:

1. **Value Overview**: Displays hotels sorted by value ratio with interactive visualizations
2. **Price Analysis**: Provides detailed price distribution and comparisons
3. **Review Analysis**: Shows review score distributions and correlations
4. **Feature Analysis**: Analyzes hotel amenities and their impact on ratings
5. **Location Analysis**: Visualizes hotel locations and distance metrics

## How It Works

This dashboard is the visualization component of a three-part hotel data pipeline:

1. **Data Collection**: The [hotel-finder](https://github.com/ibrahimceyisakar/hotel-finder/) project scrapes hotel data using Selenium
2. **Data Analysis**: The scraped data is processed to calculate value ratios and identify top-value hotels
3. **Data Visualization**: This Streamlit dashboard loads the analyzed data and presents it through interactive charts

## Installation

```bash
# Clone the repository
git clone https://github.com/ibrahimceyisakar/hotel-analyzer-dashboard.git
cd hotel-analyzer-dashboard

# Install dependencies
pip install -r requirements.txt

# Run the dashboard
streamlit run hotel_dashboard.py
```

## Requirements

The dashboard requires the following Python packages:
- streamlit
- pandas
- numpy
- plotly
- and other dependencies listed in requirements.txt

## Data Source

The dashboard uses data scraped from obilet.com, which is processed and stored in JSON and CSV formats. The data includes hotel names, prices, review scores, star ratings, locations, features, and calculated value ratios.

## Related Project

This dashboard is part of the [Hotel Finder](https://github.com/ibrahimceyisakar/hotel-finder/) project, which provides the complete hotel data collection, analysis, and visualization pipeline.
