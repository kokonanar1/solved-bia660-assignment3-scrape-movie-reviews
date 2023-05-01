Download Link: https://assignmentchef.com/product/solved-bia660-assignment3-scrape-movie-reviews
<br>
Choose one of your favorite movies and find this id of this movie at rottentomatoes.com Write a function getData(<em>movie_id</em>) to scrape reviews, including review date (see (2) in Figure), review description (see (1) in Figure), and score (see (3) in Figure) from the current page.

Input: movie id in rottentomatoes

Output: a list of 20 tuples, i.e. [(“February 19, 2019”, “It’s a typically excellent offering from the…” , “5/5”), …]

Test your function with a few movies to make your function is generic enough

Example:

<u><a href="https://www.rottentomatoes.com/m/finding_dory/reviews/">https://www.rottentomatoes.com/m/findin</a></u><a href="https://www.rottentomatoes.com/m/finding_dory/reviews/">g_</a><u><a href="https://www.rottentomatoes.com/m/finding_dory/reviews/">dor</a></u><a href="https://www.rottentomatoes.com/m/finding_dory/reviews/">y</a><u><a href="https://www.rottentomatoes.com/m/finding_dory/reviews/">/reviews/ (https://www.rottentomatoes.com/m/findin</a></u><a href="https://www.rottentomatoes.com/m/finding_dory/reviews/">g_</a><u><a href="https://www.rottentomatoes.com/m/finding_dory/reviews/">dor</a></u><a href="https://www.rottentomatoes.com/m/finding_dory/reviews/">y</a><u><a href="https://www.rottentomatoes.com/m/finding_dory/reviews/">/reviews/) </a></u>in total, 20 reviews returned

<h1>Q2. Plot data</h1>

Create a function plot_data which takes the list of tuples from Q1 as an input

converts the ratings to numbers. For example, 3.5/5 is converted to 0.7. For all reviews without a rating or with an alphabetic rating (e.g. A), set its rating to None

Hint: you can use try/except block to handle ratings which cannot be converted <a href="https://stackoverflow.com/questions/379906/how-do-i-parse-a-string-to-a-float-or-int-in-python">floats. See </a><u><a href="https://stackoverflow.com/questions/379906/how-do-i-parse-a-string-to-a-float-or-int-in-python">https://stackoverflow.com/questions/379906/how-do-i-parse-a-strin</a></u><a href="https://stackoverflow.com/questions/379906/how-do-i-parse-a-string-to-a-float-or-int-in-python">g</a><u><a href="https://stackoverflow.com/questions/379906/how-do-i-parse-a-string-to-a-float-or-int-in-python">to-a-float-or-int-in-p</a></u><a href="https://stackoverflow.com/questions/379906/how-do-i-parse-a-string-to-a-float-or-int-in-python">y</a><u><a href="https://stackoverflow.com/questions/379906/how-do-i-parse-a-string-to-a-float-or-int-in-python">thon </a></u><a href="https://stackoverflow.com/questions/379906/how-do-i-parse-a-string-to-a-float-or-int-in-python">(</a><u><a href="https://stackoverflow.com/questions/379906/how-do-i-parse-a-string-to-a-float-or-int-in-python">https://stackoverflow.com/questions/379906/how-doi-parse-a-strin</a></u><a href="https://stackoverflow.com/questions/379906/how-do-i-parse-a-string-to-a-float-or-int-in-python">g</a><u><a href="https://stackoverflow.com/questions/379906/how-do-i-parse-a-string-to-a-float-or-int-in-python">-to-a-float-or-int-in-p</a></u><a href="https://stackoverflow.com/questions/379906/how-do-i-parse-a-string-to-a-float-or-int-in-python">y</a><u><a href="https://stackoverflow.com/questions/379906/how-do-i-parse-a-string-to-a-float-or-int-in-python">thon)</a></u><a href="https://stackoverflow.com/questions/379906/how-do-i-parse-a-string-to-a-float-or-int-in-python"> for reference.</a>

calculates the average rating by the year of the review date plots a bar chart for the average rating of each year. The plot may look similar to the figure below.

<strong>Q3 (Bonus) Expand your solution to Q1 to scrape all the views for a movie.</strong>

Write a function getFullData(<em>movie_id</em>) to scrape reviews in all the pages. For the example shown in Figure of Q1, reviews are organized into 16 pages (See (4) of the figure). Scrape reviews from all the 16 pages. Save the result similar to Q1.

Note, you <strong>should not hardcode</strong> the number of pages, because the number of pages varies by movies. Instead, you should dynamically determine if the next review page exists or not.