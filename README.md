# means_and_outliers
**Build intuition for harmonic, geometric, and arithmetic means.**
***

We commonly summarize lot of numbers with one number.  This number is often an average.  But, there are different averages.  We will focus on the arithmetic mean, geometric mean, and harmonic mean.  Each has a different sensitivity to outliers. And each has use cases.

The **arithmetic mean** is the "average" the general public is familiar with.  We have two numbers, 40 and 60:

`Arithmetic mean = (40 + 60) / 2 = 50`

The **geometric mean** is the nth root of numbers multiplied together, where n is how many numbers.

* `Geometric mean of 40, 60 = (40*60)^(1/2) = 48.9898 (rounded to four decimals)`

* `Geometric mean of 3, 5, 7, 40 = (3*5*7*40)^(1/4) = 8.0503 (rounded to four decimals)`

The **harmonic mean** is the **arithmetic mean** but with -1 powers inserted. Each number in the numerator gets -1 power.  Also, the numerator and denominator are placed in parenthesis and raised to the -1 power.  This is the same as flipping the `numerator/denominator` to `denominator/numerator`.

* `Harmonic mean of 40, 60 = ((40^-1+60^-1)/(2))^-1 = 2/(1/40 + 1/60)`

Harmonic mean in words:
* Write out arithmetic mean equation: (40 + 60) / 2; 
* Rewrite equation by putting the denominator as the numerator.  
* Each number in numerator is flipped and summed in the denominator inside parenthesis.`

### How are the means  impacted by outliers?
Let's consider a *contrived* case where there are four different house quality ratings.  Kitchen, Basement, and House Quality are rated on a scale of 1-5 with 5 as the best.  Overall quality is rated on a scale of 1-10 with 10 as the best.

Here are histograms of the ratings:

![Alt text](images/four_ratings.PNG)


my text

![Alt text](images/four_ratings_combined.PNG)


