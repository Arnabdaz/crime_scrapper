# Crime Data Scraper

This Python script scrapes crime data from NDTV news articles for a given location and saves the data into a CSV file. The script uses the `requests` library to fetch the web content and `BeautifulSoup` to parse the HTML content. Additionally, it categorizes each crime based on keywords found in the title and description.

## Dependencies

- Python 3
- `requests`
- `beautifulsoup4`

You can install the required dependencies by running the following command:

```bash
pip install requests beautifulsoup4
```
## How to Use

1. Run the Python script `crime_data_scraper.py`.
2. Enter the location and state when prompted.
3. The script will scrape the crime data for the given location and save it to a CSV file.

The CSV file will be named as `<location>_crime_data.csv`, and the columns include location, time, crime type, description, state, and month.

## Example Usage

```bash
python crime_data_scraper.py
```

### Input:

```bash
Enter the location: delhi
Enter the state: delhi
```

### Output:

```
Crime data has been saved to delhi_crime_data.csv.
```

This will generate a `delhi_crime_data.csv` file containing the scraped crime data.

## Known Limitations

1. The script currently relies on specific keywords to categorize crime types, which may lead to inaccuracies or misclassifications.
2. The script only scrapes crime news from the NDTV website, which may not cover all crime incidents in a location.
3. The script may have difficulty handling non-English crime news or special characters.

## Future Improvements

1. Improve the categorization method by using machine learning techniques, such as natural language processing, to better understand the context of the news article.
2. Expand the list of sources to scrape from, to gather a more comprehensive set of crime data.
3. Add support for non-English news and handle special characters properly.
4. Include additional metadata in the output, such as the URL of the news article, to provide more context.
