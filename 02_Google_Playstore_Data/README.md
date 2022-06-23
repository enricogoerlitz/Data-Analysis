# EDA Project: Google Playstore Data

## General

Author: Enrico Goerlitz <br/>
Initial Date: 19.06.2022

<br>

## Description

This dataset came from <a href="https://datacamp.com">datacamp.com</a> and contains data of the Google Playstore. <br>
We want to find out, which kind of apps are the most popular e.g. by the rating download rates and much more!

<br>

## Data questions

### Main-Topics

#### Which kind of apps got the best rating?

-   genre

-   content ratings

-   free / paid apps

-   price category at paid apps

-   review count of app

-   app size

#### Which kind of apps got the most downloads?

-   genre

-   rating

-   free / paid apps

-   price category at paid apps

-   review count of app

-   app size

<br>

### General-Topics

#### Genre

-   What are the most published genres?

#### App Rating

-   Are higher rated apps more downloaded?

-   How is the rating distribution of the different content ratings?

-   How is the total rating distribution over all apps (0.5 - 5 categories)?

-   Got a app with many reviews an better rating? Is there a significant threshold?

#### App Reviews

-   Are high reviewed apps more downloaded

#### Free & Paid Apps

-   How is the distribution of paid and free apps?

-   Do paid apps get a better rating than free apps?

-   In terms of total releases, are paid apps downloaded more than free apps?

#### Size

-   Are bigger apps more downloaded

## Data cleaning & preprocessing

-   Drop columns: {Unnamed: 0, Android Ver, Current Ver, Last Updated, Category}

-   Rename columns: {Installs: Downloads, Content Rating: Content Group}

-   Rating: interpolate by the median of genre rating

-   Genre: split genre with more genres in one cell and add the genre as new copied row (in a new df_genre_cleaned df)

-   Reviews: classify Reviews to Review Rate {Low, Medium, High} as category dtype

-   Size: interpolate by the median of genre size; classify to Size Class {Low, Medium, High} as category dtype

-   Downloads: classify to Download Rate {Low, Medium, High} as category dtype

-   Type: as category dtype

-   Price: convert to floats; classify to Price Class {Low, Medium, High, Very High} as category dtype

-   Content Rating: map {Mature 17+: Adults, Adults only 18+: Adults, Everyone 10+: Everyone, Unrated: Everyone}

<br>

## Used technologies

-   Python
-   NumPy
-   Pandas
-   Matplotlib
-   Seaborn

<br>

## Used resources

https://unsplash.com/ <br>
https://unsplash.com/photos/mr4JG4SYOF8 <br>
https://stackoverflow.com/ <br>

<br>

## Copyright

All licenses in this repository are copyrighted by their respective authors. <br>
Everything else is released under CC0. See `LICENSE` for details.
