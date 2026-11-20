| Item | Mean | Median | Mean - median | First-to-last change|
|---|---|---|---|---|
| Oil B | 324.83 | 324.00 | 0.83 | +15.3% |
| Pulse C | 205.91 | 206.00 | -0.09 | +3.1% |
| Staple A | 111.26 | 112.50 | -1.24 | +13.0% |
| Sweetener D | 167.15 | 167.50 | -0.35 | +19.4% |

I would report the median for all items as it is less likely to be affected by an outlier.

# With and without a flagged value (Sweetener D)

| | n | Mean | Median |
|---|---|---|---|
| With the 9999 entry | 24 | 576.81 | 167.75 |
| Without it | 23 | 167.15 | 167.50 |
| Difference | | 409.66 | 0.25 | 

It has an unusual value which affects it greatly. 

#Referee's Note: 

O: Sweetener D has a mean price of 576.81 PKR/kg and a median price of 167.75 PKR/kg.


O: The mean is much higher than the median for Sweetener D.


O: The dataset contains a Sweetener D price of 9999 PKR/kg, while the other Sweetener D prices are much lower.


E: The unusually high mean is likely caused by the 9999 PKR/kg observation.


O: When the 9999 value is removed, the mean falls to 167.15 PKR/kg and the median becomes 167.50 PKR/kg.


E: This suggests that the median gives a more typical description of the Sweetener D prices in this dataset.
