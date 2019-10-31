
# Functions With Arguments - Lab

## Introduction
In this lesson, we have decided to visit one of our travel destinations! This time we have chosen to visit Albuquerque, but we aren't very familiar with this city and are quite hungry after our long flight. We will be working with information we obtained from Yelp and Google to help us find a restaurant where we can satisfy our hunger.

## Objectives
You will be able to:
* Declare and use a function with arguments

## Exploring Restaurants in Albuquerque

We've narrowed our search down to the 10 best restaurants in Albuquerque (according to a local guide), and collected their respective Yelp and Google ratings. The supposedly best restaurant is "Fork and Fig" (index 0) and the last spot of the top 10 is "Pollito con Papas".


```python
restaurants = ["Fork and Fig", "Fronties Restaurant", "Artichoke Cafe", "The Salt Yard", "Guava Tree Cafe"
               "Cocina Azul", "Farina Pizzeria", "La Crepe Michel", "Antiquity Restaurant", "Pollito con Papas"]
    
yelp_rating = [4.3, 4.5, 3.9, 2.3, 4.9, 4.8, 4.2, 4.4, 4.6, 3.9]  

google_rating = [4.9, 4.3, 4.7, 3.2, 4.4, 3.8, 4.8, 4.6, 4.2, 4.7]  
```

As we can see from our above comparison, Yelp provides us with the same information for both restaurants.  

## Writing our functions

Ok, now let's write a function `restaurant_details()` that allows to take in an index number (0-9) representing the 1st to 10th spot. The desired output of the function is the following printout:

" `restaurant name` has a Yelp Rating of `a` and a Google Rating of `b`"


```python
def restaurant_details(index):
    pass
```

Next, use your function to figure out the restaurant details for the restaurant with index 2.


```python
# Your code here  
# Expected output: "Artichoke Cafe has a Yelp Rating of 3.9 and a Google Rating of 4.7"
```

## Comparing restaurants

You would think that Restaurants higher up the list are rated better than restaurants lower down the list. Turns out that our guide has a slightly different perspective than the average Yelp or Google rater sometimes. 

Now let's write a function called `is_better_yelp()`. The first argument should be called `index_a` and the second argument should be called `index_b`, and should contain the corresponding restaurant indices.

The function should  return the following line if restaurant with index a has a higher Yelp rating than the one with index b:

>  "`Restaurant with index a` is better than `Restaurant with index a` according to the Yelp rating"

Alternatively, the function should return:

>  "`Restaurant with index a` is not better than `Restaurant with index b` according to the Yelp rating"

> **Note**: You haven't formally seen conditionals yet, but for this exercise, you'll be using something that looks like this in your code:

```python
if yelp_rating[index_a] > yelp_rating[index_b]:
        return "statement if condition is true"
    else: 
        return "statement if condition is false"
```


```python
def is_better(index_a, index_b):
    pass
    # Your code here
```

Next, run your code for the restaurants listed 4th and 8th by our guide.


```python
# Your code here  
# Expected output: The Salt Yard is not better than Antiquity Restaurant according to the Yelp rating
```

According to Yelp, our restaurant listed as 8th is actually better than the restaurant listed on the 4th place!

Awesome! We have built out some pretty cool functions so far. Next, we want to see if on average, Yelp or Google ratings are higher. We are going to create a function `mean_review()` that takes in a list as an argument, and calculates the mean rating for the 10 restaurants. We'll apply the function _twice_, once for the Yelp Ratings, and once for the Google ratings!


```python
def mean_review(rating_list):
    pass
    # code goes here
```

Use the function to compute the average Yelp Rating


```python
# Your code here
# Expected output: 4.18
```

Use the function to compute the average Google Rating


```python
# Your code here
# Expected output: 4.36
```

The Google ratings seem higher on average!

## Summary

Great! In this lab we saw how to pass both single and multiple arguments to functions. Function arguments can make functions more flexible and reusable!
