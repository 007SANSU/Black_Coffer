# Black_Coffer
Python pipeline for Blackcoffer assignment that cleans article text, performs sentiment and readability analysis, and outputs metrics (sentiment scores, Fog Index, word counts, etc.) in the exact Output Data Structure format, saved as UTF-8 Excel and CSV.

# Instructions to Run final_text_analysis.py

## Approach:
1. Read Input.xlsx containing URL_ID and URL for each article.
2. Read pre-extracted article text files from 'articles/' folder, named as URL_ID.txt.
3. Load stopwords from provided StopWords files.
4. Clean text by removing stopwords.
5. Compute 13 text analysis metrics from Text Analysis.docx:
   - POSITIVE SCORE
   - NEGATIVE SCORE
   - POLARITY SCORE
   - SUBJECTIVITY SCORE
   - AVG SENTENCE LENGTH
   - PERCENTAGE OF COMPLEX WORDS
   - FOG INDEX
   - AVG NUMBER OF WORDS PER SENTENCE
   - COMPLEX WORD COUNT
   - WORD COUNT
   - SYLLABLE PER WORD
   - PERSONAL PRONOUNS
   - AVG WORD LENGTH
6. Store results in Final_Output.xlsx (UTF-8) and Final_Output_UTF8.csv.

## How to Run:
1. Ensure you have:
   - Input.xlsx
   - articles/ folder with all article text files named as URL_ID.txt
   - StopWords text files in same folder
2. Install dependencies:
   pip install pandas numpy xlsxwriter openpyxl
3. Run:
   python final_text_analysis.py

## Output:
- Final_Output.xlsx (Excel format, matches Output Data Structure.xlsx column order)
- Final_Output_UTF8.csv (UTF-8 encoded CSV)

## Dependencies:
- Python 3.8+
- pandas
- numpy
- xlsxwriter
- openpyxl
