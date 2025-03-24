# Natural Language Processing with Hotel Data 🏨
This exercise aimed to provide valuable, data-derived insights to the following hotel review data to a fictitious Hotel Management Inc. who wish to understand what qualities of a hotel stay contribute to greater customer satisfaction and higher ratings. As the Data Scientist, I was responsible to data processing and data modelling using a large hotel review dataset. The following work and results are a sample of the hotel review analysis with my technical skills.

## Table of Contents
- [Data](#data)
- [Work](#work)
- [Results](#results)
- [Future Considerations](#future-considerations)

---

<a id="data"></a>
### Data :books:
The data was originally sourced from <a href="https://www.kaggle.com/datasets/jiashenliu/515k-hotel-reviews-data-in-europe" target="_blank">Kaggle</a>. 

The data consisted of one table containing hotel information.  

**Table: hotel_reviews**
|Column Name| Description|
|---|---|
|`Hotel_Address`|Address of hotel|
|`Review_Date`|Date when reviewer posted the corresponding review|
|`Average_Score`|Average Score of the hotel, calculated based on the latest comment in the last year|
|`Hotel_Name`|Name of Hotel|
|`Reviewer_Nationality`|Nationality of Reviewer|
|`Negative_Review`|Negative Review the reviewer gave to the hotel. If the reviewer does not give the negative review, then it should be: 'No Negative'|
|`Review_Total_Negative_Word_Counts`|Total number of words in the negative review|
|`Positive_Review`|Positive Review the reviewer gave to the hotel. If the reviewer does not give the negative review, then it should be: 'No Positive'|
|`Review_Total_Positive_Word_Counts`|Total number of words in the positive review|
|`Reviewer_Score`|Score the reviewer has given to the hotel, based on his/her experience|
|`Total_Number_of_Reviews_Reviewer_Has_Given`|Number of Reviews the reviewers has given in the past|
|`Total_Number_of_Reviews`|Total number of valid reviews the hotel has|
|`Tags`|Tags reviewer gave the hotel|
|`days_since_review`|Duration between the review date and scrape date|
|`Additional_Number_of_Scoring`|There are also some guests who just made a scoring on the service rather than a review. This number indicates how many valid scores without review in there|
|`lat`|Latitude of the hotel|
|`lng`|longtitude of the hotel|

---

<a id="work"></a>
### Work :bar_chart:

Using Python, the following sample question was answered.

**Modelling**

Fit a logistic regression model on the data and analyze the test and train accuracy. Find the top 20 words from the positive reviews that are most predictive of a positive sentiment (Reviewer_Score = 1). Similarly, find the top 20 words from the negative reviews that are most predictive of a negative sentiment (Reviewer_Score = 0). What actionable insights can you draw from these?

---

<a id="results"></a>
### Results :eyes:

**Modelling**

![image](https://github.com/user-attachments/assets/5a3d11a2-cd91-439f-b788-53b96e9d1e81)

![image](https://github.com/user-attachments/assets/dbe89247-1c21-4e18-82c5-b999bb01c853)

From Positive Reviews
- Words such as "pos_comfort","pos_luxurious",and "pos_class" suggest that customers value high quality in their hotel experience. Customers like to feel pampered in their hotel.
- Words such as "pos_attention","pos_brilliant",and "pos_exceptionally" suggest that customers felt that the hotel service was above their expectations. Customers want service in things they would not have considered but find value in it. An example is giving free toiletries in items not found in other hotels. 

From Negative Reviews
- Words such as "complain","issue",and "fault" suggest irritation and disappointment in hotel's customer service or quality.  
- Words such as "slightly","minor",and "fine" suggest that customers felt that the hotel service was below their expectations. The hotel's service need to address quality concerns. 

--- 

<a id="future-considerations"></a>
**Future Considerations**
- Explore other models and hyperparameters such as PCA with a decision tree classifier to find the best-performing model   
- Conduct a more in-depth evaluation by analyzing the confusion matrix to review model errors 

Thanks for reading! 🏨
