# **Poisson Distribution Model for Product Defects Analysis**

This project explores the **Poisson distribution** to model and analyse the number of defective products observed daily in a factory. Using a rate parameter (lambda) of 7 defects per day, the project delves into both theoretical probabilities and practical data generation to understand tThis project explores the **Poisson distribution** to model and analyse the number of defective products observed daily in a factory. Using a rate parameter (lambda) of 7 defects per day, the project delves into both theoretical probabilities and practical data generation to understand the distribution's behaviour.

## **Project Overview**
This repository contains a detailed analysis of defect occurrences in a factory, where defects are modeled using the **Poisson(7) distribution**. The project is divided into two sections:
1. **Theoretical Distribution Analysis**: This section computes probabilities using `scipy.stats.poisson` to answer key questions about the distribution.
2. **Practical Distribution Analysis**: Simulated data is generated to model 365 days (1 year) of defect observations, followed by a detailed comparison of observed data against theoretical expectations.

### **Key Objectives**
- **Understand the probability** of certain defect events (e.g., exactly 7 defects, fewer than 4 defects, more than 9 defects).
- **Generate a realistic dataset** of defects over the course of a year and compare it with theoretical expectations.
- **Analyze the frequency and severity** of defects over time, particularly focusing on bad days with high defect counts.
- **Determine percentile rankings** of defect occurrences and investigate extreme cases.

### **Dependencies:**
- Python 3.x
- `scipy` for statistical functions and distribution generation.
- `numpy` for numerical operations.

## **Theoretical Distribution Analysis**
1. **Probability of Exactly 7 Defects:**  
   The probability of observing exactly 7 defects (the expected number of defects) in a given day is calculated using the **Probability Mass Function (PMF)**.  
   - **Result:** ~14.9%

2. **Probability of 4 or Fewer Defects:**
   The **Cumulative Distribution Function (CDF)** is used to compute the probability of observing 4 or fewer defects.  
   - **Result:** ~17.3%

4. **Probability of More Than 9 Defects:**  
   To determine the likelihood of experiencing more than 9 defects (considered a bad day), the complement of the CDF is used.  
   - **Result:** ~16.9%

## **Practical Distribution Analysis**
A dataset of 365 days is simulated, where each day represents the number of defects observed using a Poisson distribution with λ = 7. The results are then analyzed in the following ways:

1. **Simulated Defect Data**:  
   A dataset (`year_defects`) is created, containing random values generated from the Poisson(7) distribution. The first 20 values of the dataset are shown as:  
   - `[10, 7, 8, 5, 12, 8, 6, 7, 4, 14, 3, 7, 5, 9, 3, 7, 2, 12, 3, 7]`.

2. **Expected vs. Actual Defects Over a Year**:  
   The expected total number of defects over 365 days is computed as `2555`, while the actual sum of the simulated defects is `2664`.


3. **Average Number of Defects**:  
   The observed average from the dataset is `7.3`, close to the theoretical average of 7 defects/day.

4. **Maximum Number of Defects in a Day**:  
   The maximum number of defects observed in a single day was `16`, which represents a rare, hectic day.

5. **Probability of Observing 16 or More Defects**:  
   The probability of seeing 16 or more defects on a given day is calculated to be `0.00096`, highlighting its rarity.

6. **90th Percentile for Defects**:  
   In 90% of the days, fewer than `10` defects are expected. Days with 10 or more defects fall in the top 10% of the distribution.

7. **Proportion of Days in the 90th Percentile**:  
   Approximately `13.15%` of the days in the simulated dataset recorded defects greater than or equal to 10, slightly above the theoretical expectation due to random variation.

## **Conclusion**
This project provided valuable insights into the **Poisson(7) distribution**, highlighting its effectiveness in modeling rare events such as product defects in a factory setting. The combination of theoretical analysis and practical simulations demonstrates how the distribution behaves in both predictable and unpredictable ways.

he distribution's behaviour.

## **Project Overview**
This repository contains a detailed analysis of defect occurrences in a factory, where defects are modeled using the **Poisson(7) distribution**. The project is divided into two sections:
1. **Theoretical Distribution Analysis**: This section computes probabilities using `scipy.stats.poisson` to answer key questions about the distribution.
2. **Practical Distribution Analysis**: Simulated data is generated to model 365 days of defect observations, followed by a detailed comparison of observed data against theoretical expectations.

### **Key Objectives**
- **Understand the probability** of certain defect events (e.g., exactly 7 defects, fewer than 4 defects, more than 9 defects).
- **Generate a realistic dataset** of defects over the course of a year and compare it with theoretical expectations.
- **Analyze the frequency and severity** of defects over time, particularly focusing on bad days with high defect counts.
- **Determine percentile rankings** of defect occurrences and investigate extreme cases.

### **Dependencies:**
- Python 3.x
- `scipy` for statistical functions and distribution generation.
- `numpy` for numerical operations.


## **Theoretical Distribution Analysis**
1. **Probability of Exactly 7 Defects:**  
   The probability of observing exactly 7 defects (the expected number of defects) in a given day is calculated using the **Probability Mass Function (PMF)**.  
   - **Result:** ~14.9%

2. **Probability of 4 or Fewer Defects:**  
   The **Cumulative Distribution Function (CDF)** is used to compute the probability of observing 4 or fewer defects.  
   - **Result:** ~17.3%

3. **Probability of More Than 9 Defects:**  
   To determine the likelihood of experiencing more than 9 defects (considered a bad day), the complement of the CDF is used.  
   - **Result:** ~16.9%

## **Practical Distribution Analysis**
A dataset of 365 days is simulated, where each day represents the number of defects observed using a Poisson distribution with λ = 7. The results are then analyzed in the following ways:

1. **Simulated Defect Data**:  
   A dataset (`year_defects`) is created, containing random values generated from the Poisson(7) distribution. The first 20 values of the dataset are shown as:  
   - `[10, 7, 8, 5, 12, 8, 6, 7, 4, 14, 3, 7, 5, 9, 3, 7, 2, 12, 3, 7]`.

2. **Expected vs. Actual Defects Over a Year**:  
   The expected total number of defects over 365 days is computed as `2555`, while the actual sum of the simulated defects is `2664`.


3. **Average Number of Defects**:  
   The observed average from the dataset is `7.3`, close to the theoretical average of 7 defects/day.

4. **Maximum Number of Defects in a Day**:  
   The maximum number of defects observed in a single day was `16`, which represents a rare, hectic day.

5. **Probability of Observing 16 or More Defects**:  
   The probability of seeing 16 or more defects on a given day is calculated to be `0.00096`, highlighting its rarity.

6. **90th Percentile for Defects**:  
   In 90% of the days, fewer than `10` defects are expected. Days with 10 or more defects fall in the top 10% of the distribution.

7. **Proportion of Days in the 90th Percentile**:  
   Approximately `13.15%` of the days in the simulated dataset recorded defects greater than or equal to 10, slightly above the theoretical expectation due to random variation.

## **Conclusion**
This project provided valuable insights into the **Poisson(7) distribution**, highlighting its effectiveness in modeling rare events such as product defects in a factory setting. The combination of theoretical analysis and practical simulations demonstrates how the distribution behaves in both predictable and unpredictable ways.

The Poisson distribution provides a valuable tool for modeling the number of product defects in this scenario. By understanding the distribution's characteristics and simulating data, we can gain insights into expected defect rates, their variability, and the probability of observing extreme events. These insights can be used to improve quality control processes and reduce the occurrence of defects.

