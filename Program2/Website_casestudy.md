# Industry use cases for the Discrete Probability Distributions

### CASE 1:Manufacturing quality control - Analyze defective products on a production line. 

#### 1. Open the Binomial module in your Web application.
[Visit the Website](https://sharasunilkottari-pixel.github.io/SDAV_Lab/)\
On opening the web application the following screen for binomial distributions pops up.
<img width="1390" height="820" alt="image" src="https://github.com/user-attachments/assets/856c2719-4d54-4de0-aca5-82b9a0069d5f" />

#### 2. Enter n = 20 and p = 0.05.
We can set the values to n=20 and p=0.05.
<img width="1382" height="822" alt="image" src="https://github.com/user-attachments/assets/b33a3d2a-6610-47e6-9e9b-09b1059ae624" />

#### 3. Calculate the mean, variance, and probability of exactly 2 defects.
On clicking update. The values of mean and variance is found, and then by setting the value of k to 2 we can find the probability of exactly 2 defects.
<img width="1387" height="822" alt="image" src="https://github.com/user-attachments/assets/f54e402d-fa5d-4e81-ad0c-9991c6d1a663" />
<img width="1410" height="667" alt="image" src="https://github.com/user-attachments/assets/3ca98aa3-e078-4f41-9255-1be1664eaf2f" />
From the created website we find that the mean = 1,variance = 0.95 and P(X=2) = 0.18867680.

#### 4. View the PMF graph. The horizontal axis represents the number of defects and the vertical axis represents the probability of each count.
<img width="1372" height="532" alt="image" src="https://github.com/user-attachments/assets/81d39682-cc18-4ac6-9e8d-5bb2955561bd" />

#### 5. Change the defect probability from 0.05 to 0.10. Observe how the distribution shifts toward larger defect counts.
On changing the p value from 0.05 to 0.10 the graph changes to:
<img width="1372" height="530" alt="image" src="https://github.com/user-attachments/assets/4c694e5c-14c3-4b1c-9403-25b742a78109" />
We can observe that The probability mass function (PMF) shifts to the right as the expected number of defects doubles from 1 to 2. The distribution also spreads out more due to the higher variance.

#### 6. Open the Poisson module and enter λ = 5 for 100 inspected products. Compare the Poisson probabilities with the Binomial results.
<img width="1392" height="822" alt="image" src="https://github.com/user-attachments/assets/0f72e501-24f8-4b66-8508-65a8505d3df8" />
On comparing Binomial(100,0.05) and Poisson(5) for 100 inspections:
<img width="722" height="160" alt="image" src="https://github.com/user-attachments/assets/d87a1846-7ddf-4330-9f9c-a65f994ce0d9" />

#### 7. Open the Geometric module and enter p = 0.05. Examine the probability of detecting the first defect on different inspection attempts.
<img width="1392" height="832" alt="image" src="https://github.com/user-attachments/assets/6c2091e8-16f6-4fa0-9409-971c461aeb4a" />
<img width="1382" height="532" alt="image" src="https://github.com/user-attachments/assets/9a98db55-39d2-47c2-b5a7-72cf7bd884bf" />

Table with probability values:\
<img width="722" height="315" alt="image" src="https://github.com/user-attachments/assets/d3cd9345-c679-432e-9add-d69f7ce947a3" />

#### 8. Write down the numerical results, graph observations, and an inference about the quality-control process.
#### Numerical Results:
For Binomial Distribution with n=20 and p=0.05 and with n=100 and p=0.05 respectively,
<img width="727" height="180" alt="image" src="https://github.com/user-attachments/assets/4915d439-e99b-4038-b302-e31cbc096524" />
<img width="717" height="180" alt="image" src="https://github.com/user-attachments/assets/d7cf4c54-c075-40a6-bc9d-3cdaf281e004" />

For Poisson Distribution with λ=5,\
<img width="722" height="177" alt="image" src="https://github.com/user-attachments/assets/91772be7-c36c-4055-a146-e4e4dd563602" />

For Geometric Distribution with p=0.05,\
<img width="722" height="97" alt="image" src="https://github.com/user-attachments/assets/1e2629fd-fc98-4a9a-860d-f582e0aaff0e" />
<img width="722" height="315" alt="image" src="https://github.com/user-attachments/assets/d3cd9345-c679-432e-9add-d69f7ce947a3" />

#### Graph Observation:
Binomial PMF Shape (p = 0.05): \
A binomial distribution with p = 0.05 (a rare 5% defect rate) has this shape for three direct reasons:\
1.Positively Skewed (Right-Skewed): Because defects are rare, outcomes cluster near zero on the left, leaving a long, thin tail extending to the right toward higher defect counts.\
2.Peak at X = 1 (Mode): For moderate sample sizes (around n = 20 to 38), finding exactly 1 defective unit is the single most likely outcome. \
3.Rapid Tapering: Each extra defect requires multiplying by another 0.05. That penalty quickly overwhelms the combination count, causing the chance of seeing 3, 4, or more defects to collapse toward zero.

Shift on Increasing p (from 0.05 to 0.10):\
The shape of the PMF changes in two specific ways:\
1.Shift to the Right (Mean Doubles):The expected value is E[X] = np.\
~At p = 0.05: E[X] = 20 *0.05 = 1.\
~At p = 0.10: E[X] = 20 *0.10 = 2.\
Because the center of mass moves from 1 to 2, the peak (mode) shifts to the right toward higher defect counts.\
2.Wider Spread (Variance Increases):\
The variance formula is Var(X) = np(1 - p).\
~At p = 0.05: Var(X) = 20(0.05)(0.95) = 0.95. \
~At p = 0.10: Var(X) = 20(0.10)(0.90) = 1.80.\
Because the variance nearly doubles, the distribution becomes flatter and more dispersed across a wider range of possible defect values.

Poisson Approximation:\
<img width="1375" height="530" alt="image" src="https://github.com/user-attachments/assets/ac4c0709-b285-4f54-9288-79f06de0d140" />
Rate parameter λ=5:The mean is centred precisely at 5, marked by the dashed red line.\
Twin modes at X = 4 and X = 5:Both values share the highest probability at roughly 17.5%.\
Mild right skew:The bulk of events clusters between 2 and 8, with a thin tail stretching out toward 13 and beyond.\
Rare extremes:Getting 0 events or more than 11 events is very unlikely.

Geometric PMF Curve: \
The distribution is strictly monotonically decreasing, showing that the probability of encountering the first defect is highest on the very first few inspections and decays exponentially over subsequent trials.

#### Inference about the Quality-Control Process:
1.Defects per batch (Binomial):\
In a standard batch of 2$, finding 2 or fewer defects is highly likely (92.45%), confirming the batch will generally have low defect counts under normal operating conditions.   
2.Defect counts over high volumes (Poisson):\
For large continuous inspection lots, the Poisson model (λ=5) serves as an accurate, computationally efficient approximation of defect counts. 
3.Waiting time to a defect (Geometric):\
With an expected value of E[X] = 20, quality inspectors should expect to test an average of 20 products before uncovering the first defective item.  


### CASE 2:Cloud operations and cybersecurity monitoring 

#### 1. Enter the data: Use the monitoring table to identify the failure rate and average alert count.
From the 12 monitoring intervals (10-minute intervals each):\
-> Total API Requests: 1200\
-> Total Failed Requests: 27\
-> Total Security Alerts: 36\
Therefore,\
<img width="732" height="156" alt="image" src="https://github.com/user-attachments/assets/4f0b8feb-8093-4b15-8ed8-39abaf9f935c" />

#### 2. Select Binomial: Set n = 100 and p = 0.0225 . Calculate the probability of exactly 3 failures and view the PMF.
<img width="1390" height="492" alt="image" src="https://github.com/user-attachments/assets/9ba80edf-84a2-44df-97b0-77a5f60a6983" />
<img width="557" height="656" alt="image" src="https://github.com/user-attachments/assets/f3a5b801-de01-48f4-9327-2379a1691d5f" />
<img width="1371" height="532" alt="image" src="https://github.com/user-attachments/assets/9a3df390-86ba-4cae-ac7d-68d81d6cb69e" />

#### 3. Select Poisson: Set λ = 3. Calculate the probabilities of 0, 1, 2, 3, and higher alert counts. View the graph.
<img width="1382" height="647" alt="image" src="https://github.com/user-attachments/assets/cff4b458-3a69-4a6d-bc80-721652636323" />
Probability values,
<img width="726" height="210" alt="image" src="https://github.com/user-attachments/assets/9850337a-995d-46d3-b89a-891838dda491" />
<img width="1380" height="540" alt="image" src="https://github.com/user-attachments/assets/2abb308c-5cde-4cc6-973e-26358983fefa" />

#### 4. Experiment with A: Compare λ = 2, λ = 3, and λ = 5. Observe how the distribution shifts as the average alert count increases.
For λ=2,\
<img width="1380" height="535" alt="image" src="https://github.com/user-attachments/assets/f6bc6174-b71b-49d1-919b-a0d3cb8a088f" />
For λ=3,\
<img width="1380" height="540" alt="image" src="https://github.com/user-attachments/assets/a89a341c-612a-44b5-9cde-e26fa65cf13c" />
For λ=5,\
<img width="1377" height="542" alt="image" src="https://github.com/user-attachments/assets/38d91c26-a12b-495d-b234-0d2f49a0da1d" />

#### 5. Select Geometric: Set p = 0.8. Calculate the probability of success on the first, second, and third attempts.
<img width="1377" height="647" alt="image" src="https://github.com/user-attachments/assets/accc901a-a553-41cc-b8d2-799287b38f0f" />
Probability of success on the first, second, and third attempts,
<img width="720" height="100" alt="image" src="https://github.com/user-attachments/assets/9a5e55bf-432c-4a67-a6c1-148e8a8f49fc" />

#### 6. Interpret the results: Discuss whether the calculated probabilities could help the operations team plan monitoring thresholds, investigate failures, or evaluate retry policies.
1.Failure Anomaly Detection (Binomial):\
In a batch of 100 requests, seeing more than 5 or 6 failures has a negligible probability under baseline operations (p = 0.0225). If failures exceed this, an investigation should trigger immediately.\
2.Alert Thresholds (Poisson):\
Since observing 6 or more alerts in a 10-minute window has only an 8.4% probability under normal conditions, the operations team can set an automated alarm threshold at ≥6 or ≥7 alerts to minimize false positives while catching true anomalies.\
3.Retry Strategy Optimization (Geometric):\
Because 99.2% of requests resolve within 3 attempts, setting a hard cap of 2 to 3 retries avoids wasting server resources or contributing to retry storms during severe outages.
