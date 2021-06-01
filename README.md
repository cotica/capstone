# Amazon recommender

- - - 

## Problem space and question

I am setting out on a bold personal mission: using my own 12-year Amazon purchase history, can a recommender I build beat the recommendations from Amazon itself?

- - -
## Data sources

For my training data, I am going to use my own Amazon purchase history.

![](http://media.corporate-ir.net/media_files/IROL/17/176060/Oct18/Amazon%20logo.PNG)


## Data acquisition strategy

Download data using [report tools](https://www.amazon.com/gp/b2b/reports) from Amazon.

- - -
## Metrics and evaluation

Using the Amazon [product API](https://pypi.org/project/python-amazon-product-api/0.2.5/), we will generate some product recommendations for my test set, and then compare against ones recommended by Amazon itself (on my homepage). We will iterate through this 25 times.

We will then see if I would actually accept those recommendations both from a) Amazon and b) from my Product Recommender.


## Analysis & key findings


## ML

For the test set, we will use a product catalog API.


## Conclusions and recommendations

### Challenges

### Assumptions made

- - -
## Report and presentation links

[`Slides`](https://docs.google.com/presentation/d/16-24og3wl4MC0OUlwuakeZuyuqF_WCxy1lFTB3g3K-8/edit?usp=sharing)

[`EDA report`](./code/Amazon-order-history-EDA.ipynb)
