README:

Please read me for all the important information about this repository.

This code examines and analyzes data on if drivers will accept a coupon.


In this Jupityer notebook we are examining data about the use of coupons by drivers.  The dataset contains information ranging from the age,income, employment, and marital status to how often the driver frequents different types of establishments and how far away a coupon establishment is from the driver currently.  With this information we are trying to determine if the driver will accept and use a certain type of coupon.

Once the dataset was loaded did a preliminary examination to see if any correlations stood out, examine if there were any columns with missing values that needed to be addressed, and anything else about the data that stood out.  The findings were that no numerical data appeared to have any strong correlations, there were a few columns with missing data that needed to be addressed, and a few other notables.  The other notables included combining the direction data into one column and creating a new column to clearly state if the drivers accepted the coupon.

Addressing the missing data was a bit more complex.  The car column had so much missing data it was simply dropped.  The Bar data was examined to see what was the most common value and it was noted that a large majority never went to bar or went less than once.  The decision was made to fill the values with less than 1.
The Coffeehouse data was more uniformally distributed thus the decision was made to fill the missing data with the most common value, also 'less1'. The other data was currently left as null until if/when it would be explored further.

The analysis of the data then began.  We began by simply looking at the total number of drivers that accepted the coupon and found 57% of drivers accepted the coupon they were given. We then took a look at what the acceptance was based on the coupon provided.  We saw that cheaper restaurants and carry out/take away had the highest accpetance rate while Bars and expensive restaurants had the lowest rates.  This would seem to make logical sense as most drivers and people overall are apt to visit cheaper restaurants and/or carry out meals, while fewer people overall are likely to go to bars and/or visit expensive restaurants.

In the next section we took a more in depth look at the Bar coupon data. We began by creating a new dataframe that only included the data about drivers given the Bar coupons. Overall we saw that only 41% of drivers accepted the bar coupons. We then took a look at who accepted Bar coupons by age group and saw that in general it was drivers between the ages of 21 and 30 that were most likely to accept the coupons.  We then took a look at who accepted the coupons based on how often they frequented bars; not surprisingly those drivers that frequented bars were more likely to accept coupons while drivers that didn't frequent bars often were not likely to accept coupons.  The most important finding was that 76% of coupons were accepted by drivers that frequent bar 4 or more times vs. only 37% by those that visit bars 3 or fewer times.

We then examined some more data related bar coupons and continued to find, unsurprisingly, frequent bar visitors,  drivers without passengers that were a kid, and drivers between the ages of 21 and 30 were most likely to accept coupons.

At this point we began to examine other data of interest. Some questions arose that would be interesting to examine. These include:

Does having children effect the acceptance of coupons?
Ultimately we see that having children does effect the acceptance rate, albeit slightly. Would be interesting to see if it is statistically signifcant.

Does it matter how far away the coupon is?  Does direction matter?
The distance away for the coupon is signifcant.  The closer the coupon is located the more likely the driver is to accept the coupon. It does not appear the direction the driver is going has a great effect.

Does gender matter for any type of coupon?






