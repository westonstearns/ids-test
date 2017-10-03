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
key: 2712a22151
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