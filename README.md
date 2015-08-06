# Saudi Newspaper Corpora (SaudiNewsNet)
This repo contains a set of Arabic newspaper articles alongwith metadata, extracted from various Saudi newspapers.

Statistics
----------
The dataset currently contains 22,524 articles, all compressed into zip files. The articles were extracted from the following Saudi newspapers (sorted by number of articles):

 - [Al-Riyadh](http://www.alriyadh.com/) (3,385 articles)
 - [Al-Jazirah](http://al-jazirah.com/) (2,484 articles)
 - [Al-Sharq Al-Awsat](aawsat.com/) (2,341 articles)
 - [Al-Yaum](http://alyaum.com/) (2,285 articles)
 - [Al-Eqtisadiya](http://aleqt.com/) (2,204 articles)
 - [Okaz](http://www.okaz.com.sa/) (2,103 articles)
 - [Al-Weeam](http://alweeam.com.sa/) (1,715 articles)
 - [Al-Watan](http://alwatan.com.sa/) (1,637 articles)
 - [Ain Alyoum](http://3alyoum.com/) (1,618 articles)
 - [Al-Madina](http://www.al-madina.com/) (1,520 articles)
 - [Sabq](http://sabq.org/) (1,334 articles)
 - [Arreyadi](http://www.arreyadi.com.sa/) (128 articles)

Article Format
----------
Each article is represented as a JSON object stored in a file (file name format: newspaper-name-[some-id].json). All files are formatted in UTF-8.

The JSON object for each article contains the following fields (notice that some fileds can have empty values in case the crawler failed to extract them):

 - **`url`**: The full URL from which the article was extracted.
 - **`title`**: The title of the article. Can be empty.
 - **`author`**: The author of the article. Can be empty.
 - **`content`**: The content of the article.
 - **`date_extracted`**: The timestamp of the date on which the article was extracted. It has the format `YYYY-MM-DD hh:mm:ss`. Notice that this field does not necessarily represent the date on which the article was authored (or made available online), however for articles stamped with a date of extraction after August 1, 2015, this field most probably represents the date of authoring.


# License
![Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png)

This work is licensed under a **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License**. The dataset is shared for the sole purpose of aiding open research in Arabic computing. The ownership of each article within the dataset belongs to the respective newspaper from which it was extracted; and the maintainer of the repository does not claim ownership of any of the content within it. If you think, by any means, that this dataset breaches any established copyrights; please contact the repository maintainer.


