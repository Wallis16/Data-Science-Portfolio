## Data Analysis Project

<img src="https://github.com/Wallis16/Data-Science-Portfolio/blob/main/Books%20%26%20Wings/Figures/books.jpg" width="400">

#### A famous investment group decided to open an e-commerce company (**Books & Wings**) aiming to sell books, and they ask us for recommending books with sale potential. The goal of this project is to collect and analyze data about bestseller books from big companies such as Amazon, eBay, and Barnes&Noble. We intend to use this data to get insights into what would be more relevant for our client.

![alt text](https://github.com/Wallis16/Data-Science-Portfolio/blob/main/Books%20%26%20Wings/Figures/presentation_image.jpg)

#### This data analysis follows the six phases shown in the Google Data Analytics course: [ask, prepare, process, analyze, share, and act.](https://medium.com/codex/6-phases-of-data-analysis-according-to-google-9e084b89f848) The ask phase helped to figure out what data would be interesting for a company that wishes to sell books and is looking for recommendations based on data-driven solutions. Prepare data was the data collecting using web scraping. In the process phase, we cleaned the data. Analyse is our data analysis, which is available on a jupyter notebook and in a notebook on Kaggle. The sharing step is our insights available in the data analysis notebook. Act phase would be for a company buys books based on our recommendations, such as buying books by Colleen Hoover, the top author in our bestseller data.

## Data analysis
You can check the [data](https://github.com/Wallis16/Web-Scraping-and-EDA-Bookstore/tree/main/Books%20%26%20Wings/Data), [analysis](https://github.com/Wallis16/Web-Scraping-and-EDA-Bookstore/tree/main/Books%20%26%20Wings/Data%20Analysis), and [web scraping](https://github.com/Wallis16/Web-Scraping-and-EDA-Bookstore/tree/main/Books%20%26%20Wings/Web%20Scraping) on [Books and Wings](https://github.com/Wallis16/Web-Scraping-and-EDA-Bookstore/tree/main/Books%20%26%20Wings).

### Following we have some details about how we made the web scraping. 

## Web Scraping
Step by step of how to make web scraping using python. In this example, we made the web scraping on the eBay site.

First, we need to know what we wish to collect. In our case, features such as title, price, and the number of ratings are considered relevant. Therefore, we select this part on the site and click on inspection.

![alt text](https://github.com/Wallis16/Data-Science-Portfolio/blob/main/Books%20%26%20Wings/Figures/web_scraping_step_by_step_1.png)

After that, you will see an HTML highlighted code related to that part of the site. We are looking for an id that contains all the books. So, we search by <div id=”<>”>, in our case id=”top-products-container-wrapper”.

![alt text](https://github.com/Wallis16/Data-Science-Portfolio/blob/main/Books%20%26%20Wings/Figures/web_scraping_step_by_step_2.png)

![alt text](https://github.com/Wallis16/Data-Science-Portfolio/blob/main/Books%20%26%20Wings/Figures/web_scraping_step_by_step_3.png)

Now that we have the id, let’s look for classes containing the data we are interested in. Starting with the title, we have the class “title”.

![alt text](https://github.com/Wallis16/Data-Science-Portfolio/blob/main/Books%20%26%20Wings/Figures/web_scraping_step_by_step_4.png)

We make the same with the other data, to get the reviews, we use the class “reviews-aggregated-stars”.

![alt text](https://github.com/Wallis16/Data-Science-Portfolio/blob/main/Books%20%26%20Wings/Figures/web_scraping_step_by_step_5.png)

Getting the price we need the class “trending-price”.

![alt text](https://github.com/Wallis16/Data-Science-Portfolio/blob/main/Books%20%26%20Wings/Figures/web_scraping_step_by_step_6.png)

More details are available on the code. Note that HTML code from the sites can change, so be aware of this when you will perform your web scraping.
