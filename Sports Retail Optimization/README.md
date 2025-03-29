This is an analysis of a sport's retail store sales information. There are five spreadsheets of information: *brands*, *finance*, *reviews*, *traffic*, and *info*. The goal of this analysis was to find out when and how the store brings in the most money, as well as where this store struggles to bring in money.

# Project Goals:
Money is profit, profit comes from revenue. The *finance* spreadsheet shows the total revenue of each product. I attempted to found out:

- Which products bring in the most revenue?
- Which brands bring in the most revenue?
  - When are these products sold?
  - Is there a common feature(s) between these products?
- Which products have the worst reviews?
  - Is there a common feature(s) between thse products?

# Data Info:
I started in Python by importing the CSV files, explored the infomrmation of each dataset, then import them into PostgreSQL. Ther were several *NULL* rows throughout the dataset, which I deleted to make analysis easier. I first did queries for individual tables and then began joining them together to specifically answer our project goals.

# Concluding Points
## Overall Rating and Review Info:

A total of 258 products that have a *0.0* rating.

A total of 212 products with no reviews.

Out of these totalS:

- *70* products have a *0.0* rating and also have a review. (trouble products?)
- *188* products have a *0.0* rating and no reviews. (are these products newer?)
- *24* products have a rating above zero but no reviews. (are they worth a review, like small/simple products? Are the ratings high enough to not need a written review?)

### Product Info:

- There are 186 products with a rating of 5.0 out of 5.0.
- The product with the most reviews is *310805* with 223 reviews, more than double that of the second-most reviewed product *880848-005* with 105 reviews.

## Best Product:
The product that makes this store the most money is *Nike Air Jordan 10 Retro* which brings has already brought in **$64,203.93**. This pair of shoes has a *4.7* rating from *223* reviews. From this analysis, this shoe was sold on Thursday and no other day.

## <ins>*Problems with this dataset*</ins>:

Only one of each product was sold, therefore I cannot do any accurate analysis of which product is most or least popular.
The Nike Air Jordan 10 Retro shoes were only sold on Thursdays, which seems very unrealistic, especially when they have given the store the most revenue. I did not proceed with finding the time at which they were most sold due to unrealistic data.
Some products have a listing price of 0.0 but have given the store revenue, such as the Nike Air Jordan 10 Retro. This makes no sense and I cannot do proper calculations to determine where there financial strengths and weaknesses are.

![image](https://github.com/user-attachments/assets/e71ca96a-13fa-43a6-9838-6629d4c974b5)

This dataset has over 3000 data points/products, of which 2259 are shoes and 71 are slippers. This is not realistic for a sports store, which can sell a lot more diverse products, especially sports' equipment.
