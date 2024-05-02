# -Big-Data-Solutions-for-Combating-Financial-Fraud

**Team Members: ** Rajashree Ramaprabu, Riris Grace Karolina, Yu-Fang(Unice) Liao, Ya Chu Hsu, Yi Cheng Chung

## Report Summary 

Our project delves into a thorough analysis of transactional and laundering activities across a multitude of currencies, offering insights into the intricate dynamics of illicit financial operations and their broader implications.

In our analysis, we unearthed intriguing patterns indicative of money laundering practices across various currencies. The noteworthy dominance of the US Dollar and Euro in both total transactions and laundering activities suggests a preference for these currencies in facilitating illicit financial flows, owing to their global prominence and liquidity. Additionally, our identification of recurrent bank codes associated with laundering activities underscores the critical role of regulatory compliance and financial intelligence in combating financial crimes.

Furthermore, our observation that most laundering transactions involve a single currency highlights the significance of currency stability and liquidity in facilitating illicit transactions. Moreover, the slight inclination towards currency conversion within laundering cycles hints at the adaptability of money laundering schemes. Similarly, the average duration of a laundering cycle per day sheds light on the operational intricacies of laundering schemes and underscores the importance of continuous monitoring and regulatory oversight.
Our visualizations, particularly the 'Laundering Amount Over Time' chart, provide valuable insights into the temporal dynamics of laundering activities, aligning with theories of financial crime and market volatility. Furthermore, our analysis of the distribution of laundering patterns within a cycle highlights the multifaceted nature of money laundering techniques employed by criminal networks.
Overall, our findings contribute to the theoretical discourse on financial crime prevention and underscore the pressing need for robust regulatory frameworks and enforcement mechanisms to combat illicit financial activities effectively.

## Table of Contents

Business Problem Definition
Data Source Brief Summary
Data Preparation & Cleaning
Exploratory Data Analysis (EDA)
Data Analysis
Data Visualization
Key Findings & Conclusion
References
Generative AI Disclosure

## Business Problem Definition

In the fight against financial fraud, predicting fraudulent transactions within massive datasets is crucial. Our project aims to leverage advanced analytics and big data techniques to identify patterns of money laundering within a comprehensive synthetic financial transaction dataset provided by IBM. 
Below are our objectives:

- Analyze synthetic transaction data and identify patterns indicative of fraud.
- Investigate correlations between transaction features such as amount, currency, and payment format that are most frequently associated with detecting potential money laundering
- Analyze temporal patterns, including transaction volume spikes, to identify potential instances of money laundering activities over time.

The proliferation of financial crimes, including money laundering, poses significant threats to both financial institutions and society at large. Financial fraud not only results in substantial economic losses but also undermines the integrity of financial systems and erodes public trust. As criminals continuously adapt their tactics to exploit vulnerabilities in traditional detection methods, there is an urgent need for innovative approaches to combat these illicit activities.

By leveraging advanced analytics and big data techniques to analyze vast amounts of transaction data, our project seeks to stay ahead of evolving fraud schemes and enhance the effectiveness of detection efforts. Identifying patterns indicative of fraud within massive datasets is crucial for preemptively flagging suspicious activities and preventing financial losses. Furthermore, understanding correlations between transaction features and detecting potential money laundering can provide valuable insights for refining risk assessment models and strengthening regulatory compliance measures.
Moreover, analyzing temporal patterns, including transaction volume spikes, enables us to uncover subtle indicators of money laundering activities that may evade traditional detection methods. Detecting and disrupting these illicit activities in real-time not only mitigates financial risks for institutions but also contributes to broader efforts to combat organized crime, terrorism financing, and other illicit activities that exploit the financial system for nefarious purposes.

Overall, our project aims to contribute to the ongoing fight against financial fraud by leveraging cutting-edge analytics and big data techniques to identify and disrupt patterns of money laundering. By doing so, we not only protect the integrity of financial markets but also uphold the principles of transparency, accountability, and trust that underpin a healthy and resilient financial ecosystem.

## Data Source Brief Summary

