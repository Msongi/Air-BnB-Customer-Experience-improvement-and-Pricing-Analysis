# Customer Experience Improvement and Pricing Analysis Project

This project has 2 main parts:

- Part 1- Develop a **Customer Experiece Improvement** on the given training data. Find out the key metrics that can be used to measure customer experience and use those metrics to build an algorithm that can be used by the Customer experience team to improve customer experience. Then **Test Your Algorithm** and see that it has met the success criteria.
- Part 2- Determine what are the **factors that influence pricing**, ascertain if there has been a growth in airBnB business and where that growth has been. 
- Finally come up with some insights that can be used to advise Business Development, Marketing and Customer Experience teams

Let's start with some background.

-----

## Introduction
AirBnB was started in August 2008. It operates an online marketplace for lodging, primarily homestays for vacation rentals, and tourism activities. It is based in San Francisco, California. The platform is accessible via website and mobile app.It has grown into a multi-billion dollar world-wide company. As part of the growth initiative, AirBnB collected this dataset from AirBnB listings in Seatle in order to learn insights that will help improve customer experience and business development.

Insert image here

When AirBnB homes are listed. Features like cancellation flexibility, property type, price, istant bookable are used by customers to decide on which listing to book. A customer can even apply more filters like rooms and beds, verified places, ammenities or if they have extra guests. The goal of this project will be to answer these key business questions:
1. What features of the listings are related to price?    
2. What vibes are happening in each neighbourhood?    
3. Are there factors/metrics for that help understand customer experience?    
4. Are there things that guests/AirBnB can do to boost guest experience and get more clients?
5. Has there been an increase in the number of AirBnb hosts?
6. What are the busiest times of the year in seattle and by how much do the prices change

## Process
We will use the Cross Industry Process for Data Mining. Which involves these steps:
1. Business understanding – What does the business need?
2. Data understanding – What data do we have / need? Is it clean?
3. Data preparation – How do we organize the data for modeling?
4. Modeling – What modeling techniques should we apply?
5. Evaluation – Which model best meets the business objectives?
6. Deployment – How do stakeholders access the results?

-----
##  Algorithm Overview

### Criteria for model assessment

The model will be evaluated against tests to ensure its valid.

The first data mining problems will be approached using descriptive statistics and visualisations of the distributions. By these we will be able to ascertain key metrics and some feature importances.

We will also need to ensure that the metric chosen will satisfy the business requirements for being an adequate representation of customer experience, and that it is not just chosen solely to produce good results from the model (Feature importance)

For the second data mining problem, we will use cross validation to evaluate candidates for modelling the data. We will evaluate using the R2 score and the RMSE if using regression. We could also plot residuals of the model to evaluate skew.

The third data mining problem will follow from the solution of the second data mining problem. We can apply a properly evaluated model on the data in order to assess the feature importance. We will ensure that the features chosen from the feature importance are appropriate for using in a strategy that could conceivably target hosts and how they could improve the guests' experiences.

Finally, it is important to note the broad nature of the project. We will narrow it down to improve customer service. We are only looking to improve guests' customer experience, and this could be limited to certain subsets of the user base. As long as the user base chosen is large enough for potential insights to be significant, then this will contribute towards satisfying our business goals.
  
### Dataset
You wil be using the dataset from kaggle https://www.kaggle.com/airbnb/seattle to draw insights and build your models.

### Getting Started
The starter code includes is a well detailed jupyter notebook. It contains the process and details of analysis
AirBnB provided three items in their dataset. 

    Listings, including full descriptions and average review score
    Reviews, including unique id for each reviewer and detailed comments
    Calendar, including listing id and the price and availability for that day
We will use the calender data to draw insights on the growth of AirBnB over time. And to answer the questions on whether there are busy times and what the trends/busiest times to visit Seattle are

The reviews data will provide us with insights and features to answer our customer experience question. We will use it to determine if there are features that cab be used as a metric to measure and improve customer experience

The listings data will provide insights into the vibes in each seattle neighbourhood, it will also tell us which features affect pricing the most.


-----
## Key Findings from the Analysis of the data

When we started we sort to understand and answer these questions:

    What features of the listings are related to price?
    What vibes are happening in each neighbourhood?
    Are there factors/metrics for that help understand customer experience?
    Are there things that guests/AirBnB can do to boost guest experience and get more clients?
    Has there been an increase in the number of AirBnb hosts?
    What are the busiest times of the year in seattle and by how much do the prices change

Our Analysis of the data has uncovered these findings.

Price

    The neighbourhood, number of beds, how many nights the guest will be staying, 
    whether they have extra guests, the day of the week, the months, the neighbourhood, 
    whether its a holiday and Amenities provided
    
    Of all the amenities that we found and listed, the ones shown on the wordmap are the ones that are strongly related to price.
    
    Some of the main ones include Wireless Internet, smoke detector, Monoxide detector, Carbon monoxide detector,
    Essentials like shampoo, Free Parking and Family and kid friendly. 
    
    These improve customer experience and also contribute to pricing. The more ammenities the host adds the pricier the listing
    
    Appartments and houses are the most common properties with 45% and 44.7% of all the listings of room types and they are the most expensive

Vibes in each neighbourhood

    Broadway is the most frequently listed neighbourhood which occurs 397 times
    
    We see that there are zipcodes that have more listings like the 98122, 98103 and 98102. 
    
    These are generally higher, the bulk of the listings are on average the same until we get to 98104.
    
    Then we see 98199, 126,106,108,133,136 have about the same listings around the 50-60 listings average

**Has there been an increase in AirBnb's hosts

    Since 2008 to 2016. In 10 years, there was a growth from 4 listings to 3816 listings, the growth is exponential. 
    
    Between 2009 and 2011 the growth rate doubled at a average growth rate of 140% per year. From 2011 the growth rate
    
    steadied to an average growth rate of 30%. About 50% of hosts joined July 2013

Busiest times in Seattle and how prices change

    The summer is the busiest times in seattle, between June and August. Prices are highest during these times. 
    
    Holidays are generally higher priced on average than normal days.The Independence day holiday is the most expensive to visit in, in Seattle. 
    
    Good holidays to visit seattle on are Martin Luther King Jr and Washington's birthday, they are cheaper as well. 
    
    Weekends are also higher priced than week days, prices go up on Friday and Saturday

Customer metrics

    reviews per month and review score rating features are useful features for understanding customer experience and thus improving customer experience. 
    
    As expected some users/hosts have many reviews but fewer reviews per month suggesting they have been listed longer but not neccesarily that they are perfoming better than those with fewer number of ratigs but higher reviews per month


