# Statistical Foundations

## Day 6 — Descriptive Statistics

### 1. Mean

Mean is the average of all values.

Formula:

Mean = Sum of values / Number of values

Example:

```python
marks = [10, 20, 30, 40, 50]
mean = sum(marks) / len(marks)
print(mean)
```

Result: 30.0

Mean can be strongly affected by extreme values (outliers).

---

## 2. Median

Median is the middle value after the data is sorted.

Example with an odd number of values:

10, 20, 30, 40, 50

Median = 30

For an even number of values, take the average of the two middle values.

10, 20, 30, 40

Median = 25

---

## 3. Mode

Mode is the value that appears most frequently.

Example:

10, 20, 20, 30, 40

Mode = 20

Python:

```python
from statistics import mode

data = [10, 20, 20, 30, 40]
print(mode(data))
```

---

## 4. Range

Range is the difference between the maximum and minimum values.

Range = Maximum - Minimum

Example:

10, 20, 30, 40, 50

Range = 40

Python:

```python
data = [10, 20, 30, 40, 50]
range_value = max(data) - min(data)
print(range_value)
```

---

## 5. Variance

Variance measures how spread out the observations are around the mean.

Basic idea:
1. Calculate the mean.
2. Find each value's difference from the mean.
3. Square those differences.
4. Calculate their average using the appropriate population or sample definition.

A larger variance generally means greater spread.

Example:

A = [49, 50, 51]
B = [10, 50, 90]

Both have mean 50, but B is more spread out, so B has higher variance.

---

## 6. Standard Deviation

Standard deviation measures the spread of data around the mean.

- Low standard deviation: values are relatively close to the mean.
- High standard deviation: values are more spread out.

Example:

Low spread: 48, 49, 50, 51, 52
High spread: 10, 30, 50, 70, 90

Standard deviation is expressed in the same units as the original data.

---

## 7. Mean vs Median and Outliers

Consider:

10, 20, 30, 40, 1000

Mean = 220
Median = 30

The large value 1000 pulls the mean upward. This shows why it is important to inspect the distribution and possible outliers instead of relying on one summary alone.

---

## 8. Central Tendency vs Variability

### Central Tendency
Describes the typical or central value:
- Mean
- Median
- Mode

### Variability / Spread
Describes how much the values differ:
- Range
- Variance
- Standard Deviation

---

## 9. Python Statistics Example

Python's statistics module provides common descriptive statistics:

```python
import statistics

data = [10, 20, 20, 30, 40]

print(statistics.mean(data))
print(statistics.median(data))
print(statistics.mode(data))
print(statistics.variance(data))
print(statistics.stdev(data))
```

The interpretation of variance and standard deviation depends on whether the data is treated as a sample or a population.

---

## Key Takeaway

Mean = Average
Median = Middle value
Mode = Most frequent value
Range = Maximum - Minimum
Variance = Measure of spread based on squared deviations
Standard Deviation = Typical spread around the mean

These concepts form the foundation of descriptive statistics and will be used later in exploratory data analysis and statistical inference.

---

**Day 6 Status: Complete**


## Day 7 — Percentiles, Probability & Correlation

### 1. Percentiles

A percentile describes the position of a value relative to the rest of the observations. For example, the 75th percentile is a value such that roughly 75% of observations are at or below it, depending on the percentile convention used.

### Percentage vs Percentile

- **Percentage** describes performance out of a possible total.
- **Percentile** describes relative position within a dataset.

For example, scoring 80 out of 100 gives 80%, but the corresponding percentile depends on how other observations are distributed.

### 2. Quartiles

Quartiles divide an ordered dataset into four parts.

- **Q1** = 25th percentile
- **Q2** = 50th percentile = Median
- **Q3** = 75th percentile

### 3. Probability

Probability measures the likelihood of an event.

Formula:

Probability = Favourable outcomes / Total outcomes

Probability is between 0 and 1.

Example:

For a fair coin:

P(Heads) = 1 / 2 = 0.5

### 4. Basic Probability Terms

- **Experiment:** A random process, such as tossing a coin.
- **Outcome:** A possible result, such as Heads.
- **Event:** One or more outcomes of interest.
- **Independent events:** One event does not change the outcome probabilities of another event.

### 5. Conditional Probability

Conditional probability measures the probability of an event given that another condition is known.

Notation:

P(A | B)

It is read as "probability of A given B."

### 6. Correlation

Correlation describes the direction and strength of a linear relationship between two numerical variables.

The correlation coefficient is commonly represented by `r` and ranges from -1 to +1.

- **r > 0:** Positive relationship
- **r < 0:** Negative relationship
- **r around 0:** Little or no linear relationship
- **r = +1:** Perfect positive linear relationship
- **r = -1:** Perfect negative linear relationship

### Examples

**Positive correlation:**
Study hours increase and marks generally increase.

**Negative correlation:**
Price increases and demand generally decreases.

**Weak or no clear correlation:**
Shoe size and exam marks.

### 7. Correlation Does Not Mean Causation

A correlation between two variables does not automatically prove that one variable causes the other.

For example, ice cream sales and swimming activity may both increase during hot weather. A third factor, such as temperature, can influence both.

### 8. Python Correlation Example

```python
import pandas as pd

data = {
    "study_hours": [1, 2, 3, 4, 5],
    "marks": [45, 50, 60, 70, 80]
}

df = pd.DataFrame(data)

print(df["study_hours"].corr(df["marks"]))
```

A positive value indicates a positive linear relationship in this example.

---

## Key Takeaway

**Percentile = Relative position**

**Quartile = Dataset divided into four parts**

**Probability = Likelihood of an event**

**Correlation = Direction and strength of linear relationship**

**Correlation is not proof of causation.**

---

**Day 7 Status: Complete ✅**
