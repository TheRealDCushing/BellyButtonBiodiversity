### Intro

Given an SQLite file, I was tasked with creating a dashboard that could conveniently display data. The theme of the data was belly-button biodiversity.

### Method & Results

SQLAlchemy queries were used in combination with Flask to get the data for each call. A bubbleplot and a pie chart are dynamically generated at each selection of a subject ID.

The resulting app was then hosted on Heroku. The app can be accessed [here](https://biodiversityforucb.herokuapp.com/)