The data source consists of Anti-Money Laundering (AML) Public Data owned by IBM and exchange rate data from the Treasury Report of Exchange. 
The data tables are as follows:
1. Transactions for AML (https://ibm.ent.box.com/v/AML-Anti-Money-Laundering-Data/folder/132399911119)
    It consists of 11 columns and 190 million rows, with the column types varying among string, categorical, and numeric data.
    
    a. Table 1: Group HI has a relatively higher illicit ratio, indicating more money laundering activities.    
    b. Table 2: Group LI has a relatively lower illicit ratio, indicating less money laundering activities.     
    c. Table 3: Pattern table, which contains the results of identifying suspected money laundering transactions, types of money laundering, and the information indicating that the transactions outlined the sequence of activities suspected to be involved in money laundering.
    
2. Exchange Rate: (https://fiscaldata.treasury.gov/datasets/treasury-reporting-rates-exchange/treasury-reporting-rates-of-exchange)
    The dataset consists of the exchange rates of the U.S. government against various currencies over a period of 10 years. It contains one table with 13 columns and 173 rows.

## Future Improvement

For future improvement in the detection and analysis of money laundering, integrating additional data sources could provide significant benefits. Incorporating diverse data such as real-time transaction feeds, geographic information, and external watchlists could enrich the analysis, allowing for the identification of nuanced patterns and correlations not visible through transaction data alone. Furthermore, experimenting with advanced machine learning models, including ensemble methods, deep learning networks, or anomaly detection systems, could enhance detection rates and reduce false positives. Expanding the temporal analysis to cover longer periods and conducting comparative year-over-year reviews might also yield insights into long-term trends and help predict future laundering activities based on past patterns. Moreover, developing a collaborative framework where multiple financial institutions can share insights and data, while respecting privacy norms, would lead to a more comprehensive view of money laundering tactics. Lastly, continuously updating analysis techniques to align with new regulatory requirements and emerging financial instruments, like cryptocurrencies, can help stay ahead of launderers who adapt quickly to the changing financial landscape.

## Conclusion

This comprehensive analysis of money laundering transactions using big data analytics has illuminated several key aspects of financial fraud. Our findings emphasize the importance of transaction timing and methods of currency conversion as crucial elements in laundering schemes. Notably, peak periods for laundering activities were identified, providing critical insights for financial institutions to enhance their monitoring systems during these times. Our study also uncovered the predominance of certain currencies and transaction methods in laundering processes, with the USD and Euro being particularly prominent due to their global acceptance and ease of use in large-scale transactions. Furthermore, sophisticated laundering patterns like "Scatter-Gather" and "Cycle" typologies were prevalent, indicating that launderers employ complex strategies to evade detection. The use of machine learning models aimed to enhance detection capabilities, though challenges like data imbalance limited the effectiveness of our initial models. However, the insights gained pave the way for further refining these models and incorporating advanced analytical tools. Moving forward, building on these insights will be crucial. By implementing the suggested improvements and integrating broader data sets, we can develop more robust defenses against money laundering. This endeavor will not only help protect the integrity of financial systems but also contribute to a broader understanding of financial crimes and their prevention mechanisms. These efforts represent a step toward a more secure and transparent financial environment, highlighting the pivotal role of data analytics in combating financial fraud.

## Reference
1. In-class exercise: https://github.com/soltaniehha/Big-Data-Analytics-for-Business/blob/master/08-EDA-and-Data-Sources/01-EDA.ipynb
2. Save the temporary file: https://stackoverflow.com/questions/51628958/spark-savewrite-parquet-only-one-file
3. Read parquet file: https://spark.apache.org/docs/latest/sql-data-sources-parquet.html
4. Functions for extracting time: https://stackoverflow.com/questions/73034490/extracting-day-week-hour-date-year-in-pyspark-from-a-string-column
5. Rename column name: https://spark.apache.org/docs/latest/api/python/reference/pyspark.sql/api/pyspark.sql.DataFrame.withColumnRenamed.html
6. Functions for extracting time (PySpark official document): https://spark.apache.org/docs/latest/api/python/reference/pyspark.sql/api/pyspark.sql.functions.dayofweek.html
7. Violine plot: https://seaborn.pydata.org/generated/seaborn.violinplot.html
8. Formatting SQL result values: https://stackoverflow.com/questions/54260352/how-to-show-a-column-in-a-pyspark-dataframe-in-the-scientific-notation-with-prop
9. SQL Recursive funtion: https://learnsql.com/blog/sql-recursive-cte/
10. SQL Categorical function: https://pandas.pydata.org/docs/reference/api/pandas.Categorical.html

## Generative AI Disclosure

We used ChatGPT for debugging codes, understand and explore visualization options in PySpark and text refinement.
1. Code for mapping the column names between the two dataframes, from ChatGPT
2. Plot the violin chart, from ChatGPT
3. Used to help in graph 11 for aligning values in individual axis.
4. Used for understanding the different network graphs that can be used.
5. Refine the code for finding transactions that might be frauduleng in cycle type.

