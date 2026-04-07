## In-Class Activity: Typing Speed Regression ([lecture page](../../pages/mar26-regression-pt3.md), [slides](../../slides/18-regression-pt3.pdf))

![Lecture18-Simpson](../images/18-regression-pt3.jpg)

Load the typing speed data: [typingSpeed.csv](typingSpeed.csv)

### Part 1: Pooled Regression

Visualize the relationship between number of typos and typing speed. Run a regression analysis on the pooled data.

Interpret the analysis results.

### Part 2: Individual Patterns

The data is from 50 participants at 50 measurement occasions each.

Pick 5 random participants and plot their 50 measurement occasions in a joint plot using different colors or symbols. Interpret the data.

### Part 3: Two Sources of Variation

As we can see, we have two sources of variation that can be used to explain or predict the rate of errors:
1. Overall, faster typists make less mistakes (group-level pattern).
2. When typing faster, typists make more mistakes (individual-level pattern).

Model the typist as a fixed effect. Interpret the regression results.

### Part 4: Mixed Effects Model

Now fit a linear mixed model and see how we can detect both the within- and between-group patterns.

```r
library(lme4)
library(lmerTest)
lmer(typos ~ speed + (1 | participant))
```

### Part 5: Within- and Between-Group Effects

What if we want to capture both the within- and between-group patterns in a simple regression?

We can split our predictor (speed) into two variables, each representing a different source of variance:
- Each typist's average typing speed
- The deviation of each measurement from the typist's overall mean

Fit a simple linear model.

What happens if you fit a linear mixed model with a random intercept for participant?

---

### Solutions

- [Typing Speed Regression](typingSpeed.pdf)
- [Mixed Effects Models](mixedEffects.pdf)
