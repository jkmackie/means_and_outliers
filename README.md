# means_and_outliers
**Build intuition for harmonic, geometric, and arithmetic means.**
***

We commonly summarize many numbers with a single number.  The number is often an average.  Different averages have different properties.  

We will discuss the arithmetic mean, geometric mean, and harmonic mean.  Each has a different sensitivity to outliers. And each has use cases.

The **arithmetic mean** is the "average" everyone is familiar with.  We have two numbers, 40 and 60:

`Arithmetic mean = (40 + 60) / 2 = 50`

The **geometric mean** is the nth root of numbers multiplied together, where n is how many numbers.

* `Geometric mean of 40, 60 = (40*60)^(1/2) = 48.9898 (rounded to four decimals)`

* `Geometric mean of 3, 5, 7, 40 = (3*5*7*40)^(1/4) = 8.0503 (rounded to four decimals)`

The **harmonic mean** is the **arithmetic mean** but with -1 powers inserted. Each number in the numerator gets -1 power.  Also, the numerator and denominator are placed in parenthesis and raised to the -1 power.  This is the same as flipping the `numerator/denominator` to `denominator/numerator`.

* `Harmonic mean of 40, 60 = ((40^-1+60^-1)/(2))^-1 = 2/(1/40 + 1/60)`

Harmonic mean in words:
* Write out arithmetic mean equation: (40 + 60) / 2; 
* Rewrite equation by putting the denominator as the numerator.  
* Each number in numerator is flipped and summed in the denominator inside parenthesis.

***
### Quality Ratings on Scales 1-5 and 1-10
Consider a contrived scenario where there are four different house quality ratings.  Only these ratings will be used to predict house price.  Kitchen, Basement, and House Quality are rated on a scale of 1-5 with 5 as the best.  Overall Quality is rated on a scale of 1-10 with 10 as the best.

Here are histograms of the ratings:

![Alt text](images/four_ratings.PNG)

We mix the 1-5 scale ratings together and view the histogram:

![Alt text](images/all_1_5_ratings_combined.PNG)

Since the scales are the same, the combined histogram also goes from 1-5.  Now, we mix in the Overall Quality ratings:

![Alt text](images/four_ratings_combined.PNG)

The histogram is right-skewed because the Overall Quality scale includes 6-10 and the other ratings do not.  If we pretend this set is [normally distributed](https://www.mathsisfun.com/data/standard-normal-distribution.html), the tails would be balanced.  Instead, the two little bars in the right tail look like outliers.  Ratings 9 and 10 in the set are over three standard deviations above the mean rating of 4.3.

### How are the means impacted by outliers?
