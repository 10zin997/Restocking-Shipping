# DATA Structure Project 2
## Restocking-Shipping
### Restocking item that are out of stock
### Computing shipping cost


This program assumes that a company has warehouses in 5 cities: New York,
Los Angeles, Miami, Houston, and Chicago. In each warehouse the company stocks three
items. A record contains the amount of each item currently in each warehouse.

The record should contain an array of 5 warehouses with the name of each warehouse
and an array of the 3 items with the amount that is currently in stock in the warehouse.

Initially the warehouses are empty. Read in a card containing the three prices of the
three items. Then read in cards which may be any one of two types:

    1. Shipment cards containing....

        S   city    amt1    amt2    amt3

    This data represents a shipment to a given city of amt1 of item1, amt2 of item 2,
    and amt3 of item3.

    2. Order cards containing....

        O   city    amt1    amt2    amt3

    This data represents an order in a given city of the respective amounts of the
    variious items.



As each shipment card is read in, print it out, update the amounts in that warehouse
and then print on the next line:

        city    amt1    amt2    amt3

As each order card is read in, print it out. If there is enough in stock at that
warehouse of each item, update the amounts. If there is not enough, search the other
warehouses for the one which has the most of that particular item, ship the amount
needed from one warehouse to the other, printing out:

        x of item y shipped from city1 to city2

    and

        city1   amt1    amt2    amt3

10% extra is to be charged for any item shipped from one city to another. If no
single warehouse has enough extra to fill the order for a particular item, print out:

    Order Unfilled

However any shipments of the previous items remain in effect.
In either case print out the adjusted...

        city    amt1    amt2    amt3

And if the order is filled print...

    Price of Order: Price
