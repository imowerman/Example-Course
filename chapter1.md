---
title       : Chapter about something cool
description : This is what a chapter file looks like on DataCamp.<br>Add some awesome description here.
attachments :
  slides_link : https://s3.amazonaws.com/assets.datacamp.com/course/teach/slides_examle.pdf

--- type:VideoExercise lang:r xp:50 skills:1
## Analyze movie ratings


*** =video_link
//player.vimeo.com/video/108225030

--- type:MultipleChoiceExercise lang:r xp:50 skills:1
## Bad movie

function code goes between:

*** =instructions
- parenthesis
- curly brackets
- quotes
- nothing

*** =hint
too easy

*** =pre_exercise_code
```{r}


```

*** =sct
```{r}
msg_bad <- "That is not correct!"
msg_success <- "Exactly! There seems to be a very bad action movie in the dataset."

# We test the multiple choice exercise, and pass option 1 (- Action in the instructions) as the correct 
# choice. We also pass the test_mc() function a vector of characters to show the correct messages when 
# an answer is tried.
	
test_mc(correct = 1, feedback_msgs = c(msg_success, msg_bad, msg_bad, msg_bad, msg_bad)) 
```

--- type:NormalExercise lang:r xp:100 skills:1
## my second exercise

this is the instruction of the exercise...


*** =instructions
- Create a function that calculates the square root of x, and store it in an object called `sqrt2`
- Test the function on the vector `z` 

*** =hint
- the basic structure of a function is `object_name <- function(x){your code}`
- to test your function the code is as follows: `object_function_name(the object or value to be inputed)`

*** =pre_exercise_code
```{r}
# creating vector z

z <- c(1,3,9)

```

*** =sample_code
```{r}
# create your function, remember to store it in an object called sqrt2


# run your function on the vector z, which is pre-loaded

```

*** =solution
```{r}
# create your function, remember to store it in an object called sqrt2
sqrt2 <- function(x){x^.5}

# run your function on the vector z, which is pre-loaded
sqrt2(z)
```

*** =sct
```{r}
success_msg("Good work!")
```
