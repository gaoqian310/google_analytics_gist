# google_analytics_gist
some question to be asked when look at the data:
- what percent of visitors are actually using the site search?
  - if this is a high number, are they struggling to find what they need?
  - what are their most common searches?
  - Anything you can use for next campaigns?
  - Will rearrange the products to feature those product help?
  - Are they searching a different names for the product?
- What pages are people searching from rather than home page?
  - Is that caused by some page experience?
- Time to purchase and session to purchase
  - How long take to conversion
  - Email marketing

# google default analytics is weighted on "last click"
Google analytics default show conversion metrics based on the last click interation, which gives too much weights to the most common last click paths, such as branded search or direct traffic, need some different attribution models comparsion.

- First click model have different contribution
  - Biggest question to ask: What channels improve the most when you move to first click attribution, which might be weighted too less in google anlytics
- Time Decay model
  - Any channel is more or less effective using time decay model?
- Liner attributions model and others we can discover.


# Goog analytics limitations on ML

Instead of occurrence based data usable to train a predictive model, GA will provide aggregate data which represents statistics on your traffic given a period 

Require to query GA to get occurrence based reports in order to cope with this problem.

In addition to that, GA will be limited to get the many occurrences and attributes that makes a ML algo satisfied. You will have the following limitations:

- query can have maximum 7 dimensions
- query can be include maximum 90 days when using segments
- reports limited by 10'000 rows

However there are ways to programmatically merge sequential queries to walk around those obstacles.

# 
