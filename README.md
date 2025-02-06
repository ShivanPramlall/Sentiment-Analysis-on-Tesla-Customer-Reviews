**Project Documentation: Sentiment Analysis on 2024 Tesla Customer Reviews**
 
**1. Introduction**

This project focuses on analyzing customer reviews of Tesla from 2024, scraped from Trustpilot.com (USA). The objective is to determine the sentiment behind these reviews and gain insights into customer satisfaction levels using Natural Language Processing (NLP) techniques.


 
**2. Objectives**

- Scrape Tesla customer reviews from Trustpilot.com (USA).

- Perform text preprocessing and sentiment analysis.

- Identify key topics in reviews using LDA topic modeling.

- Compute sentiment scores using RoBERTa.

- Analyze and categorize negative reviews to determine whether they relate to customer experience or car performance.

- Provide recommendations to Tesla based on findings.


 
**3. Data Collection**

- Source: Trustpilot.com (USA)

- Data Format: A dataset containing raw review texts.

- Tools Used: Python, BeautifulSoup/Scrapy for web scraping.


 
**4. Data Preprocessing**

- Convert text to lowercase.

- Remove punctuation, stopwords, extra spaces, and URLs.


 
**5. Exploratory Data Analysis (EDA)**

Common Words in Reviews
- The top 4 most common words in reviews were Tesla, Car, Service, and Customer.

 
Topic Modeling (LDA)
- The words customer and service appeared in the majority of the topics, indicating a strong focus on customer experience.


 
**6. Sentiment Analysis Methodology**

Sentiment Scoring
- Used RoBERTa to compute sentiment scores.

- Plotted sentiment distribution using a bar plot.

- Results: The majority of the reviews were negative.

Analysis of Negative Reviews

The key question: "Are the negative reviews about customer experiences or the car itself?"

Word Cloud and Bar Plots Analysis:

- Top Words in Negative Reviews: 'tesla', 'car', 'rattles', 'service'.

- Top Words in Positive Reviews: 'tesla', 'car', 'model', 'service'.

- 'Service' appears in both positive and negative reviews, requiring further analysis.


 
**7. Emotion Analysis (NRC Emotion Lexicon)**

Used NRC Emotion Lexicon to classify emotions in reviews.

- The results conflicted with the sentiment bar plot, indicating that NRC Lexicon may not be suitable for this dataset.



**8. Customer Experience vs. Car Performance Analysis**

Customer Service Issues
- 95% (121 out of 127 reviews) were negative about customer service.


Issues included:

- Lack of accessibility/communication from Tesla service centers.

- Customers' messages being ignored.

 
Car Service Issues

- A major case involved a customer’s daughter being injured due to an unresolved service issue.

- Other cases included complaints about car service failures.


 
**9. Tesla Model 3 Analysis**

The word "3" frequently appeared in negative reviews, indicating a need to analyze Tesla Model 3.

Bigram, Trigram, and Quadgram Analysis:

- Negative reviews included terms like "model 3", "park assist", and "performance".

- Positive reviews also mentioned "Model 3", suggesting mixed opinions.

 
**Key Findings**

Park Assist Issues:

- Malfunctioning sensors - The car did not beep when reversing near an object.

- Repeated failures - A customer experienced park assist issues three times.

Performance Concerns:

- No direct performance issues found.

- The word "Performance" mainly referred to Tesla Model X Performance or Model 3 Performance editions.

Rattle Issues:

- Three customers reported a rattling sound coming from their vehicles.


 
**10. Tools and Technologies Used**

- Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, NLTK, TextBlob, VADER, Gensim)

- BeautifulSoup/Scrapy for web scraping

- Hugging Face Transformers (RoBERTa) for sentiment analysis



**11. Challenges and Limitations**

- Possible scraping restrictions from Trustpilot.

- Bias in sentiment scoring due to dataset composition.

- NRC Emotion Lexicon did not align well with sentiment scores.


 
**12. Future Enhancements**

- Expand analysis across multiple review platforms.

- Implement real-time sentiment tracking.

- Fine-tune RoBERTa with a larger dataset for improved accuracy.


 
**13. Conclusion**

This project provides valuable insights into Tesla's customer sentiment in 2024. The analysis suggests that Tesla's customer service is a major issue, accounting for the majority of negative reviews. Additionally, Tesla Model 3 has mixed reviews, with concerns regarding Park Assist failures but no direct performance issues.


 
**14. Recommendations for Tesla**


Improve Customer Service:

- Enhance communication channels and responsiveness at service centers.

- Implement a more efficient ticketing/support system to track and resolve customer issues.
  


Address Park Assist Malfunctions:

- Investigate reported issues with the car sensors.

- Consider a software update or recall if necessary.

  

Investigate Rattle Issues:

- Conduct further testing on vehicles with reported rattling problems.

- Offer diagnostic services to affected customers.
  


Continue Monitoring Sentiment Trends:

- Regularly analyze customer reviews to identify and address new concerns.

- Use NLP-driven dashboards to track sentiment changes in real time.


 
By addressing these key concerns, Tesla can significantly improve customer satisfaction and mitigate negative feedback.
