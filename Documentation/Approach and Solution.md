# Solution Details

## Source File Analysis

The source file to our project is a csv file containing rating and reviews of various movies.<br>
Path: Documentation/Popular Movies TV shows from Prime Videos Netflix version_3.csv<br>
**_Please note that in the code we have placed it in the Bronze Volumes movie.movie_bronze.dataset-movies to fetch the data._ <br>

It contains the following fields:-
<table>
<tr><th>Field</th><th> Description</th>
<tr><td>[Blank]</td><td>No definition for this field. Only obeservation is this field holds ID - 1 value</td></tr>
<tr><td>ID</td><td>Movie Id with values like 1,2,3,4...</td></tr>
<tr><td>Title</td><td>Name of Movie</td></tr>
<tr><td>Year</td><td>Year of Release</td></tr>
<tr><td>Rating</td><td>Age rating</td></tr>
<tr><td>IMDb</td><td>IMDb rating out of 5</td></tr>
<tr><td>Rotten Tomatoes</td><td>Rotten tomatoes rating out of 100</td></tr>
<tr><td>Genre</td><td>Genre under which movie is categorised</td></tr>
<tr><td>Netflix</td><td>Was the move released in Netflix? Value is 0 if No and 1 if Yes</td></tr>
<tr><td>Amazon Prime Video</td><td>Was the movie released in Amazon Prime Video? Value is 0 if No and 1 if Yes</td></tr>
</table>

## Creation of Medallion Architecture

**Notebook Path:** _Movie-Data-Engineering-Using-Databricks/Create medallion Architecture - movie/create medellion architecture for movies.ipynb_<br>

With notebook we creating the Medallion Architecture. First we create the Catalog named movies. Inside the catalog we create three Schemas:-
- movie_bronze
- movie_silver
- movie_gold

Once the notebook is run successfully we will see the following output in Catalog
![](medallion_architecture.jpg)

## Load Data in Bronze

**Notebook Path:** _Movie-Data-Engineering-Using-Databricks/Job pipeline setup for refresh Bronze, Silver and Gold layer Data/Create job pipeline for refreshing bronze and silver layer.ipynb_<br>

In this notebook we load the csv file into a record in bronze layer called movies. The table is created as movie.movie_bronze.movies. It contains the raw data as it is we have in the csv source file.

![](Bronze_table.jpg)

This table will be the source of data for us to build the tables in Silver Layer.

## Load Data in Gold
