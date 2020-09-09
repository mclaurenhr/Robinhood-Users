# Robinhood Users Time Series Model

<img src='Cap_Images\roman-synkevych-FI4NKaiTePY-unsplash.jpg'/>

## Introduction 
With the rise of Fintech (Financial Technology), I wanted to further explore and research the Robinhood dataset to determine just how well investors were at investing on their own. Are people as financially savvy as they think they are by abandoning the traditional ways of hiring a Wealth Management firm to manage and handle their investments and self invest? I wanted to dive deeper to see if they were. As an ex financial advisor myself, there was always the challenge of my millennial generation wanting to make their own investment choices and not take the advice from the "experts" so I wanted to see exactly how that has panned out.

When I started my EDA, I started to discover a big shift in the data pre and post COVID-19. There were a lot more investors on the Robinhood platform since quarantine and that triggered me to shift my research on that time period.

I also wanted to create a time series model that forecasted Tesla's stock prices according to my Robinhood dataset. I wanted to use some techniques that I have not used before. I got this time series modeling method from two Udemy time series courses and combined the two modeling techniques. Combining the models was not in my orginial plan but my model was not producing any results when I got to the forecasting section with my first process of choice, so combining the two strategies finally gave me some forecasting results.

# Data Description
<summary style="font-size: 18px"> Data File Used</summary>

* The file was too large to upload so I have included the link to the dataset 
<a href="https://www.kaggle.com/lechterventures/robinhood-user-participation-in-last-year/data">Robinhood Dataset</a>

## Robinhood Closing Stock Price Average (Sept 2019- July 2020)
<img src='Cap_Images\Annotation 2020-09-08 033748.png'/>


# ARIMA Model Results

<details><summary style="font-size: 16px"> Question 1: How much has Robinhood's user base changed since the COVID 19 declaration on March 13, 2020?</summary>

<img src='Cap_Images\Annotation 2020-09-08 033814.png'/>


### Question Details 
I wanted to analysis the average Robinhood Closing Stock Price VS. Active Users post COVID 19, which was officially declared on March 13, 2020. The active users on the Robinhood platform increased by 122% between March 13, 2020 and July 17, 2020

</details>

<details><summary style="font-size: 16px"> Question 2: What are the most popular assets among Robinhood users?</summary>

<img src='Cap_Images\Annotation 2020-09-08 034755.png'/>

### Question Details
I wanted to figure out what assets users invested in the most on the Robinhood platform. After that, I could then compare that to the top performing assets to determine if users were choosing the most appropriate funds to maximize their portfolios. 

</details>

<details><summary style="font-size: 16px"> Question 3: Did Robinhood users choose the most profitable assets?</summary>

<img src='Cap_Images\Annotation 2020-09-08 040631.png'/>
<img src='Cap_Images\Annotation 2020-09-08 040649.png'/>

### Question Details
I wanted to compare the top 5 performing assets and to top 5 most popular assets in Robinhood. I also wanted to see the trend of how and when users decided to buy and sell assets based on the change in stock price. Ford Motors was one of the most popular assets with users. I compared 4 more assets and you can see those findings in my notebook.

</details>

# Conclusion
Robinhood users had grown substantailly post COVID 19. The official declaration date for COVID was March 13, 2020 and my data went up to July 17, 2020. Between that time, the total user amount increased by 122.26%. This is a direct correlation with people wanting to invest due to the stock market quick crash in March and it's quick bounce back through July 17th. 

The most popular assets among Robinhood users were: 

        Stock Name               % Change Post COVID
    1. Aurora Cannabis Inc.            22.00%   
    2. Ford                            20.78%        
    3. General Electric                -9.80%  
    4. Walt Disney                     10.70% 
    5. GoPro Inc.                      82.56%
    
The percentage changes post COVID for these assets, besides Ford seems to be great looking at it from just a percentage change stand point. But all of the assets, except for Disney has a stock price of under $10 and their returns are very limited from a dollar amount stand point. 

Looking at the most profitable stocks post COVID:

        Stock Name               % Change Post COVID         
    1. Moderna                        345.00%                         
    2. DocuSign                       153.86%                         
    3. Zoom                           129.00%                         
    4. Amazon                         65.94%                          
    5. Netflix                        46.60%                          
    
It is very apparent that the Robinhood users did not choose the most profitable assets. My conclusion leads to price being one factor and not understanding recessions and how the economy works in another factor. I will go more into detail with that in the Recommendation section.
____
Using the Advanced Auto ARIMA model produced a far more accurate forecasting model than the simple Auto ARIMA model due to the ability of customizing the parameters. My r2 score went from a -0.15836897303755193 to a 0.7006142667306581. Or a -0.16 to a 0.70. It went from not accurate at all to being substantially accurate. 

I also believe that my model would have been a lot more accurate if it did not have the unforeseen COVID 19 stock market crash in March - April 2020. Trying to create accuracy with a recession built into the data makes things a lot harder since the forecasting values are determined by the past. I want to keep tweaking my model with the different advanced parameter options as well to see if I can  get my model to start to predict volatility. 
# Recommendation
I believe that the Robinhood users did not invest in the most profitable assets based on my findings. The assets that were the most popular were assets that would have be profitable pre COVID 19. If you look further into these specific industries, they have all been declining since March 13, 2020. Because of the current circumstances, our 'new normal' may become a permanent reality and investment strategies must shift. Industries like the car, agriculture, home appliances, and entertainment may all never be what they once were. When investing, you must look at the bigger picture. 

With companies now having to shift their business to an almost 100% digital platform, companies like FAANG are on the rise more than ever. FAANG stands for Facebook, Amazon, Apple, Netflix, and Alphabet(Google). Looking into technology companies seems to be the better investment move going forward. Thinking about how our world will forever change because of COVID 19 has to be in the forefront when making business and investment decisions. This is a concept that a lot of people, if not exposed to it, will not think about on their own. As you can see from my findings, self-managed investments without some form of in-depth knowledge about finance and economics will prohibit maximum profits. Just understanding the buy low, sell high method will give your ROI a boost. Smart investing is a proactive process and not a reactive process. If you react to the market, you will always be behind it. Working with a professional or at least someone who understands these concepts will ensure you are maximizing your portfolio growth potential.

____
* Please check out my blog post as well!
<a href="https://medium.com/@heatherrachael9/is-investing-in-robinhood-a-great-idea-c466ce69cc95">Medium Blog</a>

# Future Work
1. I want to compare asset growth to user popularity to see if this growth is truely from a business stand point and not from the increase in investors. This will give a false indication of a successful business and the stocks will go back down once their next quarterly statements show that they do not have a sustainable and profitable product or service.

2. I want to compare portfolios from Robinhood users to see the bigger picture. Right now, I have conducted my research on an asset to asset basis and comparing that portfolio to a strategically allocated portfolio from a professional financial advisor will solidify which option is the best.

3. I want to update my forecast model by tweaking the parameters to see if I can get more accuracy. I want to also model in volatility hoping that will help with my accuracy as well. 