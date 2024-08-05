![star_wars_unsplash](star_wars_unsplash.jpg)

Lego is a household name across the world, supported by a diverse toy line, hit movies, and a series of successful video games. In this project, we are going to explore a key development in the history of Lego: the introduction of licensed sets such as Star Wars, Super Heroes, and Harry Potter.

In this project we will see the impact of licensed sets, the quantity compared to those that are Lego's own, as well as the sets with the most pieces, the most popular sets.
We will do an A/B testing and a small three-year prediction to see if the number of sets increases.
We also developed two connections to an API for a set of parts based on the name of the set and the technical name of the part, which will return an image of it.

## The Data

You have been provided with two datasets to use. A summary and preview are provided below.

## lego_sets.csv

| Column     | Description              |
|------------|--------------------------|
| `"set_num"` | A code that is unique to each set in the dataset. This column is critical, and a missing value indicates the set is a duplicate or invalid! |
| `"name"` | The name of the set. |
| `"year"` | The date the set was released. |
| `"num_parts"` | The number of parts contained in the set. This column is not central to our analyses, so missing values are acceptable. |
| `"theme_name"` | The name of the sub-theme of the set. |
| `"parent_theme"` | The name of the parent theme the set belongs to. Matches the name column of the parent_themes csv file.
|

## parent_themes.csv

| Column     | Description              |
|------------|--------------------------|
| `"id"` | A code that is unique to every theme. |
| `"name"` | The name of the parent theme. |
| `"is_licensed"` | A Boolean column specifying whether the theme is a licensed theme. |