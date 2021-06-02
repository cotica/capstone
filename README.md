# Product recommender (Me vs Amazon)

- - - 

## Problem space and question

I am setting out on a bold personal mission: using my own 12-year Amazon purchase history, can a recommender I build beat the recommendations from Amazon itself?

- - -
## Data sources

For my training data, I am going to use my own Amazon purchase history along with any donated / sourced purchase history I can get my hands on in this very limited timeframe and mindful of PII.

![](http://media.corporate-ir.net/media_files/IROL/17/176060/Oct18/Amazon%20logo.PNG)


## Data acquisition strategy

1. For training:

** Download purchase history data using [Amazon report tools](https://www.amazon.com/gp/b2b/reports) from Amazon.

** Potentially request history from classmates and / or family


2. For test:

** Obtain generic product catalog data. Possible [source](https://data.world/promptcloud/amazon-product-listing-q2-2020/workspace/project-summary?agentid=promptcloud&datasetid=amazon-product-listing-q2-2020)

- - -
## Metrics and evaluation

Using a sample from the Amazon product catalog, we will generate some product recommendations for my test set, and then compare against ones recommended by Amazon itself (on my homepage). We will iterate through this 25 times.

We will then see if I and / or my classmates or family members would actually accept those recommendations both from:

a) Amazon

b) from my Product Recommender

If they accept, then we rank our recommendations as good, if they do not, then we rank recommendations as poor.

We are shooting for more than 50% accuracy. 50% accuracy is basically a shot in the dark (coin flip), less than that means that we should leave this job for Amazon and probably get out of the recommendation business.

- - - 
## Methodology


### Challenges

The first challenge was very much gaining access to Amazon's product catalog. To do this, I needed to get an Affiliate Marketer (Amazon Associate) seller account, which in itself required a website to be up and running (here's [mine](https://productincubator.co/)) where I could place and monetize Amazon's product links, all in order to get an Amazon API secret and key to use to obtain their coveted product data. This was scratched in favor of 


### Assumptions made


### Questions along the way

1. What is a good predictive test / training set size?
2. How to we tackle the inherent bias from sampling just a single user's (my!) preferences?
3. How many iterations do we want to run through?
4. How do we evaluate the recommendations? What baseline do we use to make the determination?
5. Merging strategy


- - -
## Analysis & key findings



## ML

For the test set, we will use a product catalog API.

- - - 

## Conclusions and recommendations


WARNING! WARNING! This is not production ready!

In the future, we would want to collect samples from other consumers and get some good variety (at least 30 samples x say 100-500 products each!), for this recommender to be validated more legitimately.

- - -
## Report and presentation links

[`Slides`](https://docs.google.com/presentation/d/16-24og3wl4MC0OUlwuakeZuyuqF_WCxy1lFTB3g3K-8/edit?usp=sharing)

[`EDA report`](./code/Amazon-order-history-EDA.ipynb)

- - -
## References and contributors

The General Assembly instruction team for Data Science Immersive cohort DSIR-322 greatly contributed in consultation for this project. It includes Gwen Rathgeber, Charlie Rice, Heather Robbins and Devin Fay.

In addition, several family members assisted with helping obtain the required ad purchases to satisfy Amazon's own requirements. These family members include Rick and Nellie Troisi.
