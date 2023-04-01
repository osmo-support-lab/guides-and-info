# Building and running database queries

Even with block explorers and community or validator built information hubs, some pieces of info can still be very difficult to find. Thanks to [Flipside](https://flipsidecrypto.xyz/), there is a free-to-use database built for this, and much more. Data experts and clever amateurs use this to uncover interesting data or correlations that would otherwise be buried in the blockchain.<br>

![](https://github.com/osmo-support-lab/guides-and-info/blob/main/guide-images/flipside/1.png?raw=true "Community dashboards")

Full [documentation](https://docs.flipsidecrypto.com/) here.

<br>

### Getting started, basic queries are very simple. After some trial and error you'll be building more complex searches and filters in no time.

#### First off, expand the left side panel and click 'Create New' to start building your first query.

![](https://github.com/osmo-support-lab/guides-and-info/blob/main/guide-images/flipside/2a.png?raw=true)
<br>

#### After this, if you go to 'Explore Data' and choose Osmosis, you will see a long list of all the possible parameters you can query against. 
*If you click each one you will see some further options and information.*

![](https://github.com/osmo-support-lab/guides-and-info/blob/main/guide-images/flipside/3a.png?raw=true)

<br>

#### This extra info in the lower panel is the actual data points you can query. You can combine several for a powerful search, and go even further by excluding others, using "and/or" statements, etc.


**The syntax is important. The form will try to assist you by completing each term. If something isn't working or it won't accept a value you've entered, try enclosing it in single quotes.** [ ' ' ]

*Here's an example to get you started. This will return 'all' (*) entries from 'fact_daily_balances' where the address and date both match these values exactly.*
```
SELECT
*
FROM
osmosis.core.fact_daily_balances
WHERE
ADDRESS = 'osmo1wev8ptzj27aueu04wgvvl4gvurax6rj5p5lw4u'
AND
DATE = '2022-07-30'
```

![](https://github.com/osmo-support-lab/guides-and-info/blob/main/guide-images/flipside/4a.png?raw=true)

<br>

### After your query is completed, hit the blue 'play' button at the top right and wait for it to process. 
*(More complex queries may take some time!)*

![](https://github.com/osmo-support-lab/guides-and-info/blob/main/guide-images/flipside/5a.png?raw=true)

<br>

### To make a second query, or to tweak your first one, you can either start a new one, simply change the first one, or you can use the 'fork' option to make a copy of that one without destroying the previous one.

![](https://github.com/osmo-support-lab/guides-and-info/blob/main/guide-images/flipside/6a.png?raw=true)

<br>

### Remember all those other links on the homepage? Those are other dashboards made by other community members. If you want, you can open those up and dig into the guts to learn more about what can be done here and how to do it. 
*Don't forget to share any cool info you put together with the community!*
![](https://github.com/osmo-support-lab/guides-and-info/blob/main/guide-images/flipside/7a.png?raw=true)
