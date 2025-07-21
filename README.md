# European Parliament Sessions Dataset (1996–2024)

<div align="justify">

The dataset was self-developed, taking the data from the HTML code used to structure the records at the EP website at <a href="https://www.europarl.europa.eu/plenary/en/debates-video.html">https://www.europarl.europa.eu/plenary/en/debates-video.html</a>. This was done through a Python scraper, which saved relevant information such as speaker names, countries, parties and quotes. The outcome was a set of 29 CSV files amounting to over 600,000 quotes. The data is organised in CSV files chronologically by date and preprocessed for text mining with NLTK, having removed stopwords and stemmed the dataset. From 2012 the data was translated using the MarianMT translation model (<a href="https://huggingface.co/docs/transformers/model_doc/marian">https://huggingface.co/docs/transformers/model_doc/marian</a>) as the original records were no longer in English. The party and country data was bolstered by cross-referencing with the EP records of MEPs: <a href="https://www.europarl.europa.eu/meps/en/directory/all/all">https://www.europarl.europa.eu/meps/en/directory/all/all</a>. This database was created for the purposes of my master's thesis available here: <a href="https://studenttheses.uu.nl/handle/20.500.12932/49054?show=full">https://studenttheses.uu.nl/handle/20.500.12932/49054?show=full</a>.

The precise number of quotes contained in the dataset is 624,001 quotes, with an average of 21,782 quotes per year. These represent debates, procedural statements, questions and answers, and other forms of parliamentary proceedings carried out in the 12 plenary meetings held yearly in Strasbourg, alongside 5 to 10 additional meetings held to address minor proceedings and exceptional circumstances in Brussels. In these meetings, which have a duration of 2 to 3 days, the average quote length was around 92 words. Generally, the frequencies tended to grow slightly over time but remained consistent. The notable exception is the 2014 to 2016 period, which saw abnormally high quote numbers of up to 93,000 in 2016, followed by a sharp reduction in the number of quotes in 2017. This is due to a temporary change in the parliamentary proceeding practices, whereby written responses were either more commonly allowed or better recorded between 2014 and 2016, encouraging greater participation among MEPs and creating a period with a richer quantity of data to draw from.

</div>

## Quotes per Year and Number of Quotes in Writing

<p align="center">
  <img src="https://github.com/user-attachments/assets/d60a33b8-2bb3-458d-a4a4-c8241f96d1d4" alt="Quotes per Year" width="80%">
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/6deefcb4-31a3-4fcb-b28d-dd5278c9e46a" alt="Quotes in Writing" width="80%">
</p>
