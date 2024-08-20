# nosql-challenge

The UK Food Standards Agency evaluates various establishments across the United Kingdom and gives them a food hygiene rating. Project to evaluate some of the ratings data in order to help their journalists and food critics decide where to focus future articles.


![english food](https://github.com/caitlin-hartley/nosql-challenge/blob/main/images/uk_food_magazine.jpg)

## Contents:

[Setup](https://github.com/caitlin-hartley/nosql-challenge/blob/main/README.md#setup)

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

---

## Analysis

### Exploratory Analysis

- Use count_documents to display the number of documents contained in the result.
- Display the first document(s) in the results using pprint
- Convert the result to a Pandas DataFrame, print the number of rows in the DataFrame, and display the first 10 rows

- Which establishments have a hygiene score equal to 20?

![q1](https://github.com/caitlin-hartley/nosql-challenge/blob/main/images/q1.png)

- Which establishments in London have a RatingValue greater than or equal to 4?

![q2](https://github.com/caitlin-hartley/nosql-challenge/blob/main/images/q2.png)

- What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?

![q3](https://github.com/caitlin-hartley/nosql-challenge/blob/main/images/q3.png)

- How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.

![q4](https://github.com/caitlin-hartley/nosql-challenge/blob/main/images/q4.png)
