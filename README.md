# IMDB-Movies

## Extracting, Transforming, and Loading movie information using APIs and SQL

## Author: Joseph Lim

### Business Problem:
Client wished to create a database of movies from 2000-2022 using movies that were US-centric, as well as determine which movies were successful.

### Data Extraction

Data was extracted collected [from this source](https://datasets.imdbws.com/) as well as extracted from [The Movie DataBase](https://www.themoviedb.org/).

### Data Transformation

Data was transformed using Pandas to create multiple tables.

### Data Loading

Data was loaded into MySQL for later queries.

### Hypothesis Testing

#### Client specified question: Does movie rating (PG, G, R, etc.) affect revenue?

After running a Tukey test, it was determined that movie rating affect revenue. PG-13 movies earned significantly more than PG rated movies, which in turn earned significantly more than G and R rated movies. However, there was no significant difference in revenue in movies rated G and R.

#### Determining if the pandemic may have affected movie revenue.

Two, two year datasets were extracted with SQL from the created database and compared, one from 2018-2019, and the other from 2020-2021. After running an independent T-Test, it was determined that movie revenue was affected during the pandemic. Movies prior to the start of the pandemic earned more revenue than movies that debuted during the first two years of the pandemic.

#### Determining if movie length may have affected movie revenue

Data was extracted from the SQL database and sorted based off of if it was 2 hours or less, or longer than 2 hours. After running an independent T-Test, it was determined that movies with longer revenue earned significantly more than movies that were lesss than 2 hours long. 

### Limitations & Next Steps
* There can always be better visuals.

* A series of regressions may be useful for helping predict revenue by movie.

### For further information

Please send me an email @ jplim96@gmail.com. 
