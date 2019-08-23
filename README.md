### Bacterial Biodiversity

Given an SQLite database containing information about the biodiversity of specific bacterial cultures,
I was tasked with creating a dynamic dashboard that queries the database and outputs visualizations based
on specific set selections. So, this assignment required an understanding of how to curate a front-end
and a back-end.  This task was accomplished using a combination of flask and javascript. The app was ultimately hosted
on Heroku. 

I used MySQL workbench to get a basic idea of what the data looks like. The columns afforded included
often repeated information: i.e., the infromation ascribed to the set itself (the metadata). It also
included single rows for every bacteria, with id, labels, and values ascribed to each one. 

The Python app itself relies on SQLAlchemy to quickly and efficiently query the database. Using the 
selected sample, I needed to harvest the metadata and the sample information for each bacteria. To this
end, I created two separate flask paths. They each returned json objects. The sample data was returned
as a list of values.

The Javascript consisted mainly of taking the already created json objects, and converting them into
traces that could be used by plotly to create the charts of interest.

The resulting app was then hosted on Heroku. The app can be accessed [here](https://biodiversityforucb.herokuapp.com/)
