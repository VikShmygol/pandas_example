Following tasks were implemented in 'books_database.ipynb' with Pandas:

Fetch external database related to the books (http://www2.informatik.uni-freiburg.de/~cziegler/BX/BX-CSV-Dump.zip). 
This database includes a csv file with authors and their books. This dataset needs to be preprocessed and split into multiple csv files. 
One file will contain information about the book (BOOKS.CSV), another one the information about book authors (AUTHORS.CSV) and the last one their relationships (BOOK_AUTHORS.CSV). 
The next step is to match author names from AUTHORS.CSV in the description of SITE_DATA.CSV. The result of this operation needs to be saved to the file MENTIONED_AUTHORS.CSV, which includes the following columns:

1. reference to the author from the AUTHORS.CSV
2. url of the page where this author appeared
3. snippet of text (2-3 meaningful sentences around matched author name)

The accuracy of the matching also must be measured (for example confusion matrix for the specific matching algorithm). Pandas is required part for each step related to the data processing - it should be used there.
Additional tasks:
-Find the most frequent author of the site.
-Find what books from the site are missing in the BOOKS.CSV for the authors from MENTIONED_AUTHORS.CSV.
-Create a top 10 most frequent meaningful words from the title of each BOOKS.CSV
-Create BOOK_DESCRIPTION.CSV for the books from BOOKS.CSV, wherever it is possible.