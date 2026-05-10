# NKC-Health-Hospital-Sentiment-Analysis-Project
Text analytics project using sentiment analysis and n-grams on hospital reviews

NKC Hospital Text Analysis of Patient Reviews

Business Description

The business analyzed in this project is North Kansas City Hospital (NKC Health).
The goal of this project is to analyze patient reviews to understand patient experiences, identify recurring issues, and find areas where the hospital can improve service delivery and patient satisfaction.

Dataset Description

The dataset consists of patient reviews collected online from Google Maps reviews. Each review includes text (comments) and a rating. The text data was used for analysis, and the ratings (1-5 stars) were used to help identify negative and positive experiences. The reviews were processed and cleaned to ensure consistency for text analysis.

Executive Summary

In this project, I used multiple text analytics methods to analyze patient reviews and connect the results to real issues the hospital needs to address.
First, I cleaned the text data by removing punctuation, converting text to lowercase, and removing stopwords. This made the data easier to work with and reduced noise, which helps improve the accuracy of the analysis and ensures the hospital is working with reliable insights.
Next, I performed text preprocessing, including tokenization and lemmatization, to break the text into usable words and standardize them. This makes it easier to identify patterns across reviews instead of treating similar words as different issues.
I then used sentiment analysis (BERT) to classify reviews as positive, negative, or neutral. This made it easier to separate good experiences from bad ones and focus more on negative feedback. This helps the hospital quickly identify where patients are having poor experiences and prioritize those areas.


 <img width="585" height="198" alt="image" src="https://github.com/user-attachments/assets/2fed6962-a9d7-4170-93d1-850b649d7245" />


After that, I used word frequency analysis, especially on low-rated reviews (1–2 stars), to identify commonly used words in poor experiences. This showed repeated issues mentioned by patients and helps the hospital focus on the most common problems instead of guessing.
I also applied n-gram analysis (bigrams and trigrams) to identify common phrases. Examples include “told wait,” “pain meds,” and “waiting room,” which point directly to patient complaints. This gives more context about what patients are actually experiencing, not just single words.
Top Words/Phrases in Negative Reviews (Ngram)

 
 <img width="440" height="471" alt="image" src="https://github.com/user-attachments/assets/d3ef1232-c2a9-4770-8bfc-6e87942e8d65" />


<img width="454" height="539" alt="image" src="https://github.com/user-attachments/assets/3398bb9e-4cf7-4a5c-88ab-6be4f6c6e459" />


 Next, I used keyword-based classification to group complaints into categories such as wait time, staff attitude, billing, and communication. This made it easier to see which issues occurred the most and helps the hospital prioritize improvements based on what shows up the most in reviews.

 
<img width="495" height="354" alt="image" src="https://github.com/user-attachments/assets/030c876d-219d-4109-afdb-52022327983d" />


I then applied topic modeling (LDA) to automatically group reviews into themes. The results aligned with earlier findings, confirming key problem areas like wait time, staff behavior, and pain management. This helps validate that the results are consistent and not just random patterns.
Finally, I used text summarization methods:
•	TextRank (extractive)
•	PEGASUS (abstractive)
These helped reduce long reviews into shorter summaries while still keeping the main points. This can help management quickly review feedback without having to read every single review.

Combining Text and Numerical Analysis

One clear example of combining text and numerical data in this project is using ratings together with word frequency and n-gram analysis.
From the BERT sentiment and rating comparison table, most 1-star reviews are classified as negative, while most 5-star reviews are classified as positive. However, there are a few mismatches where a review may have a higher rating but still contains negative sentiment. This shows that ratings alone do not always capture the full patient experience.
I filtered out low-rated reviews (1–2 stars) and analyzed the most common words and phrases in those reviews. This made it easier to see what patients were actually complaining about.
Instead of just knowing patients are unhappy, the analysis shows that the issues are mainly related to wait times, staff attitude, and delays in treatment.
Combining both ratings and reviews text makes the results more useful because it shows both how patients rate their experience and the specific reasons behind it.

Key Findings

The main problems identified are:
1. Long wait times (e.g., “waiting room,” “told wait”)  
2. Poor staff attitude  
3. Pain management issues (e.g., “pain meds”)  
4. Billing concerns  
5. Communication issues  
Positive reviews showed strengths such as:
1. Good nursing staff  
2. Patient comfort  
3. Good overall care  

Conclusion and Recommendations

Based on the analysis, the hospital should focus on the following:
1. Reduce wait times, especially in the emergency room  
2. Improve staff communication and patient interaction  
3. Improve pain management processes  
4. Increase transparency in billing  
To move forward, the hospital should:
1. Continue analyzing new patient reviews regularly  
2. Track complaint categories over time  
3. Focus on the most frequent issues first  
4. Use this data to guide operational and service improvements  
All charts, tables, and outputs used in this analysis are included in the Colab notebook uploaded in this repository.
