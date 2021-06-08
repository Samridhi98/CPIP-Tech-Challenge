# CPIP-Tech-Challenge
Hi! We have implemented 2 solutions - CSV Encoding & Fuzzy Search

## CSV Encoding
  Backend and processing - Python & Flask
    We have used simple pandas to read the file. Given we don't know what encoding it actually is we use the chardet module to try and automatically guess what the right encoding is. Post this we process the file and return the excel with corrected encodings.
  Frontend - HTML, CSS, Javascript
  
  ### Encoding Types
  Tested with various encoding types:
  1. ISO-8859-1
  2. ASCII
  3. UTF-8
  4. WINDOWS 1251
  5. Big-5
  
  ### Datasets
  1. Transcripts - (Devnagri file)
  2. Mobile_data - (Chinese Script)
  3. imdblet_latin - (Latin)

  ### Steps to run 
    1. $git clone 
    2. $cd encoding
    2. $python myapp.py
  
  You will see the form on "http://localhost:5000/"
  Drop your file and the processed file will be downloaded!
  
## Fuzzy Search
  We will use TF-IDF, N-grams & Cosine Similarity techniques to process the data and find out the minimum distance between the query and search data.
  We have used a csv file as our dataset to perform the search.
  
### Library Requirements
  1. pandas
  2. sklearn
  3. scipy
  4. numpy
  5. sparse_dot_topn
  (I have used pip freeze to generate requirement.txt file hence may not be useful in some environments)

### Run
  1. $git clone
  2. $cd fuzzy
  3. $python main.py
  
## Future Implementation
  1. Building a interactive UI for fuzzy search
  2. Incorporating both encoding and fuzzy in a web app with toggle menu
  3. Multiple file downloads with encoding
