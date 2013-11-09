# Other APIs

Here is a collection of APIs we've gathered for quick access during the Hackathon.

* Financial
    * [dev.markitondemand.com](http://dev.markitondemand.com)
        * [Company Lookup](http://dev.markitondemand.com/#companylookup)
        * [Quote](http://dev.markitondemand.com/#stockquote)
        * [CDS](http://dev.markitondemand.com/#cdsmovers)
        * [Interactive Chart](http://dev.markitondemand.com/#interactive)
    * Yahoo!
        * [Yahoo! YQL](http://developer.yahoo.com/yql/console/) (choose 'Show Community Tables' on right, filter by 'finance')
        * [Stock Info](http://developer.yahoo.com/yql/console/?q=select%20*%20from%20yahoo.finance.stocks%20where%20symbol%3D%22GOOG%22&env=store%3A%2F%2Fdatatables.org%2Falltableswithkeys)
        * [Sectors](http://developer.yahoo.com/yql/console/?q=select%20*%20from%20yahoo.finance.sectors&env=store%3A%2F%2Fdatatables.org%2Falltableswithkeys )
        * [Industry](http://developer.yahoo.com/yql/console/?q=select%20*%20from%20yahoo.finance.industry%20where%20id%3D%22112%22&env=store%3A%2F%2Fdatatables.org%2Falltableswithkeys)
        * [Options](http://developer.yahoo.com/yql/console/?q=SELECT%20*%20FROM%20yahoo.finance.options%20WHERE%20symbol%3D'GOOG'%20AND%20expiration%3D'2010-06'&env=store%3A%2F%2Fdatatables.org%2Falltableswithkeys)
        * [Historical Data](http://developer.yahoo.com/yql/console/?q=select%20*%20from%20yahoo.finance.historicaldata%20where%20symbol%20%3D%20%22YHOO%22%20and%20startDate%20%3D%20%222009-09-11%22%20and%20endDate%20%3D%20%222010-03-10%22&env=store%3A%2F%2Fdatatables.org%2Falltableswithkeys)
        * [Quant](http://developer.yahoo.com/yql/console/?q=select%20*%20from%20yahoo.finance.quant%20where%20symbol%20in%20%22YHOO%22&env=store%3A%2F%2Fdatatables.org%2Falltableswithkeys)
* Weather
    * [Forecast.io](http://forecast.io/)
* Maps
    * [Bing Maps](http://www.bingmapsportal.com/) - Requires API key/registration
* Music
    * [iTunes](http://itunes.apple.com/search?explicit=No&term=rock) - Modify the "term" value
    * [Last.fm](http://www.last.fm/api) - Requires API key/registration
    * [MTV Services](http://api.mtvnservices.com/docs/)
* News
    * [Yahoo! News RSS feeds](http://news.yahoo.com/sitemap/)
    * [Google News RSS](https://news.google.com/news/feeds?q=apple&output=rss)
    * [WSJ.com RSS](http://online.wsj.com/public/page/0_0813.html)
    * [MarketWatch RSS](http://www.marketwatch.com/rss/)
    * [CNBC RSS](http://www.cnbc.com/id/28295763)
* Research
    * [Morningstar RSS](http://news.morningstar.com/rss/rss.html)
    * [Markit RSS](http://www.markit.com/en/about/rss/rss-homepage.page)
* Search
    * [Bing Search](https://datamarket.azure.com/dataset/5BA839F1-12CE-4CCE-BF57-A49D98D29A44) - Requires API key/registration
* Sports
    * [ESPN](http://developer.espn.com/docs) - Lots of different APIs, Most require API key/registration
* Social
    * [StockTwits](http://stocktwits.com/developers/docs) or [StockTwits JSON API](https://api.stocktwits.com/api/2/streams/symbol/GOOG.json)
* Travel
    * [Kayak RSS (Air, Airport to Airport, Hotel, etc.)](http://www.kayak.com/labs/rss/)
    * [Lodgix Vacation Rentals](http://www.lodgix.com/vacation-rental-api.html) - Requires API key/registration
    * [Hotwire (Hotel, Rental Cars, etc.)](http://developer.hotwire.com/docs)
* Video
    * [CNBC Video RSS](http://www.cnbc.com/id/15839263/device/rss/rss.xml)
    * [Open Movie Database](http://www.omdbapi.com/)



## Using RSS Feeds in JavaScript Apps

Look at the [Google Feed API](https://developers.google.com/feed/v1/) which allows developers to request a JSON or JSONP dataset via the Feed API.

Example:

`https://ajax.googleapis.com/ajax/services/feed/load?v=1.0&q=http://www.digg.com/rss/index.xml`

Example using JSONP:

`https://ajax.googleapis.com/ajax/services/feed/load?v=1.0&q=http://www.digg.com/rss/index.xml&callback=yourCallbackFunc`

Checkout the [JSON Dev Guide](https://developers.google.com/feed/v1/jsondevguide) for specifics.