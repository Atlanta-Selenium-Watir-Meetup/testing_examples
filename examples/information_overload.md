Information Overload 
================

### The Bad
Information you can almost never have too much of it, unless you do. this is an odd problem to have more often we have the exact opposite.  

Here are a few examples: 
  1. https://groups.google.com/d/msg/cukes/QZfmjvtd3DE/4Br6DOx0asYJ
  2. https://groups.google.com/d/msg/cukes/_hoLYeTNUvU/7IgD_1UjlikJ
  3. https://groups.google.com/d/msg/cukes/xW3bIjatnTk/M-6pxU6QdgkJ


### The Answer
I think a good test has just enough. and possibly is written in the domain's language and meant for the team so there is some level of knowledge is implied. 

### Example 1
Without knowing the whole scenario. or what we are actually trying to validate I can only guess. so my best guess would be we want to make sure that thru whatever mechanism we create tasks they are displayed in this table
I would personally keep the noise down since its not too important. the real important things seem like an "Admin" has tasks in his queue. since we dont really care what type of task or maybe we do how does this sound
   
    Given I have 4 tasks in progress
    When I view my task list
    Then I see all 4 tasks in my list

### Example 2
This to me looks a lot like implmentation language. [Getting the language right](https://skillsmatter.com/skillscasts/4307-richard-lawrence) was a great presentation/exercise on how to notice this. The exercise offers a great exercise on how to spot it and keep it out of your tests. 
