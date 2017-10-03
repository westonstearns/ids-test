---
title                : R Basics 
description          : In this course we introduce you to the basics of computing and analyzing data in the user-friendly and helpful R interface. This first chapter starts with the very basics of functions, objects to get us acquainted with the world of R. 

---
## Using variables 1

```yaml
type: NormalExercise
lang: r
xp: 100
skills: 1
key: cf1ed0ec29
```

What is the sum of the first $n$ positive integers? 

We can use the formula $ n(n+1)/2 $ to quickly compute this quantity.


`@instructions`
- Define 'n=100'
- Then use R to compute the sum of 1 through 100 using the formula $ n(n+1)/2$. What is the sum?

`@hint`
- Define `n` to be 100 in one line and simply type the formula using R code in the second line.
- Remember that in R you multiply using `*`.

`@pre_exercise_code`
```{r}
# no pec
```

`@sample_code`
```{r}
# Here is how you compute the sum for the first 20 integers
20*(20+1)/2 

# However, we can define a variable to use the formula for other values of n
n <- 20
n*(n+1)/2

n <- 25
n*(n+1)/2

# Below, write your code to calculate the sum of the first 100 integers

```

`@solution`
```{r}
# Here is how you compute the sum for the first 20 integers
20*(20+1)/2 

# However, we can define a variable to use the formula for other values of n
n <- 20
n*(n+1)/2

n <- 25
n*(n+1)/2

# Below, write your code to calculate the sum of the first 100 integers 
n <- 100
n*(n+1)/2 
```

`@sct`
```{r}
# first instruction  
#test_object("n", incorrect_msg = "Make sure that you use `n` as your variable name and that you have assigned the correct value to `n`.")
#test_object("x", incorrect_msg = "Make sure that you use `n` as your variable name and that you have assigned the correct value to `n`.")
#test_output_contains ("12332424", incorrect_msg = "Take a look at your code for the second instruction.")
# General 
test_error() 
success_msg("Good job ! Let`s apply this to another question")
```
---
## Using variables 2

```yaml
type: NormalExercise
key: fd3f36c6ff
lang: r
xp: 100
skills: 1
```
What is the sum of the first $n$ positive integers? 

We can use the formula $ n(n+1)/2 $ to quickly compute this quantity.

`@instructions`
- Use the same formula as the last exercise but substitute `n`


`@hint`
Use the same R code as you used in the first question after changing the value of `n`.

`@pre_exercise_code`
```{r}
# no pec
```

`@sample_code`
```{r}
# Below, write you code to calculate the sum of the first 1000 integers 

```

`@solution`
```{r}
# Below, write you code to calculate the sum of the first 1000 integers 
n <- 1000
n*(n+1)/2
```

`@sct`
```{r}
# test n 
test_object("n", incorrect_msg = "Something is wrong with `n`. Make sure you have assigned the correct value to `n`.")

# test correct output
test_output_contains ("(n*(n+1)/2)", incorrect_msg = "Take a look at your code for the second instruction.")

# General 
test_error() 
success_msg("Good job ! Let`s get to work on another question!")
```
