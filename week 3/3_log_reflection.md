Oil B, Pulse C, Staple A, and Sweetener D all show increases from their first recorded price to their last recorded price. Staple A has the largest percentage increase among the items except for Sweetener D, which has the largest increase at 23.83%. Sweetener D's mean is much higher than its median, suggesting that the data are strongly affected by an unusually high observation. The 9999 value appears to be responsible for this difference because removing it brings the mean close to the median.

| AI claim | Colour | How I checked it | Result |
|---|---|---|---|
| All four items increased from first to last | 🟢 Green | Compared first and last prices | Accepted |
| Sweetener D increased by 23.83% | 🟢 Green | `(184.5-149)/149 × 100` | Accepted |
| Sweetener D has the largest percentage increase | 🟢 Green | Compared all four percentage changes | Accepted |
| Sweetener D's mean is much higher than its median | 🟢 Green | Compared 576.81 and 167.75 | Accepted |
| The 9999 observation causes the unusually high mean | 🟠 Amber | Compared statistics with and without 9999 | Accepted as an explanation, not a direct observation |
| The 9999 value is an actual data error | 🔴 Red | The dataset only tells us the value is 9999; it does not prove why it occurred | Rejected |

claims are reproducable 

##confused classmate

The mean is the arithmetic average of all the prices, but it can be strongly affected by an unusually large value. For Sweetener D, the mean is 576.81 PKR/kg because of the 9999 observation, while the median is 167.75 PKR/kg. When we remove 9999, the mean falls to 167.15 PKR/kg. So in this case, the median is closer to the typical prices in the dataset, but neither statistic tells us whether 9999 is actually an error.

##reflection 

My first draft went beyond what the data allowed when I treated the 9999 Sweetener D value as an error. The data clearly show that 9999 is an unusually large observation and that it has a major effect on the mean, but the dataset does not explain why that value occurred. I could therefore describe its effect on the statistics, but I should not claim that it was definitely entered incorrectly. This helped me distinguish between what I can directly observe in the data and what I am only suggesting as a possible explanation.
