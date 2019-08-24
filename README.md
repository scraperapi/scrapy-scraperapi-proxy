Scraper API middleware for Scrapy (http://scrapy.org/)
=======================================================

Processes Scrapy requests using the Scraper API service https://www.scraperapi.com.


Install
--------

Checkout the source and run

    python setup.py install


settings.py
-----------

    # Activate the middleware
    SCRAPERAPI_ENABLED = True
    # Address of the API service
    SCRAPERAPI_URL='api.scraperapi.com'
    #The API key 
    SCRAPERAPI_KEY='your API key'

    DOWNLOADER_MIDDLEWARES = {
        'scrapy_scraperapi.ScraperApiProxy': 610,
    }


