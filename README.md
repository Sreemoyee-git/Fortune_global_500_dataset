# Fortune_global_500_dataset

Problem Statement

The goal of this project was to extract and clean data from Wikipedia containing the Fortune Global 500 companies for 2023, and then save it as a structured dataset suitable for analysis and machine learning applications. The challenge was to accurately scrape the HTML tables, identify the relevant one among multiple tables, clean column names, and prepare a dataset with standardized fields like Industry, Company, Country, Rank, and Revenue.

What I Did

1. Data Extraction:

Used the Wikipedia URL for Fortune Global 500 companies and read all tables using pandas.read_html().

Enumerated each table to identify the correct one containing the required data structure.

2. Data Cleaning and Transformation:

Selected the correct table, renamed and standardized column names (converted to lowercase, replaced spaces with underscores, and removed special characters).
Dropped empty rows and reset the index for a clean dataset.
Verified column data types and removed null values using df.dropna() to ensure accuracy.

3. Data Exporting and Uploading:

Saved the cleaned dataset as a CSV file (fortune_global_500_2023.csv).

Uploaded it to Kaggle’s working directory for public access and further use in analytics or visualization projects.
Here's the Dataset link -

https://www.kaggle.com/datasets/sreemoyeesengupta/fortune-global-500-companies-2023-list

4. Validation:

Re-read the file using pd.read_csv() to ensure successful storage and correctness of data formatting.

Tools Used

Python (Pandas, Requests, OS): For web scraping, data cleaning, and file handling.

Jupyter Notebook / Kaggle Notebook: For running, testing, and saving code outputs.

Wikipedia (Data Source): For obtaining the Fortune Global 500 dataset in HTML format.

Recommendations

1. Automate Updates: Schedule the scraper to run annually or quarterly to fetch updated Fortune 500 lists automatically.

2. Data Enrichment: Enhance the dataset by adding additional metrics like market capitalization, number of employees, or stock price trends.

3. Visualization: Use Power BI or Tableau to visualize company rankings, industry dominance, and regional performance for better insights.

4. API Integration: Instead of web scraping, consider using structured data APIs for more reliable updates and faster extraction.

Conclusion

This project provided hands-on experience with web scraping, data wrangling, and dataset publishing. It demonstrated how unstructured web data can be transformed into clean, usable information for analytics. Through this process, I learned how to handle multiple tables, clean column structures efficiently, and verify dataset integrity before sharing. The final dataset serves as a valuable resource for studying global industry trends, corporate performance, and economic patterns across countries.
