# Restaurant Review System

This is a simple Python program for managing restaurant reviews.

## Description

### Customer

Represents a customer who can review restaurants.

#### Attributes

- `first_name`: First name of the customer.
- `last_name`: Last name of the customer.

#### Methods

- `reviews()`: Returns a list of reviews made by this customer.
- `restaurants()`: Returns a list of restaurants reviewed by this customer.
- `num_negative_reviews()`: Returns the number of negative reviews (ratings <= 2) made by this customer.
- `has_reviewed_restaurant(restaurant)`: Checks if the customer has reviewed a specific restaurant.

### Restaurant

Represents a restaurant that can be reviewed.

#### Attributes

- `name`: Name of the restaurant.

#### Methods

- `reviews()`: Returns a list of reviews for this restaurant.
- `customers()`: Returns a list of customers who have reviewed this restaurant.
- `average_star_rating()`: Returns the average star rating for this restaurant.
- `top_two_restaurants()`: Returns the top two restaurants based on average ratings.

### Review

Represents a review made by a customer for a restaurant.

#### Attributes

- `customer`: Customer who made the review.
- `restaurant`: Restaurant being reviewed.
- `rating`: Rating given in the review.

## Usage

You can use these classes to manage restaurant reviews in your Python projects. Here's an example of how to use them:

```python
# Create customers
customer1 = Customer("John", "Doe")
customer2 = Customer("Jane", "Smith")

# Create restaurants
restaurant1 = Restaurant("Restaurant A")
restaurant2 = Restaurant("Restaurant B")

# Create reviews
review1 = Review(customer1, restaurant1, 4)
review2 = Review(customer2, restaurant2, 5)

# Get top two restaurants
top_restaurants = Restaurant.top_two_restaurants()
print("Top two restaurants:", [restaurant.name for restaurant in top_restaurants])

Author
saarakhalid GitHub: @saarakhalid LinkedIn: saarakhalid
