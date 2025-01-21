# Real Estate Data Scraper, Cleaner, and Analyzer

This project provides a comprehensive pipeline for scraping, cleaning, preprocessing, and analyzing real estate data from Armenian websites. It automates the process of collecting real estate information and visualizing meaningful insights from the data.

---

## Features

1. **Web Scraping**:
   - Scrapes real estate data from websites like [senyak.am](https://www.senyak.am/) and [banali.am](https://banali.am/).
   - Extracts information such as region, building type, number of rooms, area, floor, repair status, and price.

2. **Data Cleaning**:
   - Removes duplicates from datasets.
   - Cleans and standardizes fields like area and price.
   - Combines multiple CSV files into a single cleaned dataset.

3. **Data Preprocessing**:
   - Encodes categorical features using Label Encoding.
   - Standardizes and normalizes numerical features for better analysis.

4. **Exploratory Data Analysis (EDA)**:
   - Visualizes distributions of key features (e.g., area, rooms, price).
   - Generates correlation heatmaps.
   - Creates bar plots and pie charts to compare and analyze data.

---

## Installation

1. **Clone the Repository**:
   ```bash
   git clone <repository_url>
   cd <repository_name>
   ```

2. **Install Dependencies**:
   - Make sure you have Python installed.
   - Install the required Python libraries:
     ```bash
     pip install selenium scikit-learn pandas matplotlib seaborn numpy
     ```

3. **Setup WebDriver**:
   - Download the Chrome WebDriver compatible with your Chrome browser version from [here](https://googlechromelabs.github.io/chrome-for-testing/)
   - Place the WebDriver executable in your system PATH or the project folder.

---

## Usage

### 1. Web Scraping
- Modify the `value` variable to set the exchange rate for price conversion.
- Run the script to scrape data from the supported websites:
  ```bash
  python scraper.py
  ```
- Scraped data will be saved in CSV files.

### 2. Data Cleaning
- Combine multiple scraped datasets using the script.
- Clean duplicates and save the cleaned dataset as `Cleaned_result.csv`.

### 3. Data Preprocessing
- Encode categorical features using LabelEncoder.
- Standardize and normalize numerical data.
- Preprocessed data is visualized for verification.

### 4. Data Analysis
- Use the EDA section of the script to generate visualizations:
  - Histograms of area, rooms, and building types.
  - Correlation heatmaps.
  - Bar plots comparing different features.
  - Pie charts showing property distribution by region and price range.

---

## Visualizations

### Example Plots

1. **Price Distribution by Region**
   ![output](https://github.com/user-attachments/assets/3126b0d4-d21a-46d3-9b94-3a3e8790a081)

2. **Correlation Heatmap**
   ![output](https://github.com/user-attachments/assets/2d7f3be0-428a-4dbb-974c-7e06069c44ad)

3. **Bar Plot of Area vs. Rooms**
   ![output](https://github.com/user-attachments/assets/2493b7d4-f8ec-495a-8b24-b682ef58927f)

---

## Requirements

- Python 3.7+
- Google Chrome Browser
- Chrome WebDriver

### Python Libraries:
- selenium
- scikit-learn
- pandas
- matplotlib
- seaborn
- numpy

---

## Challenges and Notes

- Some data fields on the websites may vary in structure; the scraping logic includes handling exceptions.
- Ensure that web scraping respects the website’s terms of service.
- For large-scale scraping, adjust delays to prevent being blocked.

---

## Future Improvements

- Add support for additional real estate websites.
- Enhance data visualization with interactive plots using libraries like Plotly or Dash.
- Implement machine learning models for price prediction or property classification.

---

