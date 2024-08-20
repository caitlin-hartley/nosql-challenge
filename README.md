# nosql-challenge

The UK Food Standards Agency evaluates various establishments across the United Kingdom and gives them a food hygiene rating. Project to evaluate some of the ratings data in order to help their journalists and food critics decide where to focus future articles.


![english food](https://github.com/caitlin-hartley/nosql-challenge/blob/main/images/uk_food_magazine.jpg)

## Contents:

[Setup]

[Analysis]


---

## Setup

### Database and Jupyter Notebook Set Up

- Import the data in the establishments.json file in Terminal
- Name the database uk_food and the collection establishments
- Import the libraries: PyMongo and Pretty Print (pprint)
- Create an instance of the Mongo Client

### Update the Database
- Add the Penang Flavors restaurant to the database

![penang](https://github.com/caitlin-hartley/nosql-challenge/blob/main/images/add_penang.png)

- Find the BusinessTypeID for "Restaurant/Cafe/Canteen" and return only the BusinessTypeID and BusinessType fields
- Update the new restaurant with the BusinessTypeID

- Check how many documents contain the Dover Local Authority
- Remove any establishments within the Dover Local Authority from the database
- Check the number of documents to ensure they were deleted

![dover](https://github.com/caitlin-hartley/nosql-challenge/blob/main/images/delete_dover.png)

- Use update_many to convert latitude and longitude to decimal numbers
- Use update_many to convert RatingValue to integer numbers
