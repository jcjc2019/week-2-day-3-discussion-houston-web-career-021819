#Answers

1 . When you tweet a tweet, your tweet is available to THE WHOLE INTERNET FOREVER. Why doesn't your tweet disappear after you post it? How does it stay on Twitter and stay associated to ​_your_​ account?

A: Each tweet is stored in a database of all tweets. 

2 . When you enter your debit card into an ATM, how is your account identified? How does the bank associate that card number to your account? How does your bank store your account information? Do you think your address and phone number are stored the same way as your account number and how much money you have?

A: The bank may have a large database of many different tables. In this case, a possible scenario is one table stores personal information with a person's name, address, phone number listed as properties. Another table stores information such as bank account number, and debit card number, as well as the balance. Another possiblity is the bank stores personal information and account information in two separate tables, while using a balance table to join the two. The balance table could be written and revised constantly.

 3 . How does Tinder know you are who you say you are when you open your application, type your password, and begin to swipe insatiably? How does it know that you and your latest match swiped right on each other, and that is wasn't someone other _John/Jane Doe_?
 
 A: All your personl information is stored at Tinder's back-end database, which may be in the form of a table that includes many columns, including your username, your password, your interests etc. Each user is identified by using primary key or username. Then when you anr your latest macth swpied right on each other, it is possible that Tinder will store that information in a separate table where you and your matach are listed there. Then the app automatically calls on this table and connects two users. Tinder may use a certain type of algorithm to calcuate the perfect match.


4 . How do you think Yelp can show you all Latin Restaurants, with a $$ price rating, in the Financial District, which have higher than a 3 star rating?

A: use SELECT
```sql
SELECT * FROM restaurants WHERE type = 'Latin' AND price_rating = '$$' AND location = 'Financial District' AND rating > 3;
```

 5 . What do you think this is doing:
```sql
SELECT * FROM artists WHERE ArtistName='Kid Cudi'
```
A. give a list of all rows that contains the column "Kid Cudi"