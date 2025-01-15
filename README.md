# Analyze how educational videos differ in popularity from entertainment videos.

This project analyzes the popularity differences between educational and entertainment videos. It is part of the Data Engineering course project. The work begins by collecting data for analysis from two sources: YouTube API and Kaggle Dataset. The data is stored in MongoDB to gradually collect more than 5000 records from the YouTube API. Once the data is complete, it is transformed and cleaned before plotting graphs to observe trends and differences to summarize the analysis results.
## Presentation
For more detailed information, please refer to the [Presentation.pdf](./Presentation.pdf)

## Summary of Findings

1. **Midday** is the time when the most videos are uploaded.
2. **Entertainment videos** are significantly more popular than educational videos in terms of views, likes, and comments.
3. **Videos uploaded during 2017-2018** received the most comments, even though it was not the year with the highest number of video uploads.
4. **Educational videos** are generally longer than entertainment videos on average.
5. The year **2022** saw the highest number of educational video uploads, but with fewer views than in 2015. In contrast, entertainment videos had the highest number of uploads and views in 2018.

## Tools and Methods Used

This project utilizes several tools and methods to analyze the popularity differences between educational and entertainment videos. Below is a summary of the tools and methods used:

### Data Collection
- **YouTube API**: Used to collect video data from YouTube.
- **Kaggle Dataset**: Additional data source for video information.
- **MongoDB**: A NoSQL database used to store the collected data.

### Data Processing
- **Pandas**: A Python library used for data manipulation and analysis.
- **NumPy**: A library for numerical operations.
- **LangDetect**: A library used to detect the language of text data.
- **ISODate**: A library to parse ISO-8601 duration strings.

### Data Cleaning and Transformation
- **Duplicate Removal**: Functions to check and remove duplicate documents in MongoDB collections.
- **Data Normalization**: Converting JSON data from MongoDB into Pandas DataFrames.
- **Language Detection**: Identifying and filtering data based on language.
- **Duration Conversion**: Converting video duration from ISO-8601 format to minutes.
- **Category Mapping**: Mapping category IDs to category names.

### Data Analysis
- **Grouping and Aggregation**: Grouping data by various attributes (e.g., year, category) and calculating sums and means.
- **Regular Expressions**: Extracting date and time components from timestamps.

### Data Visualization
- **Matplotlib**: A plotting library used to create various types of graphs and charts.
- **Natsort**: A library for natural sorting of data.
