# Analyzing 2016-2017 NYC Real Estate Sales
This is my final project for my CIS 9650 Programming for Data Analytics graduate course. I analyzed 2016-2017 real estate sales across NYC found on Kaggle and used Python to explore the most popular borough and property types for sale.

# Borough/Neighborhood Exploration

![boroughs](https://github.com/sallywuhoo/CIS9650-NYC2017-RE-Sales/assets/148400043/25273595-afe7-4240-962e-3bed7b6a79f3)

Of the 5 boroughs, Queens and Brooklyn see the most action in terms of real estate transactions. Looking deeper, in the 2016-2017 timeframe, Queens ranked #1 with 84,548 transactions. Additionally, research showed that Queens and Brooklyn sold more homes than Manhattan (and other boroughs) in the 2010-2020 timeframe (PropertyClub Team, "The 50 Best-Selling NYC Neighborhoods from 2010 to 2020"). The top 3 neighborhoods with the most sales 2010-200 PropertyClub reported are Flushing-North (Queens), Bedford Stuyvesant (Brooklyn), and Ozone Park (Queens); in fact, of the 50 neighborhoods listed, 22 are within Queens. Upon further analysis into the 2016-2017 dataset I was working with, the neighborhoods that saw the most transactions were Flushing Meadow Park, Flushing-South, Howard Beach, Astoria and Bayside, all located in Queens Borough.

![boroklyn_queens_neighborhoods](https://github.com/sallywuhoo/CIS9650-NYC2017-RE-Sales/assets/148400043/ff4f9e8d-bc38-42b4-ba0b-8b6d01798383)

# Property Type Exploration
In this data, there are 47 unique dwelling types listed ranging from single-family units to commercial real estate buildings. Of all these property types, in 2016-2017, the top seller were one-family dwellings with 18,235 transactions. This initially was surprising because according to the article "Report: Only 17% of NYC Homes are Single-Family" by Mike Lafirenza at Cooperatornews, this rate of 17% is the smallest share among all large US cities. However, this makes sense because most people when looking to buy are most interested in (and most financially able to afford) single-family homes as opposed to the larger corporations that purchase multifamily buildings for investments.

![building type](https://github.com/sallywuhoo/CIS9650-NYC2017-RE-Sales/assets/148400043/8c141b44-b3f7-4b93-90c8-1be8eb3127e3)

# Year Built Exploration
The average age of properties sold in 2016-2017 were built in 1950 and majority were built some time between 1925-1970. This isn't surprising as most properties in NYC are older and according to Renthop, "the median age of a surviving residential building is nearly 90 years old" since the city saw massive growth between 1900-1920 which led to a spike in residential construction. Something interesting I learned here is that some of the oldest neighborhoods with buildings dating far back are Bowery, Soho, Greenwich Village and East Village all located in Manhattan.

![year built](https://github.com/sallywuhoo/CIS9650-NYC2017-RE-Sales/assets/148400043/942ad68b-e03b-4725-a6dd-ebf7044ab9ba)

# Correlation between # of Units and Sales Price
Using the regression plot functionality in Seaborn, I plotted the correlation between the number of units and the sales price of each property. Unsurprisingly, there's a clear positive correlation between the two factors; as a property contained more units, the sales price was higher. In a city like NYC, the most units a property has, the more cashflow the owner is able to generate thus leading to lower cap rates and higher valuations. Although, looking at the graph, it appears there are a couple of outliers, but this could be due to other factors such as the unit mix and presence of commercial units in mixed-use buildings. It would be interesting to further break out the types of units within a property and apply the correlation again.

![units_vs_price](https://github.com/sallywuhoo/CIS9650-NYC2017-RE-Sales/assets/148400043/305090ba-18bc-419b-9d43-bf74cc9e5bcb)

# Seasonality
A last analysis I performed is looking at sales trends throughout the 2016-2017 year to identify whether there was a pattern. Prior to plotting this line graph, I hypothesized a higher number of sales in the warmer months and a decrease in the winter, however, there doesn't appear to be any significant trends. Although, it's important to note this analysis only looks at a small snippet of real estate transactions from 2016-2017 as opposed to analyzing seasonality across multiple years; it would be best to extend the timeframe and perhaps look at trends throughout the decades. From further research, in the article "When Is the Best Time to List Your NYC Property?" by Forbes, it appears that most deals occur from March to June. Although, there is a caveat that certain sub-neighborhoods could see different seasonal trends. It would be interesting to look further into this and analyze the trends by neighborhoods as well as the types of property within those neighborhoods.

![daily sales](https://github.com/sallywuhoo/CIS9650-NYC2017-RE-Sales/assets/148400043/7e6e4532-3a47-4c8f-aac5-0ca76e5106b5)
