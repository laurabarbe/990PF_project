##990PF_project
##project for Metis Intro to Data Science spring 2016

* What is the question you hope to answer? 
Private operating foundations are required to distribute a minimum amount (based on their investment returns) for charitable purposes each year. I am interested in seeing how far above the minimum distrbution is typical, and whether this amount is correlated with anything else.

* What data are you planning to use to answer that question? 
The IRS has made available extracts of selected financial data filed by tax-exempt organizations in the years 2012, 2013, 2014, and 2015. I will be looking specifically at the extracts of Form 990-PF, which is filed by private foundations, for fiscal years 2012 and 2013 (forms that were filed in 2014).

* What do you know about the data you're using so far? 
The data contains approximately 100,000 samples and 187 features. Several of the features are variations of one another (for instance, subtotals that make up a total), so some feature engineering will be required before any analysis can be performed.

* Why did you choose this topic? 
I work in fundraising for a large non-profit and am interested in better understanding the private grant-making world.


* What data have you gathered, and how did you gather it?
I used the 2014 extract of form 990-PF prepared by the IRS.
	
* How have you explored the data and what insights have you gained as a result?
There is a huge variation in giving levels among foundations. Among the higher-end organizations, the IRS-determined required distribution has basically no effect on how much they give - their philanthropy is completely professionalized.
	
* Will you be able to answer your question with this data, or do you need to gather more data (or adjust your question)?
I suspect that there are a lot of additional factors influcing giving that are not representated in this data set. These could include the number of people on the foundation's board, their relationships with each other, their relationships with the other organizations they support, or the time of year in which distributions are made. The IRS does not provide this data, so someone would have to scrape it from the actual tax returns.
	
* What modeling approach are you using to answer your question?
This data set has a lot of features that are simply variations of each other, so my original plan was to run two analyses: one using only the aggregate features, and one using the sub-totals. In both cases, I ended up having way too many features to handle. Ultimately, I decied to look only at the features relating to foundation revenue (donation income, interest income, dividends, rents, etc.) using a random forests approach.
