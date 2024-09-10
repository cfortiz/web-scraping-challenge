# Module 11 Challenge - Web Scraping and Data Analysis

Web scraping, data analysis, and visualization with selenium/splinter,
BeautifulSoup, Pandas, and Matplotlib of HTML web content relating to news
about Mars and Martian weather.

## Files

* `part_1_mars_news.ipynb`: Jupyter notebook with code to scrape titles and
  preview text of news articles about Mars.
* `part_2_mars_weather.ipynb`: Jupyter notebook with code to scrape and analyze
  Mars weather data.
* `mars_weather.csv`: CSV file exported via Pandas of the Mars weather data
  scraped from the web.
* `README.md`: This file.
* `.gitignore`: Standard python .gitignore generated via github.

## Challenge

### Part 1

Use `splinter` / `selenium` to scrape the titles and preview text of news
articles about Mars from a website.  Uses browser automation to fetch the HTML
from the provided URL, parses the HTML using `BeautifulSoup`, then navigates and
queries the parsed HTML to obtain a list of dictionaries containing the title
and preview for each article in the page.

### Part 2

Use `splinter` / `selenium` to scrape Mars weather data by fetching, parsing,
and then transforming the HTML from the provided URL into a Pandas `DataFrame`
which will be used to analyze, visualize, and export the data.

#### Metadata

Mars weather metadata per [The Pudding](https://data.world/the-pudding/mars-weather):

**Note**: This table has been edited for brevity, and to limit the scope to the
fields / columns in the URL provided for the challenge.

| Header           | Description                                                                        | Data Type |
| ---------------- | ---------------------------------------------------------------------------------- | --------- |
| id               | The identification number of a single transmission.                                | number    |
| terrestrial_date | The date on Earth (formatted as yyyy-mm-dd).                                       | date      |
| sol              | The number of elapsed sols (Martian days) since Curiosity landed on Mars.          | number    |
| ls               | The solar longitude or the Mars-Sun angle, measured from the Northern Hemisphere.  | number    |
| month            | The Martian Month. Similarly to Earth, Martian time can be divided into 12 months. | text      |
| min_temp         | The minimum temperature (in °C) observed during a single Martian sol.              | number    |
| pressure         | The atmospheric pressure (Pa) in Curiosity's location on Mars.                     | number    |
