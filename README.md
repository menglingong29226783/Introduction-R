# Introduction-R
Introduction R from datacamp

Chapter 1
1 Intro to basics
How it works
In the editor on the right you should type R code to solve the exercises. When you hit the 'Submit Answer' button, every line of code is interpreted and executed by R and you get a message whether or not your code was correct. The output of your R code is shown in the console in the lower right corner.
R makes use of the # sign to add comments, so that you and others can understand what the R code is about. Just like Twitter! Comments are not run as R code, so they will not influence your result. For example, Calculate 3 + 4 in the editor on the right is a comment.
You can also execute R commands straight in the console. This is a good way to experiment with R code, as your submission is not checked for correctness.
Instructions
100 XP
•	In the editor on the right there is already some sample code. Can you see which lines are actual R code and which are comments?
•	Add a line of code that calculates the sum of 6 and 12, and hit the 'Submit Answer' button.
Take Hint (-30 XP)

# Calculate 3 + 4
3 + 4
3+4
# Calculate 6 + 12
6+12

Arithmetic with R
变量的数学加减乘除求余运算。
In its most basic form, R can be used as a simple calculator. Consider the following arithmetic operators:
•	Addition: +
•	Subtraction: -
•	Multiplication: *
•	Division: /
•	Exponentiation: ^
•	Modulo: %%
•	
•	加Addition: +
•	减Subtraction: -
•	乘Multiplication: *
•	除Division: /
•	加平方Exponentiation: ^
•	Modulo: %%
•	
The last two might need some explaining:
•	The ^ operator raises the number to its left to the power of the number to its right: for example 3^2 is 9.
•	The modulo returns the remainder of the division of the number to the left by the number on its right, for example 5 modulo 3 or 5 %% 3 is 2.
With this knowledge, follow the instructions below to complete the exercise.
Instructions
100 XP
•	Type 2^5 in the editor to calculate 2 to the power 5.
•	Type 28 %% 6 to calculate 28 modulo 6.
•	Click 'Submit Answer' and have a look at the R output in the console.
•	Note how the # symbol is used to add comments on the R code.
Take Hint (-30 XP)

# An addition
5 + 5 
5+5
# A subtraction
5 - 5 
5-5
# A multiplication
3 * 5
3*5
 # A division
(5 + 5) / 2 
(5+5)/2
# Exponentiation
2^5

# Modulo
28%%6

Variable assignment
A basic concept in (statistical) programming is called a variable. 

A basic concept in (statistical) programming is called a variable. 
概念：变量（variable）

A variable allows you to store a value (e.g. 4) or an object (e.g. a function description) in R. You can then later use this variable's name to easily access the value or the object that is stored within this variable.
You can assign a value 4 to a variable my_var with the command
my_var <- 4
Instructions
100 XP
Over to you: complete the code in the editor such that it assigns the value 42 to the variable x in the editor. Click 'Submit Answer'. Notice that when you ask R to print x, the value 42 appears.
Take Hint (-30 XP)

# Assign the value 42 to x
x <- 42
my_var<-42
# Print out the value of the variable x
X

Variable assignment (2)
Suppose you have a fruit basket with five apples. As a data analyst in training, you want to store the number of apples in a variable with the name my_apples.
Instructions
100 XP
•	Type the following code in the editor: my_apples <- 5. This will assign the value 5 to my_apples.
•	Type: my_apples below the second comment. This will print out the value of my_apples.
•	Click 'Submit Answer', and look at the console: you see that the number 5 is printed. So R now links the variable my_apples to the value 5.
Take Hint (-30 XP)

# Assign the value 5 to the variable my_apples
my_apples<-5

# Print out the value of the variable my_apples
my_apples

输出数据的运算叫做print(my_apples)
或者直接输入变量名
my_apples

Variable assignment (3)
Every tasty fruit basket needs oranges, so you decide to add six oranges. As a data analyst, your reflex is to immediately create the variable my_oranges and assign the value 6 to it. Next, you want to calculate how many pieces of fruit you have in total. Since you have given meaningful names to these values, you can now code this in a clear way:
my_apples + my_oranges
Instructions
100 XP
•	Assign to my_oranges the value 6.
•	Add the variables my_apples and my_oranges and have R simply print the result.
•	Assign the result of adding my_apples and my_oranges to a new variable my_fruit.
Take Hint (-30 XP)

# Assign a value to the variables my_apples and my_oranges
my_apples <- 5
my_oranges<-6

# Add these two variables together
my_apples + my_oranges

# Create the variable my_fruit
my_fruit=my_apples + my_oranges
my_fruit

Apples and oranges
Common knowledge tells you not to add apples and oranges. But hey, that is what you just did, no :-)? The my_apples and my_oranges variables both contained a number in the previous exercise. The + operator works with numeric variables in R. If you really tried to add "apples" and "oranges", and assigned a text value to the variable my_oranges (see the editor), you would be trying to assign the addition of a numeric and a character variable to the variable my_fruit. This is not possible.
Instructions
100 XP
•	Click 'Submit Answer' and read the error message. Make sure to understand why this did not work.
•	Adjust the code so that R knows you have 6 oranges and thus a fruit basket with 11 pieces of fruit.
Take Hint (-30 XP)

# Assign a value to the variable my_apples
my_apples <- 5 

# Fix the assignment of my_oranges
my_oranges <- "six" 
my_oranges <- 6
# Create the variable my_fruit and print it out
my_fruit <- my_apples + my_oranges 
my_fruit= my_apples + my_oranges
my_fruit

输出数据的运算叫做print(my_fruit)
或者直接输入变量名
my_fruit

Basic data types in R
R works with numerous data types. Some of the most basic types to get started are:
•	Decimal values like 4.5 are called numerics. 
•	（数值型数据(numerics)可以含有小数位浮点。）
•	Natural numbers like 4 are called integers. Integers are also numerics. 
•	（整数型数据(integers)也算是数值型数据的一种作为不含有小数位浮点的数据。）
•	Boolean values (TRUE or FALSE) are called logical.
•	（逻辑型数据（logical /Boolean values）只有两种，真或假）
•	Text (or string) values are called characters.
•	（文本型数据（characters /Text (or string) values）注意赋值录入的时候需要加引号）
Note how the quotation marks on the right indicate that "some text" is a character.
Instructions
100 XP
Change the value of the:
•	my_numeric variable to 42.
•	my_character variable to "universe". Note that the quotation marks indicate that "universe" is a character.
•	my_logical variable to FALSE.
Note that R is case sensitive!
Take Hint (-30 XP)

# Change my_numeric to be 42
my_numeric <- 42.5
my_numeric=my_numeric-0.5
# Change my_character to be "universe"
my_character <- "some text"
my_character <- "universe"
# Change my_logical to be FALSE
my_logical <- TRUE
my_logical <- FALSE

What's that data type?
Do you remember that when you added 5 + "six", you got an error due to a mismatch in data types? You can avoid such embarrassing situations by checking the data type of a variable beforehand. You can do this with the class() function, as the code on the right shows.
You can do this with the class() function
(Class函数:用来check目标变量variables的数据类型，数字型数据/文字型数据/真伪型数据（Bloomberg值）)
Instructions
100 XP
Complete the code in the editor and also print out the classes of my_character and my_logical.
Take Hint (-30 XP)

# Declare variables of different types
my_numeric <- 42
my_character <- "universe"
my_logical <- FALSE 

# Check class of my_numeric
class(my_numeric)

# Check class of my_character
class(my_character)

# Check class of my_logical
class(my_logical)


 
Chapter 2
Vectors

Create a vector
Feeling lucky? You better, because this chapter takes you on a trip to the City of Sins, also known as Statisticians Paradise!
Thanks to R and your new data-analytical skills, you will learn how to uplift your performance at the tables and fire off your career as a professional gambler. This chapter will show how you can easily keep track of your betting progress and how you can do some simple analyses on past actions. Next stop, Vegas Baby... VEGAS!!
Instructions
100 XP
•	Do you still remember what you have learned in the first chapter? Assign the value "Go!" to the variable vegas. Remember: R is case sensitive!
Take Hint (-30 XP)

# Define the variable vegas
vegas <- 'Go!'
（加引号对变量进行赋值）
Create a vector (2)
( vector矢量)
Let us focus first!
On your way from rags to riches, you will make extensive use of vectors. Vectors are one-dimension arrays that can hold numeric data, character data, or logical data. In other words, a vector is a simple tool to store data. For example, you can store your daily gains and losses in the casinos.
In R, you create a vector with the combine function c().
在R语言中，我们使用c()函数来创建一个矢量
In R, you create a vector with the combine function c(). You place the vector elements separated by a comma between the parentheses. For example:
numeric_vector <- c(1, 2, 3)
character_vector <- c("a", "b", "c")
Once you have created these vectors in R, you can use them to do calculations.
Instructions
100 XP
Complete the code such that boolean_vector contains the three elements: TRUE, FALSE and TRUE (in that order).
Take Hint (-30 XP)

numeric_vector <- c(1, 10, 49)
character_vector <- c("a", "b", "c")

# Complete the code for boolean_vector
boolean_vector <-c(TRUE, FALSE, TRUE)

Create a vector (3)
After one week in Las Vegas and still zero Ferraris in your garage, you decide that it is time to start using your data analytical superpowers.
Before doing a first analysis, you decide to first collect all the winnings and losses for the last week:
For poker_vector:
•	On Monday you won $140
•	Tuesday you lost $50
•	Wednesday you won $20
•	Thursday you lost $120
•	Friday you won $240
For roulette_vector:
•	On Monday you lost $24
•	Tuesday you lost $50
•	Wednesday you won $100
•	Thursday you lost $350
•	Friday you won $10
You only played poker and roulette, since there was a delegation of mediums that occupied the craps tables. To be able to use this data in R, you decide to create the variables poker_vector and roulette_vector.
Instructions
100 XP
Assign the winnings/losses for roulette to the variable roulette_vector.
Take Hint (-30 XP)

# Poker winnings from Monday to Friday
poker_vector <- c(140, -50, 20, -120, 240)

# Roulette winnings from Monday to Friday
roulette_vector <-  c(-24,-50,100,-350,10)

Naming a vector
As a data analyst, it is important to have a clear view on the data that you are using. Understanding what each element refers to is therefore essential.
In the previous exercise, we created a vector with your winnings over the week. Each vector element refers to a day of the week but it is hard to tell which element belongs to which day. It would be nice if you could show that in the vector itself.
You can give a name to the elements of a vector with the names() function. Have a look at this example:
some_vector <- c("John Doe", "poker player")
names(some_vector) <- c("Name", "Profession")
This code first creates a vector some_vector and then gives the two elements a name. The first element is assigned the name Name, while the second element is labeled Profession. Printing the contents to the console yields following output:
          Name     Profession 
    "John Doe" "poker player" 
Instructions
100 XP
•	The code on the right names the elements in poker_vector with the days of the week. Add code to do the same thing for roulette_vector.
Take Hint (-30 XP)

# Poker winnings from Monday to Friday
poker_vector <- c(140, -50, 20, -120, 240)

# Roulette winnings from Monday to Friday
roulette_vector <- c(-24, -50, 100, -350, 10)

# Assign days as names of poker_vector
names(poker_vector) <- c("Monday", "Tuesday", "Wednesday", "Thursday", "Friday")

# Assign days as names of roulette_vector
names(roulette_vector) <- c("Monday", "Tuesday", "Wednesday", "Thursday", "Friday")

Naming a vector (2)
If you want to become a good statistician, you have to become lazy. (If you are already lazy, chances are high you are one of those exceptional, natural-born statistical talents.)
In the previous exercises you probably experienced that it is boring and frustrating to type and retype information such as the days of the week. However, when you look at it from a higher perspective, there is a more efficient way to do this, namely, to assign the days of the week vector to a variable!
Just like you did with your poker and roulette returns, you can also create a variable that contains the days of the week. This way you can use and re-use it.
Instructions
100 XP
•	A variable days_vector that contains the days of the week has already been created for you.
•	Use days_vector to set the names of poker_vector and roulette_vector.
Take Hint (-30 XP)

# Poker winnings from Monday to Friday
poker_vector <- c(140, -50, 20, -120, 240)

# Roulette winnings from Monday to Friday
roulette_vector <- c(-24, -50, 100, -350, 10)

# The variable days_vector
days_vector <- c("Monday", "Tuesday", "Wednesday", "Thursday", "Friday")
 
# Assign the names of the day to roulette_vector and poker_vector
names(poker_vector) <-   c("Monday", "Tuesday", "Wednesday", "Thursday", "Friday")
names(roulette_vector) <-c("Monday", "Tuesday", "Wednesday", "Thursday", "Friday")

Calculating total winnings
Now that you have the poker and roulette winnings nicely as named vectors, you can start doing some data analytical magic.
You want to find out the following type of information:
•	How much has been your overall profit or loss per day of the week?
•	Have you lost money over the week in total?
•	Are you winning/losing money on poker or on roulette?
To get the answers, you have to do arithmetic calculations on vectors.
It is important to know that if you sum two vectors in R, it takes the element-wise sum. For example, the following three statements are completely equivalent:
c(1, 2, 3) + c(4, 5, 6)
c(1 + 4, 2 + 5, 3 + 6)
c(5, 7, 9)
You can also do the calculations with variables that represent vectors:
a <- c(1, 2, 3) 
b <- c(4, 5, 6)
c <- a + b
Instructions
100 XP
•	Take the sum of the variables A_vector and B_vector and assign it to total_vector.
•	Inspect the result by printing out total_vector.
Take Hint (-30 XP)

A_vector <- c(1, 2, 3)
B_vector <- c(4, 5, 6)

# Take the sum of A_vector and B_vector
total_vector <- A_vector+B_vector
  
# Print out total_vector
print (total_vector)

Calculating total winnings (2)
Now you understand how R does arithmetic with vectors, it is time to get those Ferraris in your garage! First, you need to understand what the overall profit or loss per day of the week was. The total daily profit is the sum of the profit/loss you realized on poker per day, and the profit/loss you realized on roulette per day.
In R, this is just the sum of roulette_vector and poker_vector.
Instructions
100 XP
Assign to the variable total_daily how much you won or lost on each day in total (poker and roulette combined).
Take Hint (-30 XP)

# Poker and roulette winnings from Monday to Friday:
poker_vector <- c(140, -50, 20, -120, 240)
roulette_vector <- c(-24, -50, 100, -350, 10)
days_vector <- c("Monday", "Tuesday", "Wednesday", "Thursday", "Friday")
names(poker_vector) <- days_vector
names(roulette_vector) <- days_vector

# Assign to total_daily how much you won/lost on each day
total_daily <- poker_vector+roulette_vector

Calculating total winnings (3)
Based on the previous analysis, it looks like you had a mix of good and bad days. This is not what your ego expected, and you wonder if there may be a very tiny chance you have lost money over the week in total?
A function that helps you to answer this question is sum(). It calculates the sum of all elements of a vector. For example, to calculate the total amount of money you have lost/won with poker you do:
total_poker <- sum(poker_vector)
Instructions
100 XP
•	Calculate the total amount of money that you have won/lost with roulette and assign to the variable total_roulette.
•	Now that you have the totals for roulette and poker, you can easily calculate total_week (which is the sum of all gains and losses of the week).
•	Print out total_week.
Take Hint (-30 XP)

# Poker and roulette winnings from Monday to Friday:
poker_vector <- c(140, -50, 20, -120, 240)
roulette_vector <- c(-24, -50, 100, -350, 10)
days_vector <- c("Monday", "Tuesday", "Wednesday", "Thursday", "Friday")
names(poker_vector) <- days_vector
names(roulette_vector) <- days_vector

# Total winnings with poker
total_poker <- sum(poker_vector)

# Total winnings with roulette
total_roulette <-  sum(roulette_vector)

# Total winnings overall
total_week <- sum(total_poker,total_roulette)

# Print out total_week
  print (total_week)

Comparing total winnings
Oops, it seems like you are losing money. Time to rethink and adapt your strategy! This will require some deeper analysis...
After a short brainstorm in your hotel's jacuzzi, you realize that a possible explanation might be that your skills in roulette are not as well developed as your skills in poker. So maybe your total gains in poker are higher (or > ) than in roulette.
Instructions
100 XP
•	Calculate total_poker and total_roulette as in the previous exercise. Use the sum() function twice.
•	Check if your total gains in poker are higher than for roulette by using a comparison. Simply print out the result of this comparison. What do you conclude, should you focus on roulette or on poker?
•	
Take Hint (-30 XP)

# Poker and roulette winnings from Monday to Friday:
poker_vector <- c(140, -50, 20, -120, 240)
roulette_vector <- c(-24, -50, 100, -350, 10)
days_vector <- c("Monday", "Tuesday", "Wednesday", "Thursday", "Friday")
names(poker_vector) <- days_vector
names(roulette_vector) <- days_vector

# Calculate total gains for poker and roulette
total_poker <-sum(poker_vector)
total_roulette <-sum(roulette_vector)

# Check if you realized higher total gains in poker than in roulette 
total_poker > total_roulette

Vector selection: the good times
Your hunch seemed to be right. It appears that the poker game is more your cup of tea than roulette.
Another possible route for investigation is your performance at the beginning of the working week compared to the end of it. You did have a couple of Margarita cocktails at the end of the week...
To answer that question, you only want to focus on a selection of the total_vector. In other words, our goal is to select specific elements of the vector. To select elements of a vector (and later matrices, data frames, ...), you can use square brackets. Between the square brackets, you indicate what elements to select. For example, to select the first element of the vector, you type poker_vector[1]. To select the second element of the vector, you type poker_vector[2], etc. Notice that the first element in a vector has index 1, not 0 as in many other programming languages.
Instructions
100 XP
Assign the poker results of Wednesday to the variable poker_wednesday.
Take Hint (-30 XP)

# Poker and roulette winnings from Monday to Friday:
poker_vector <- c(140, -50, 20, -120, 240)
roulette_vector <- c(-24, -50, 100, -350, 10)
days_vector <- c("Monday", "Tuesday", "Wednesday", "Thursday", "Friday")
names(poker_vector) <- days_vector
names(roulette_vector) <- days_vector

# Define a new variable based on a selection
poker_wednesday <- poker_vector[3]

Vector selection: the good times (2)
How about analyzing your midweek results?
To select multiple elements from a vector, you can add square brackets at the end of it. You can indicate between the brackets what elements should be selected. For example: suppose you want to select the first and the fifth day of the week: use the vector c(1, 5) between the square brackets. For example, the code below selects the first and fifth element of poker_vector:
poker_vector[c(1, 5)]
Instructions
100 XP
Assign the poker results of Tuesday, Wednesday and Thursday to the variable poker_midweek.
Take Hint (-30 XP)

# Poker and roulette winnings from Monday to Friday:
poker_vector <- c(140, -50, 20, -120, 240)
roulette_vector <- c(-24, -50, 100, -350, 10)
days_vector <- c("Monday", "Tuesday", "Wednesday", "Thursday", "Friday")
names(poker_vector) <- days_vector
names(roulette_vector) <- days_vector

# Define a new variable based on a selection
poker_midweek <- poker_vector[c(2, 3,4)]

Vector selection: the good times (3)
Selecting multiple elements of poker_vector with c(2, 3, 4) is not very convenient. Many statisticians are lazy people by nature, so they created an easier way to do this: c(2, 3, 4) can be abbreviated to2:4, which generates a vector with all natural numbers from 2 up to 4.
So, another way to find the mid-week results is poker_vector[2:4]. Notice how the vector 2:4 is placed between the square brackets to select element 2 up to 4.
Instructions
100 XP
Assign to roulette_selection_vector the roulette results from Tuesday up to Friday; make use of : if it makes things easier for you.
Take Hint (-30 XP)

# Poker and roulette winnings from Monday to Friday:
poker_vector <- c(140, -50, 20, -120, 240)
roulette_vector <- c(-24, -50, 100, -350, 10)
days_vector <- c("Monday", "Tuesday", "Wednesday", "Thursday", "Friday")
names(poker_vector) <- days_vector
names(roulette_vector) <- days_vector

# Define a new variable based on a selection
roulette_selection_vector <- roulette_vector[2:5]

Vector selection: the good times (4)
Another way to tackle the previous exercise is by using the names of the vector elements (Monday, Tuesday, ...) instead of their numeric positions. For example,
poker_vector["Monday"]
will select the first element of poker_vector since "Monday" is the name of that first element.
Just like you did in the previous exercise with numerics, you can also use the element names to select multiple elements, for example:
poker_vector[c("Monday","Tuesday")]
Instructions
100 XP
•	Select the first three elements in poker_vector by using their names: "Monday", "Tuesday" and "Wednesday". Assign the result of the selection to poker_start.
•	Calculate the average of the values in poker_start with the mean() function. Simply print out the result so you can inspect it.
Take Hint (-30 XP)

# Poker and roulette winnings from Monday to Friday:
poker_vector <- c(140, -50, 20, -120, 240)
roulette_vector <- c(-24, -50, 100, -350, 10)
days_vector <- c("Monday", "Tuesday", "Wednesday", "Thursday", "Friday")
names(poker_vector) <- days_vector
names(roulette_vector) <- days_vector

# Select poker results for Monday, Tuesday and Wednesday
poker_start <- poker_vector[c("Monday","Tuesday","Wednesday")]
  
# Calculate the average of the elements in poker_start
mean(poker_start)

Selection by comparison - Step 1
By making use of comparison operators, we can approach the previous question in a more proactive way.
The (logical) comparison operators known to R are:
•	< for less than
•	> for greater than
•	<= for less than or equal to
•	>= for greater than or equal to
•	== for equal to each other
•	!= not equal to each other
As seen in the previous chapter, stating 6 > 5 returns TRUE. The nice thing about R is that you can use these comparison operators also on vectors. For example:
> c(4, 5, 6) > 5
[1] FALSE FALSE TRUE
This command tests for every element of the vector if the condition stated by the comparison operator is TRUE or FALSE.
Instructions
100 XP
•	Check which elements in poker_vector are positive (i.e. > 0) and assign this to selection_vector.
•	Print out selection_vector so you can inspect it. The printout tells you whether you won (TRUE) or lost (FALSE) any money for each day.
Take Hint (-30 XP)

# Poker and roulette winnings from Monday to Friday:
poker_vector <- c(140, -50, 20, -120, 240)
roulette_vector <- c(-24, -50, 100, -350, 10)
days_vector <- c("Monday", "Tuesday", "Wednesday", "Thursday", "Friday")
names(poker_vector) <- days_vector
names(roulette_vector) <- days_vector

# Which days did you make money on poker?
selection_vector <- (poker_vector>0)
  
# Print out selection_vector
print (selection_vector)

Selection by comparison - Step 2
Working with comparisons will make your data analytical life easier. Instead of selecting a subset of days to investigate yourself (like before), you can simply ask R to return only those days where you realized a positive return for poker.
In the previous exercises you used selection_vector <- poker_vector > 0 to find the days on which you had a positive poker return. Now, you would like to know not only the days on which you won, but also how much you won on those days.
You can select the desired elements, by putting selection_vector between the square brackets that follow poker_vector:
poker_vector[selection_vector]
R knows what to do when you pass a logical vector in square brackets: it will only select the elements that correspond to TRUE in selection_vector.
Instructions
100 XP
Use selection_vector in square brackets to assign the amounts that you won on the profitable days to the variable poker_winning_days.
Take Hint (-30 XP)

# Poker and roulette winnings from Monday to Friday:
poker_vector <- c(140, -50, 20, -120, 240)
roulette_vector <- c(-24, -50, 100, -350, 10)
days_vector <- c("Monday", "Tuesday", "Wednesday", "Thursday", "Friday")
names(poker_vector) <- days_vector
names(roulette_vector) <- days_vector

# Which days did you make money on poker?
selection_vector <- poker_vector > 0

# Select from poker_vector these days
poker_winning_days <- poker_vector[selection_vector]

Advanced selection
Just like you did for poker, you also want to know those days where you realized a positive return for roulette.
Instructions
100 XP
•	Create the variable selection_vector, this time to see if you made profit with roulette for different days.
•	Assign the amounts that you made on the days that you ended positively for roulette to the variable roulette_winning_days. This vector thus contains the positive winnings of roulette_vector.
•	
•	
•	
Take Hint (-30 XP)

# Poker and roulette winnings from Monday to Friday:
poker_vector <- c(140, -50, 20, -120, 240)
roulette_vector <- c(-24, -50, 100, -350, 10)
days_vector <- c("Monday", "Tuesday", "Wednesday", "Thursday", "Friday")
names(poker_vector) <- days_vector
names(roulette_vector) <- days_vector

# Which days did you make money on roulette?
selection_vector <-(roulette_vector>0)

# Select from roulette_vector these days
roulette_winning_days <- roulette_vector[selection_vector]



 
Chapter 3
Matrices

What's a matrix?
In R, a matrix is a collection of elements of the same data type (numeric, character, or logical) arranged into a fixed number of rows and columns. Since you are only working with rows and columns, a matrix is called two-dimensional.
You can construct a matrix in R with the matrix() function. Consider the following example:
matrix(1:9, byrow = TRUE, nrow = 3)
In the matrix() function:
•	The first argument is the collection of elements that R will arrange into the rows and columns of the matrix. Here, we use 1:9 which is a shortcut for c(1, 2, 3, 4, 5, 6, 7, 8, 9).
•	The argument byrow indicates that the matrix is filled by the rows. If we want the matrix to be filled by the columns, we just place byrow = FALSE.
•	The third argument nrow indicates that the matrix should have three rows.
Instructions
100 XP
Construct a matrix with 3 rows containing the numbers 1 up to 9, filled row-wise.
Take Hint (-30 XP)

# Construct a matrix with 3 rows that contain the numbers 1 up to 9
matrix(1:9, byrow = TRUE, nrow = 3)

经过实验，必须要输入by row， nrow。这两个都不能省略。

Analyze matrices, you shall
It is now time to get your hands dirty. In the following exercises you will analyze the box office numbers of the Star Wars franchise. May the force be with you!
In the editor, three vectors are defined. Each one represents the box office numbers from the first three Star Wars movies. The first element of each vector indicates the US box office revenue, the second element refers to the Non-US box office (source: Wikipedia).
In this exercise, you'll combine all these figures into a single vector. Next, you'll build a matrix from this vector.
Instructions
100 XP
•	Use c(new_hope, empire_strikes, return_jedi) to combine the three vectors into one vector. Call this vector box_office.
•	Construct a matrix with 3 rows, where each row represents a movie. Use the matrix() function to do this. The first argument is the vector box_office, containing all box office figures. Next, you'll have to specify nrow = 3 and byrow = TRUE. Name the resulting matrix star_wars_matrix.
Take Hint (-30 XP)

c(new_hope, empire_strikes, return_jedi)# Box office Star Wars (in millions!)
new_hope <- c(460.998, 314.4)
empire_strikes <- c(290.475, 247.900)
return_jedi <- c(309.306, 165.8)

# Create box_office
box_office <- c(new_hope, empire_strikes, return_jedi)

# Construct star_wars_matrix
star_wars_matrix <- matrix(box_office,byrow = TRUE,nrow = 3 )

Naming a matrix
To help you remember what is stored in star_wars_matrix, you would like to add the names of the movies for the rows. Not only does this help you to read the data, but it is also useful to select certain elements from the matrix.
Similar to vectors, you can add names for the rows and the columns of a matrix
rownames(my_matrix) <- row_names_vector
colnames(my_matrix) <- col_names_vector
We went ahead and prepared two vectors for you: region, and titles. You will need these vectors to name the columns and rows of star_wars_matrix, respectively.
Instructions
100 XP
•	Use colnames() to name the columns of star_wars_matrix with the region vector.
•	Use rownames() to name the rows of star_wars_matrix with the titles vector.
•	Print out star_wars_matrix to see the result of your work.
Take Hint (-30 XP)

# Box office Star Wars (in millions!)
new_hope <- c(460.998, 314.4)
empire_strikes <- c(290.475, 247.900)
return_jedi <- c(309.306, 165.8)

# Construct matrix
star_wars_matrix <- matrix(c(new_hope, empire_strikes, return_jedi), nrow = 3, byrow = TRUE)

# Vectors region and titles, used for naming
region <- c("US", "non-US")
titles <- c("A New Hope", "The Empire Strikes Back", "Return of the Jedi")

# Name the columns （列）with region 
对谁进行赋值，在此，对列变量进行命名
colnames(star_wars_matrix) <- region

# Name the rows （行）with titles
对谁进行赋值，在此，对行变量进行命名
rownames(star_wars_matrix) <- titles

# Print out star_wars_matrix
print(star_wars_matrix)

Calculating the worldwide box office
The single most important thing for a movie in order to become an instant legend in Tinseltown is its worldwide box office figures.
To calculate the total box office revenue for the three Star Wars movies, you have to take the sum of the US revenue column and the non-US revenue column.
In R, the function rowSums() conveniently calculates the totals for each row of a matrix. This function creates a new vector:
Rowsums函数负责对行变量进行求和
rowSums(my_matrix)
Instructions
100 XP
Calculate the worldwide box office figures for the three movies and put these in the vector named worldwide_vector.
Take Hint (-30 XP)

# Construct star_wars_matrix
box_office <- c(460.998, 314.4, 290.475, 247.900, 309.306, 165.8)
star_wars_matrix <- matrix(box_office, nrow = 3, byrow = TRUE,
                           dimnames = list(c("A New Hope", "The Empire Strikes Back", "Return of the Jedi"), 
                                           c("US", "non-US")))

# Calculate worldwide box office figures
worldwide_vector <- rowSums(star_wars_matrix)
注意：rowsums的括号里的对象必须是矩阵而不能是像（box_office）这样的向量

Adding a column for the Worldwide box office
In the previous exercise you calculated the vector that contained the worldwide box office receipt for each of the three Star Wars movies. However, this vector is not yet part of star_wars_matrix.
You can add a column or multiple columns to a matrix with the cbind() function, which merges matrices and/or vectors together by column. For example:
big_matrix <- cbind(matrix1, matrix2, vector1 ...)
Instructions
100 XP
Add worldwide_vector as a new column to the star_wars_matrix and assign the result to all_wars_matrix. Use the cbind() function.
Take Hint (-30 XP)

# Construct star_wars_matrix
box_office <- c(460.998, 314.4, 290.475, 247.900, 309.306, 165.8)
star_wars_matrix <- matrix(box_office, nrow = 3, byrow = TRUE,
                           dimnames = list(c("A New Hope", "The Empire Strikes Back", "Return of the Jedi"), 
                                           c("US", "non-US")))

# The worldwide box office figures
worldwide_vector <- rowSums(star_wars_matrix)

# Bind the new variable worldwide_vector as a column to star_wars_matrix
all_wars_matrix <- cbind(star_wars_matrix,worldwide_vector)
要想给matrix矩阵加向量vector，矩阵在前，向量在后

Adding a row
Just like every action has a reaction, every cbind() has an rbind(). (We admit, we are pretty bad with metaphors.)
Your R workspace, where all variables you defined 'live' (check out what a workspace is), has already been initialized and contains two matrices:
•	star_wars_matrix that we have used all along, with data on the original trilogy,
•	star_wars_matrix2, with similar data for the prequels trilogy.
Type the name of these matrices in the console and hit Enter if you want to have a closer look. If you want to check out the contents of the workspace, you can type ls() in the console.
Instructions
100 XP
Use rbind() to paste together star_wars_matrix and star_wars_matrix2, in this order. Assign the resulting matrix to all_wars_matrix.
Take Hint (-30 XP)

# star_wars_matrix and star_wars_matrix2 are available in your workspace
star_wars_matrix  
star_wars_matrix2 

# Combine both Star Wars trilogies in one matrix
all_wars_matrix <- rbind(star_wars_matrix,star_wars_matrix2)

rbind函数主要是用来

The total box office revenue for the entire saga
Just like cbind() has rbind(), colSums() has rowSums(). Your R workspace already contains the all_wars_matrix that you constructed in the previous exercise; type all_wars_matrix to have another look. Let's now calculate the total box office revenue for the entire saga.
Instructions
100 XP
•	Calculate the total revenue for the US and the non-US region and assign total_revenue_vector. You can use the colSums() function.
•	Print out total_revenue_vector to have a look at the results.
Take Hint (-30 XP)

# all_wars_matrix is available in your workspace
all_wars_matrix

# Total revenue for US and non-US
total_revenue_vector <- colSums(all_wars_matrix)
  
# Print out total_revenue_vector
print(total_revenue_vector)

Selection of matrix elements
Similar to vectors, you can use the square brackets [ ] to select one or multiple elements from a matrix. Whereas vectors have one dimension, matrices have two dimensions. You should therefore use a comma to separate the rows you want to select from the columns. For example:
•	my_matrix[1,2] selects the element at the first row and second column.
•	my_matrix[1:3,2:4] results in a matrix with the data on the rows 1, 2, 3 and columns 2, 3, 4.
If you want to select all elements of a row or a column, no number is needed before or after the comma, respectively:
•	my_matrix[,1] selects all elements of the first column.
•	my_matrix[1,] selects all elements of the first row.
Back to Star Wars with this newly acquired knowledge! As in the previous exercise, all_wars_matrix is already available in your workspace.
Instructions
100 XP
•	Select the non-US revenue for all movies (the entire second column of all_wars_matrix), store the result as non_us_all.
•	Use mean() on non_us_all to calculate the average non-US revenue for all movies. Simply print out the result.
•	This time, select the non-US revenue for the first two movies in all_wars_matrix. Store the result as non_us_some.
•	Use mean() again to print out the average of the values in non_us_some.
Take Hint (-30 XP)

# all_wars_matrix is available in your workspace
all_wars_matrix

# Select the non-US revenue for all movies
non_us_all <- all_wars_matrix[,2]
  
# Average non-US revenue
mean(non_us_all)
  
# Select the non-US revenue for first two movies
non_us_some <- all_wars_matrix[1:2,2]
  
# Average non-US revenue for first two movies
mean(non_us_some)

A little arithmetic with matrices
Similar to what you have learned with vectors, the standard operators like +, -, /, *, etc. work in an element-wise way on matrices in R.
For example, 2 * my_matrix multiplies each element of my_matrix by two.
As a newly-hired data analyst for Lucasfilm, it is your job to find out how many visitors went to each movie for each geographical area. You already have the total revenue figures in all_wars_matrix. Assume that the price of a ticket was 5 dollars. Simply dividing the box office numbers by this ticket price gives you the number of visitors.
Instructions
100 XP
•	Divide all_wars_matrix by 5, giving you the number of visitors in millions. Assign the resulting matrix to visitors.
•	Print out visitors so you can have a look.
Take Hint (-30 XP)

# all_wars_matrix is available in your workspace
all_wars_matrix

# Estimate the visitors
visitors <- all_wars_matrix/5
  
# Print the estimate to the console
print(visitors)

A little arithmetic with matrices (2)
Just like 2 * my_matrix multiplied every element of my_matrix by two, my_matrix1 * my_matrix2 creates a matrix where each element is the product of the corresponding elements in my_matrix1 and my_matrix2.
After looking at the result of the previous exercise, big boss Lucas points out that the ticket prices went up over time. He asks to redo the analysis based on the prices you can find in ticket_prices_matrix (source: imagination).
Those who are familiar with matrices should note that this is not the standard matrix multiplication for which you should use %*% in R.
Instructions
100 XP
•	Divide all_wars_matrix by ticket_prices_matrix to get the estimated number of US and non-US visitors for the six movies. Assign the result to visitors.
•	From the visitors matrix, select the entire first column, representing the number of visitors in the US. Store this selection as us_visitors.
•	Calculate the average number of US visitors; print out the result.
Take Hint (-30 XP)

# all_wars_matrix and ticket_prices_matrix are available in your workspace
all_wars_matrix
ticket_prices_matrix

# Estimated number of visitors
visitors <- all_wars_matrix/ticket_prices_matrix

# US visitors
us_visitors <- visitors[,1]

# Average number of US visitors
mean(us_visitors)












 
Chapter 4
What's a factor and why would you use it?
In this chapter you dive into the wonderful world of factors.
The term factor refers to a statistical data type used to store categorical variables. The difference between a categorical variable and a continuous variable is that a categorical variable can belong to a limited number of categories. A continuous variable, on the other hand, can correspond to an infinite number of values.
It is important that R knows whether it is dealing with a continuous or a categorical variable, as the statistical models you will develop in the future treat both types differently. (You will see later why this is the case.)
A good example of a categorical variable is sex. In many circumstances you can limit the sex categories to "Male" or "Female". (Sometimes you may need different categories. For example, you may need to consider chromosomal variation, hermaphroditic animals, or different cultural norms, but you will always have a finite number of categories.)
Instructions
100 XP
Assign to variable theory the value "factors for categorical variables".
Take Hint (-30 XP)

# Assign to the variable theory what this chapter is about!
theory<-"factors for categorical variables"
（对变量进行赋值（文本值，前文已讲，记得加引号））

What's a factor and why would you use it? (2)
To create factors in R, you make use of the function factor(). First thing that you have to do is create a vector that contains all the observations that belong to a limited number of categories. For example, sex_vector contains the sex of 5 different individuals:
sex_vector <- c("Male","Female","Female","Male","Male")
It is clear that there are two categories, or in R-terms 'factor levels', at work here: "Male" and "Female".
The function factor() will encode the vector as a factor:
factor_sex_vector <- factor(sex_vector)
（factor函数负责把vector（向量）转化为factor变量，新变量名字是factor_sex_vector）

Instructions
100 XP
•	Convert the character vector sex_vector to a factor with factor() and assign the result to factor_sex_vector
•	Print out factor_sex_vector and assert that R prints out the factor levels below the actual values.
Take Hint (-30 XP)

# Sex vector
sex_vector <- c("Male", "Female", "Female", "Male", "Male")

# Convert sex_vector to a factor
factor_sex_vector <-factor(sex_vector)

# Print out factor_sex_vector
print(factor(sex_vector))

What's a factor and why would you use it? (3)
There are two types of categorical variables: a nominal categorical variable and an ordinal categorical variable.
变量分为两种：nominal categorical variable（名义变量）和ordinal categorical variable（）
A nominal variable is a categorical variable without an implied order. This means that it is impossible to say that 'one is worth more than the other'. For example, think of the categorical variable animals_vector with the categories "Elephant", "Giraffe", "Donkey" and "Horse". Here, it is impossible to say that one stands above or below the other. (Note that some of you might disagree ;-) ).
名义变量是没有隐含顺序的范畴变量。这意味着我们不可能说“一个比另一个更有价值”。例如，考虑包含类别“大象”、“长颈鹿”、“驴”和“马”的分类变量animals_vector。在这里，我们不可能说其中一个高于或低于另一个。(注意有些人可能不同意;-))。
In contrast, ordinal variables do have a natural ordering. Consider for example the categorical variable temperature_vector with the categories: "Low", "Medium" and "High". Here it is obvious that "Medium" stands above "Low", and "High" stands above "Medium".
相反，序数变量///有一个自然的顺序。例如，考虑类别变量temperature_vector，其中包含类别:“低”、“中”和“高”。很明显，“中等”高于“低”，“高”高于“中等”。
Instructions
100 XP
Click 'Submit Answer' to check how R constructs and prints nominal and ordinal variables. Do not worry if you do not understand all the code just yet, we will get to that. （此处没有写代码要求，只要求看代码）

Take Hint (-30 XP)

# Animals
animals_vector <- c("Elephant", "Giraffe", "Donkey", "Horse")
factor_animals_vector <- factor(animals_vector)
factor_animals_vector

# Temperature
temperature_vector <- c("High", "Low", "High","Low", "Medium")
factor_temperature_vector <- factor(temperature_vector, order = TRUE, levels = c("Low", "Medium", "High"))
factor_temperature_vector
（此处没有写代码要求，只要求看代码）

以下是输出部分内容：

> # Animals
> animals_vector <- c("Elephant", "Giraffe", "Donkey", "Horse")
> factor_animals_vector <- factor(animals_vector)
> factor_animals_vector
[1] Elephant Giraffe  Donkey   Horse   
Levels: Donkey Elephant Giraffe Horse
> 
> # Temperature
> temperature_vector <- c("High", "Low", "High","Low", "Medium")
> factor_temperature_vector <- factor(temperature_vector, order = TRUE, levels = c("Low", "Medium", "High"))
> factor_temperature_vector
[1] High   Low    High   Low    Medium
Levels: Low < Medium < High
>

Can you already tell what's happening in this exercise? Awesome! Continue to the next exercise and get into the details of factor levels.


Factor levels
When you first get a data set, you will often notice that it contains factors with specific factor levels. However, sometimes you will want to change the names of these levels for clarity or other reasons. R allows you to do this with the function levels():
levels(factor_vector) <- c("name1", "name2",...)
对向量内不同的变量进行改名(change the names of these levels for clarity or other reasons/因为清晰或其他原因而希望更改这些级别的名称),使用levels函数：
levels函数语法
Levels（变量名：可以是factor或者vector变量）<- c("第一个变量改为名称1name1", "第二个变量改为名称2 name2",...)
A good illustration is the raw data that is provided to you by a survey. A common question for every questionnaire is the sex of the respondent. Here, for simplicity, just two categories were recorded, "M" and "F". (You usually need more categories for survey data; either way, you use a factor to store the categorical data.)
survey_vector <- c("M", "F", "F", "M", "M")

这个变量使用简写M和F,我们可能会误解所以为了清晰和规范表达，我们使用"Male" and "Female" instead of "M" and "F" for clarity。

Recording the sex with the abbreviations "M" and "F" can be convenient if you are collecting data with pen and paper, but it can introduce confusion when analyzing the data. At that point, you will often want to change the factor levels to "Male" and "Female" instead of "M" and "F" for clarity.
Watch out: the order with which you assign the levels is important. If you type levels(factor_survey_vector), you'll see that it outputs [1] "F" "M". If you don't specify the levels of the factor when creating the vector, R will automatically assign them alphabetically. To correctly map "F" to "Female" and "M" to "Male", the levels should be set to c("Female", "Male"), in this order.
Instructions
100 XP
•	Check out the code that builds a factor vector from survey_vector. You should use factor_survey_vector in the next instruction.
•	Change the factor levels of factor_survey_vector to c("Female", "Male"). Mind the order of the vector elements here.
Take Hint (-30 XP)

# Code to build factor_survey_vector
survey_vector <- c("M", "F", "F", "M", "M")
factor_survey_vector <- factor(survey_vector)

# Specify the levels of factor_survey_vector
levels(factor_survey_vector) <-c("Female", "Male")

factor_survey_vector

Summarizing a factor
After finishing this course, one of your favorite functions in R will be summary(). This will give you a quick overview of the contents of a variable:
summary(my_var)
Going back to our survey, you would like to know how many "Male" responses you have in your study, and how many "Female" responses. The summary() function gives you the answer to this question.
Summary函数的目的在于给某个特定的变量(variable) a quick overview of the contents快速概述一个变量的内容
This enables R to show the number of elements for each category.
Instructions
100 XP
Ask a summary() of the survey_vector and factor_survey_vector. Interpret the results of both vectors. Are they both equally useful in this case?
Take Hint (-30 XP)

# Build factor_survey_vector with clean levels
survey_vector <- c("M", "F", "F", "M", "M")
factor_survey_vector <- factor(survey_vector)
levels(factor_survey_vector) <- c("Female", "Male")
factor_survey_vector

# Generate summary for survey_vector
summary(survey_vector)

# Generate summary for factor_survey_vector
summary(factor_survey_vector)

Battle of the sexes
You might wonder what happens when you try to compare elements of a factor. In factor_survey_vector you have a factor with two levels: "Male" and "Female". But how does R value these relative to each other?
Instructions
100 XP
Read the code in the editor and click 'Submit Answer' to test if male is greater than (>) female.
Take Hint (-30 XP)

（此处没有写代码要求，只要求看代码）
# Build factor_survey_vector with clean levels
survey_vector <- c("M", "F", "F", "M", "M")
factor_survey_vector <- factor(survey_vector)
levels(factor_survey_vector) <- c("Female", "Male")

# Male
male <- factor_survey_vector[1]

# Female
female <- factor_survey_vector[2]

# Battle of the sexes: Male 'larger' than female?
male > female

（此处没有写代码要求，只要求看代码）

以下是输出部分内容：

> # Build factor_survey_vector with clean levels
> survey_vector <- c("M", "F", "F", "M", "M")
> factor_survey_vector <- factor(survey_vector)
> levels(factor_survey_vector) <- c("Female", "Male")
> 
> # Male
> male <- factor_survey_vector[1]
> 
> # Female
> female <- factor_survey_vector[2]
> 
> # Battle of the sexes: Male 'larger' than female?
> male > female
Warning message: '>' not meaningful for factors
[1] NA

How interesting! By default, R returns NA when you try to compare values in a factor, since the idea doesn't make sense. Next you'll learn about ordered factors, where more meaningful comparisons are possible.
多么有趣啊!默认情况下，当您试图比较一个因子中的值时，R会返回NA，因为这个想法没有意义。接下来，您将了解有序因子，在这里可以进行更有意义的比较。

Ordered factors
Since "Male" and "Female" are unordered (or nominal) factor levels, R returns a warning message, telling you that the greater than operator is not meaningful. As seen before, R attaches an equal value to the levels for such factors.
But this is not always the case! Sometimes you will also deal with factors that do have a natural ordering between its categories. If this is the case, we have to make sure that we pass this information to R...
Let us say that you are leading a research team of five data analysts and that you want to evaluate their performance. To do this, you track their speed, evaluate each analyst as "slow", "medium" or "fast", and save the results in speed_vector.
Instructions
100 XP
As a first step, assign speed_vector a vector with 5 entries, one for each analyst. Each entry should be either "slow", "medium", or "fast". Use the list below:
•	Analyst 1 is medium,
•	Analyst 2 is slow,
•	Analyst 3 is slow,
•	Analyst 4 is medium and
•	Analyst 5 is fast.
No need to specify these are factors yet.
Take Hint (-30 XP)

# Create speed_vector
speed_vector <-c("medium","slow","slow","medium","fast")

Ordered factors (2)
speed_vector should be converted to an ordinal factor since its categories have a natural ordering. By default, the function factor() transforms speed_vector into an unordered factor. To create an ordered factor, you have to add two additional arguments: ordered and levels.

把vector转化为ordinal factor7因为他的分类（categories）具有自然顺序（natural ordering）。默认的，函数factor()将speed_vector 转化为一个无序的factor（unordered factor）。为了创建一个有序factor（ordered factor），你需要对factor()这个函数加入两个额外参数：ordered and levels。
以下是函数语法：
factor(some_vector,
       ordered = TRUE,
       levels = c("lev1", "lev2" ...))
By setting the argument ordered to TRUE in the function factor(), you indicate that the factor is ordered. With the argument levels you give the values of the factor in the correct order.
Ordered参数是用来确认这个factor是有序的还是无序的。ordered = TRUE说明factor is ordered（该参数是有序的）
Levels参数是对factor进行正确序列进行value评估。levels = c("slow", "medium", "fast")说明正确的排序方式是("slow", "medium", "fast")
Instructions
100 XP
From speed_vector, create an ordered factor vector: factor_speed_vector. Set ordered to TRUE, and set levels to c("slow", "medium", "fast").
Take Hint (-30 XP)

# Create speed_vector
speed_vector <- c("medium", "slow", "slow", "medium", "fast")

# Convert speed_vector to ordered factor vector
factor_speed_vector <-factor(speed_vector,ordered = TRUE, levels = c("slow", "medium", "fast"))

factor函数有三个输入值，第一个是vector值，第二个是ordered值，可以是true或者false，第三个是levels值，按照levels = c("slow", "medium", "fast")进行。

# Print factor_speed_vector
factor_speed_vector
summary(factor_speed_vector)

Great! Have a look at the console. It is now indicated that the Levels indeed have an order associated, with the < sign. Continue to the next exercise.

Comparing ordered factors
Having a bad day at work, 'data analyst number two' enters your office and starts complaining that 'data analyst number five' is slowing down the entire project. Since you know that 'data analyst number two' has the reputation of being a smarty-pants, you first decide to check if his statement is true.
The fact that factor_speed_vector is now ordered enables us to compare different elements (the data analysts in this case). You can simply do this by using the well-known operators.
Instructions
100 XP
•	Use [2] to select from factor_speed_vector the factor value for the second data analyst. Store it as da2.
•	Use [5] to select the factor_speed_vector factor value for the fifth data analyst. Store it as da5.
•	Check if da2 is greater than da5; simply print out the result. Remember that you can use the > operator to check whether one element is larger than the other.
Take Hint (-30 XP)

# Create factor_speed_vector
speed_vector <- c("medium", "slow", "slow", "medium", "fast")
factor_speed_vector <- factor(speed_vector, ordered = TRUE, levels = c("slow", "medium", "fast"))

# Factor value for second data analyst
da2 <-factor_speed_vector[2]

（从vector中选取特定的某个/某一排/某一列变量variable）

# Factor value for fifth data analyst
da5 <-factor_speed_vector[5]

# Is data analyst 2 faster than data analyst 5?
Da2>da5
（大于小于符号本身就是比较，其结果输出为true或者false这样的逻辑值）



















 
Chapter 5 Data frames
What's a data frame [计] 数据帧?
You may remember from the chapter about matrices that all the elements that you put in a matrix should be of the same type. Back then, your data set on Star Wars only contained numeric elements.
When doing a market research survey, however, you often have questions such as:
•	'Are you married?' or 'yes/no' questions (logical)逻辑值
•	'How old are you?' (numeric)数值型数据
•	'What is your opinion on this product?' or other 'open-ended' questions (character)文本值
•	...
The output, namely the respondents' answers to the questions formulated above, is a data set of different data types. You will often find yourself working with data sets that contain different data types instead of only one.
输出，即受访者对上述问题的回答，是不同数据类型的数据集。您经常会发现自己处理的数据集包含不同的数据类型，而不是只有一种。
A data frame has the variables of a data set as columns and the observations as rows. This will be a familiar concept for those coming from different statistical software packages such as SAS or SPSS.
数据帧将数据集的变量作为列，将观察值作为行。对于来自不同统计软件包(如SAS或SPSS)的人来说，这是一个熟悉的概念。
Instructions
100 XP
Click 'Submit Answer'. The data from the built-in example data frame mtcars will be printed to the console.
Take Hint (-30 XP)

（此处没有写代码要求，只要求看代码）

# Print out built-in R data frame
Mtcars

以下是输出内容： 

> # Print out built-in R data frame
> mtcars
                     mpg cyl  disp  hp drat    wt  qsec vs am gear carb
Mazda RX4           21.0   6 160.0 110 3.90 2.620 16.46  0  1    4    4
Mazda RX4 Wag       21.0   6 160.0 110 3.90 2.875 17.02  0  1    4    4
Datsun 710          22.8   4 108.0  93 3.85 2.320 18.61  1  1    4    1
Hornet 4 Drive      21.4   6 258.0 110 3.08 3.215 19.44  1  0    3    1
Hornet Sportabout   18.7   8 360.0 175 3.15 3.440 17.02  0  0    3    2
Valiant             18.1   6 225.0 105 2.76 3.460 20.22  1  0    3    1
Duster 360          14.3   8 360.0 245 3.21 3.570 15.84  0  0    3    4
Merc 240D           24.4   4 146.7  62 3.69 3.190 20.00  1  0    4    2
Merc 230            22.8   4 140.8  95 3.92 3.150 22.90  1  0    4    2
Merc 280            19.2   6 167.6 123 3.92 3.440 18.30  1  0    4    4
Merc 280C           17.8   6 167.6 123 3.92 3.440 18.90  1  0    4    4
Merc 450SE          16.4   8 275.8 180 3.07 4.070 17.40  0  0    3    3
Merc 450SL          17.3   8 275.8 180 3.07 3.730 17.60  0  0    3    3
Merc 450SLC         15.2   8 275.8 180 3.07 3.780 18.00  0  0    3    3
Cadillac Fleetwood  10.4   8 472.0 205 2.93 5.250 17.98  0  0    3    4
Lincoln Continental 10.4   8 460.0 215 3.00 5.424 17.82  0  0    3    4
Chrysler Imperial   14.7   8 440.0 230 3.23 5.345 17.42  0  0    3    4
Fiat 128            32.4   4  78.7  66 4.08 2.200 19.47  1  1    4    1
Honda Civic         30.4   4  75.7  52 4.93 1.615 18.52  1  1    4    2
Toyota Corolla      33.9   4  71.1  65 4.22 1.835 19.90  1  1    4    1
Toyota Corona       21.5   4 120.1  97 3.70 2.465 20.01  1  0    3    1
Dodge Challenger    15.5   8 318.0 150 2.76 3.520 16.87  0  0    3    2
AMC Javelin         15.2   8 304.0 150 3.15 3.435 17.30  0  0    3    2
Camaro Z28          13.3   8 350.0 245 3.73 3.840 15.41  0  0    3    4
Pontiac Firebird    19.2   8 400.0 175 3.08 3.845 17.05  0  0    3    2
Fiat X1-9           27.3   4  79.0  66 4.08 1.935 18.90  1  1    4    1
Porsche 914-2       26.0   4 120.3  91 4.43 2.140 16.70  0  1    5    2
Lotus Europa        30.4   4  95.1 113 3.77 1.513 16.90  1  1    5    2
Ford Pantera L      15.8   8 351.0 264 4.22 3.170 14.50  0  1    5    4
Ferrari Dino        19.7   6 145.0 175 3.62 2.770 15.50  0  1    5    6
Maserati Bora       15.0   8 301.0 335 3.54 3.570 14.60  0  1    5    8
Volvo 142E          21.4   4 121.0 109 4.11 2.780 18.60  1  1    4    2
>

（此处没有写代码要求，只要求看代码）

Quick, have a look at your data set
Wow, that is a lot of cars!
Working with large data sets is not uncommon in data analysis. When you work with (extremely) large data sets and data frames, your first task as a data analyst is to develop a clear understanding of its structure and main elements. Therefore, it is often useful to show only a small part of the entire data set.
使用大型数据集在数据分析中并不少见。当您使用(非常)大的数据集和数据帧时，作为数据分析人员，您的第一个任务是清楚地理解它的结构和主要元素。因此，只显示整个数据集的一小部分通常是有用的。
So how to do this in R? Well, the function head() enables you to show the first observations of a data frame. Similarly, the function tail() prints out the last observations in your data set.
那么在R中怎么做呢?head()函数使您能够显示数据帧的第一次观察结果。类似地，tail()函数输出数据集中的最后一个观察值。
Both head() and tail() print a top line called the 'header', which contains the names of the different variables in your data set.
head()和tail()都打印一个名为“header”的顶行，其中包含数据集中不同变量的名称。
Instructions
100 XP
Call head() on the mtcars data set to have a look at the header and the first observations.
Take Hint (-30 XP)

# Call head() on mtcars
head(mtcars)

Wonderful! So, what do we have in this data set? For example, hp represents the car's horsepower; the Datsun has the lowest horse power of the 6 cars that are displayed. For a full overview of the variables' meaning, type ?mtcars in the console and read the help page. Continue to the next exercise!
太棒了!这个数据集中有什么?例如，hp表示汽车的马力;在展示的6辆车中，达特桑的马力最低。要全面了解变量的含义，请在控制台中键入?mtcars并阅读帮助页面。继续下一个练习!

注意：还有一个自动索引关联出来的函数叫做：head.matrix
head.matrix(mtcars)


Have a look at the structure
Another method that is often used to get a rapid overview of your data is the function str(). The function str() shows you the structure of your data set. For a data frame it tells you:
另一种经常用于快速查看数据的方法是函数str()。函数str()会显示数据集的结构。对于一个数据帧，它会告诉你:
•	The total number of observations (e.g. 32 car types)
•	The total number of variables (e.g. 11 car features)
•	A full list of the variables names (e.g. mpg, cyl ... )
•	The data type of each variable (e.g. num)
•	The first observations
•	
•	•观察总数(例如32种车型)
•	•变量总数(例如11个汽车特性)
•	完整的变量名列表(如mpg, cyl…)
•	•每个变量的数据类型(例如num)
•	•第一次观察
Applying the str() function will often be the first thing that you do when receiving a new data set or data frame. It is a great way to get more insight in your data set before diving into the real analysis.
Instructions
100 XP
Investigate the structure of mtcars. Make sure that you see the same numbers, variables and data types as mentioned above.
Take Hint (-30 XP)

# Investigate the structure of mtcars
str(mtcars)

Nice work! Can you find all the information that is listed in the exercise's assignment? Continue to the next exercise.

Creating a data frame
Since using built-in data sets is not even half the fun of creating your own data sets, the rest of this chapter is based on your personally developed data set. Put your jet pack on because it is time for some space exploration!
As a first goal, you want to construct a data frame that describes the main characteristics of eight planets in our solar system. According to your good friend Buzz, the main features of a planet are:
作为第一个目标，您需要构建一个数据框架来描述太阳系中八大行星的主要特征。根据你的好朋友巴斯的说法，行星的主要特征是:
•	The type of planet (Terrestrial or Gas Giant).
•	The planet's diameter relative to the diameter of the Earth.
•	The planet's rotation across the sun relative to that of the Earth.
•	If the planet has rings or not (TRUE or FALSE).
•	
•	•行星的类型(类地或气体巨星)。
•	•地球的直径与地球的直径之比。
•	•相对于地球，行星绕太阳的自转。
•	•行星是否有光环(对或错)。
After doing some high-quality research on Wikipedia, you feel confident enough to create the necessary vectors: name, type, diameter, rotation and rings; these vectors have already been coded up on the right. The first element in each of these vectors correspond to the first observation.
在对Wikipedia做了一些高质量的研究之后，您有足够的信心创建必要的向量:名称、类型、直径、旋转和圆环;这些向量已经在右边编码了。这些向量中的第一个元素对应于第一个观察值。

You construct a data frame with the data.frame() function. As arguments, you pass the vectors from before: they will become the different columns of your data frame. Because every column has the same length, the vectors you pass should also have the same length. But don't forget that it is possible (and likely) that they contain different types of data.
使用data.frame()函数构造一个数据框架。作为参数，传递之前的向量:它们将成为数据框架的不同列。因为每一列都有相同的长度，传递的向量也应该有相同的长度。但是不要忘记它们可能(而且很可能)包含不同类型的数据。

Instructions
100 XP
Use the function data.frame() to construct a data frame. Pass the vectors name, type, diameter, rotation and rings as arguments to data.frame(), in this order. Call the resulting data frame planets_df.
使用data.frame()函数构造一个数据框架。将向量名、类型、直径、旋转和环作为参数传递给data.frame()，按此顺序。调用结果数据帧planets_df。

Take Hint (-30 XP)

# Definition of vectors
name <- c("Mercury", "Venus", "Earth", "Mars", "Jupiter", "Saturn", "Uranus", "Neptune")
type <- c("Terrestrial planet", "Terrestrial planet", "Terrestrial planet", 
          "Terrestrial planet", "Gas giant", "Gas giant", "Gas giant", "Gas giant")
diameter <- c(0.382, 0.949, 1, 0.532, 11.209, 9.449, 4.007, 3.883)
rotation <- c(58.64, -243.02, 1, 1.03, 0.41, 0.43, -0.72, 0.67)
rings <- c(FALSE, FALSE, FALSE, FALSE, TRUE, TRUE, TRUE, TRUE)

# Create a data frame from the vectors
planets_df <-data.frame(name,type,diameter,rotation,rings)

Creating a data frame (2)
The planets_df data frame should have 8 observations and 5 variables. It has been made available in the workspace, so you can directly use it.
Instructions
100 XP
Use str() to investigate the structure of the new planets_df variable.
Take Hint (-30 XP)

# Check the structure of planets_df
str(planets_df)

Selection of data frame elements
Similar to vectors and matrices, you select elements from a data frame with the help of square brackets [ ]. By using a comma, you can indicate what to select from the rows and the columns respectively. For example:
•	my_df[1,2] selects the value at the first row and second column in my_df.
•	my_df[1:3,2:4] selects rows 1, 2, 3 and columns 2, 3, 4 in my_df.
Sometimes you want to select all elements of a row or column. For example, my_df[1, ] selects all elements of the first row. Let us now apply this technique on planets_df!
Instructions
100 XP
•	From planets_df, select the diameter of Mercury: this is the value at the first row and the third column. Simply print out the result.
•	From planets_df, select all data on Mars (the fourth row). Simply print out the result.
Take Hint (-30 XP)

# The planets_df data frame from the previous exercise is pre-loaded

# Print out diameter of Mercury (row 1, column 3)
planets_df[1,3]

# Print out data for Mars (entire fourth row)
planets_df[4, ]

Great! Apart from selecting elements from your data frame by index, you can also use the column names. To learn how, head over to the next exercise.

Selection of data frame elements (2)
Instead of using numerics to select elements of a data frame, you can also use the variable names to select columns of a data frame.
Suppose you want to select the first three elements of the type column. One way to do this is
planets_df[1:3,2]
A possible disadvantage of this approach is that you have to know (or look up) the column number of type, which gets hard if you have a lot of variables. It is often easier to just make use of the variable name:
planets_df[1:3,"type"]
Instructions
100 XP
Select and print out the first 5 values in the "diameter" column of planets_df.
Take Hint (-30 XP)

# The planets_df data frame from the previous exercise is pre-loaded

# Select first 5 values of diameter column
planets_df[1:5,"diameter"]

Only planets with rings
You will often want to select an entire column, namely one specific variable from a data frame. If you want to select all elements of the variable diameter, for example, both of these will do the trick:
planets_df[,3]
planets_df[,"diameter"]
However, there is a short-cut. If your columns have names, you can use the $ sign:
planets_df$diameter
Instructions
100 XP
•	Use the $ sign to select the rings variable from planets_df. Store the vector that results as rings_vector.
•	Print out rings_vector to see if you got it right.
Take Hint (-30 XP)

# planets_df is pre-loaded in your workspace

# Select the rings variable from planets_df
rings_vector <- planets_df$rings
  
# Print out rings_vector
print(rings_vector)

Only planets with rings (2)
You probably remember from high school that some planets in our solar system have rings and others do not. Unfortunately you can not recall their names. Could R help you out?
If you type rings_vector in the console, you get:
[1] FALSE FALSE FALSE FALSE  TRUE  TRUE  TRUE  TRUE
This means that the first four observations (or planets) do not have a ring (FALSE), but the other four do (TRUE). However, you do not get a nice overview of the names of these planets, their diameter, etc. Let's try to use rings_vector to select the data for the four planets with rings.
这意味着前四个观测(或行星)没有环(假)，但其他四个有环(真)。然而，你并不能很好地了解这些行星的名字，它们的直径等等。让我们尝试使用rings_vector来为有光环的四颗行星选择数据。
Instructions
100 XP
The code on the right selects the name column of all planets that have rings. Adapt the code so that instead of only the name column, all columns for planets that have rings are selected.
右边的代码选择所有有光环的行星的名称列。调整代码，这样就可以不选择name列，而是选择所有具有光环的行星的列。
Take Hint (-30 XP)

# planets_df and rings_vector are pre-loaded in your workspace

# Adapt the code to select all columns for planets with rings
planets_df[rings_vector, ]

Only planets with rings but shorter
So what exactly did you learn in the previous exercises? You selected a subset from a data frame (planets_df) based on whether or not a certain condition was true (rings or no rings), and you managed to pull out all relevant data. Pretty awesome! By now, NASA is probably already flirting with your CV ;-).
Now, let us move up one level and use the function subset(). You should see the subset() function as a short-cut to do exactly the same as what you did in the previous exercises.
现在，让我们向上移动一层并使用函数subset()。您应该将subset()函数视为实现与前面的练习完全相同功能的捷径。
subset(my_df, subset = some_condition)
The first argument of subset() specifies the data set for which you want a subset. By adding the second argument, you give R the necessary information and conditions to select the correct subset.
subset()的第一个参数指定您想要子集的数据集。通过添加第二个参数，您可以为R提供必要的信息和条件来选择正确的子集。
Subset()函数一共有两个参数，第一个参数是想调用的数据集的名称，第二个参数是筛选所必要的信息/条件。举例：subset(planets_df, subset = rings)

The code below will give the exact same result as you got in the previous exercise, but this time, you didn't need the rings_vector!
下面的代码将给出与前一个练习完全相同的结果，但是这一次，您不需要rings_vector!
subset(planets_df, subset = rings)
Instructions
100 XP
Use subset() on planets_df to select planets that have a diameter smaller than Earth. Because the diameter variable is a relative measure of the planet's diameter w.r.t that of planet Earth, your condition is diameter < 1.
Take Hint (-30 XP)

# planets_df is pre-loaded in your workspace

# Select planets with diameter < 1
subset(planets_df,diameter<1)

Great! Not only is the subset() function more concise, it is probably also more understandable for people who read your code. Continue to the next exercise.
太棒了!子集()函数不仅更简洁，而且对于阅读代码的人来说也更容易理解。继续下一个练习。

Sorting
排序
Making and creating rankings is one of mankind's favorite affairs. These rankings can be useful (best universities in the world), entertaining (most influential movie stars) or pointless (best 007 look-a-like).
排名和创造排名是人类最喜爱的事情之一。这些排名可以是有用的(世界上最好的大学)，娱乐的(最具影响力的电影明星)，也可以是毫无意义的(看起来像007的最佳演员)。
In data analysis you can sort your data according to a certain variable in the data set. In R, this is done with the help of the function order().
在数据分析中，可以根据数据集中的某个变量对数据进行排序。在R中，这是在order()函数的帮助下完成的。
order() is a function that gives you the ranked position of each element when it is applied on a variable, such as a vector for example:
order()是一个函数，当它应用于一个变量(例如一个向量)时，它会给出每个元素的排名位置:
> a <- c(100, 10, 1000)
> order(a)
[1] 2 1 3
(注意：排序是通过从小到大的顺序生成的，order(a)的意思是，对矢量(vector)a中的元素进行排序，从小到大分别是1，2，3，。。。。)
10, which is the second element in a, is the smallest element, so 2 comes first in the output of order(a). 100, which is the first element in a is the second smallest element, so 1 comes second in the output of order(a).
This means we can use the output of order(a) to reshuffle a:
这意味着我们可以使用(a)的输出来重新洗牌a

> a[order(a)]
[1]   10  100 1000

A                  （ a[order(a)]使得对矢量a进行从小到大排序。）
Instructions
100 XP
Experiment with the order() function in the console. Click 'Submit Answer' when you are ready to continue.
Take Hint (-30 XP)

（此处没有写代码要求，只要求看代码）
（此处没有写代码要求，只要求看代码）

Sorting your data frame
对数据帧进行排序
Alright, now that you understand the order() function, let us do something useful with it. You would like to rearrange your data frame such that it starts with the smallest planet and ends with the largest one. A sort on the diameter column.
好了，现在您已经理解了order()函数，让我们对它做一些有用的事情。你想要重新安排你的数据框架，使它以最小的行星开始，以最大的行星结束。在直径列上排序。
Instructions
100 XP
•	Call order() on planets_df$diameter (the diameter column of planets_df). Store the result as positions.
•	Now reshuffle planets_df with the positions vector as row indexes inside square brackets. Keep all columns. Simply print out the result.
•	
•	•调用planets_df$diameter (planets_df的直径列)上的order()。将结果存储为位置。
•	
•	•现在用方括号内的位置向量作为行索引重新洗牌planets_df。保持所有列。只需打印出结果。
Take Hint (-30 XP)

# planets_df is pre-loaded in your workspace

# Use order() to create positions
positions <-  order(planets_df$diameter)

# Use positions to sort planets_df
planets_df[positions, ]

（备注：Use planets_df[positions, ] to sort planets_df; the comma inside the square brackets is crucial!
使用planets_df[position，]对planets_df进行排序;方括号内的逗号很重要!
poker_vector[1].表示选择poker_vector矢量的第一个变量
•	my_matrix[,1] selects all elements of the first column.
•	my_matrix[1,] selects all elements of the first row.
对于矩阵而言，空格表示选择该行或者该列的所有。1：3/1，2，3表示从第一行/列到第三行/列）






 
Chapter 6
6 Lists
Lists, why would you need them?
Congratulations! At this point in the course you are already familiar with:
•	Vectors (one dimensional array): can hold numeric, character or logical values. The elements in a vector all have the same data type.
•	Matrices (two dimensional array): can hold numeric, character or logical values. The elements in a matrix all have the same data type.
•	Data frames (two-dimensional objects): can hold numeric, character or logical values. Within a column all elements have the same data type, but different columns can be of different data type.
Pretty sweet for an R newbie, right? ;-)
Instructions
100 XP
Click 'Submit Answer' to start learning everything about lists!
Take Hint (-30 XP)

（此处没有写代码要求，只要求看代码）
（此处没有写代码要求，只要求看代码）

Lists, why would you need them? (2)
A list in R is similar to your to-do list at work or school: the different items on that list most likely differ in length, characteristic, and type of activity that has to be done.
A list in R allows you to gather a variety of objects under one name (that is, the name of the list) in an ordered way. These objects can be matrices, vectors, data frames, even other lists, etc. It is not even required that these objects are related to each other in any way.
You could say that a list is some kind super data type: you can store practically any piece of information in it!
Instructions
100 XP
Click 'Submit Answer' to start the first exercise on lists.
Take Hint (-30 XP)

（此处没有写代码要求，只要求看代码）
（此处没有写代码要求，只要求看代码）

Creating a list
Let us create our first list! To construct a list you use the function list():
my_list <- list(comp1, comp2 ...)
The arguments to the list function are the list components. Remember, these components can be matrices, vectors, other lists, ...
Instructions
100 XP
Construct a list, named my_list, that contains the variables my_vector, my_matrix and my_df as list components.
Take Hint (-30 XP)

# Vector with numerics from 1 up to 10
my_vector <- 1:10 

# Matrix with numerics from 1 up to 9
my_matrix <- matrix(1:9, ncol = 3)

# First 10 elements of the built-in data frame mtcars
my_df <- mtcars[1:10,]

# Construct list with these different elements:
my_list <-list(my_vector,my_matrix,my_df)

Creating a named list
Well done, you're on a roll!
Just like on your to-do list, you want to avoid not knowing or remembering what the components of your list stand for. That is why you should give names to them:
my_list <- list(name1 = your_comp1, 
                name2 = your_comp2)
This creates a list with components that are named name1, name2, and so on. If you want to name your lists after you've created them, you can use the names() function as you did with vectors. The following commands are fully equivalent to the assignment above:
my_list <- list(your_comp1, your_comp2)
names(my_list) <- c("name1", "name2")
(改名字的话使用names函数，names(目标矢量)<- c("name1", "name2"))
Instructions
100 XP
•	Change the code of the previous exercise (see editor) by adding names to the components. Use for my_vector the name vec, for my_matrix the name mat and for my_df the name df.
•	Print out my_list so you can inspect the output.
Take Hint (-30 XP)

# Vector with numerics from 1 up to 10
my_vector <- 1:10 

# Matrix with numerics from 1 up to 9
my_matrix <- matrix(1:9, ncol = 3)

# First 10 elements of the built-in data frame mtcars
my_df <- mtcars[1:10,]

# Adapt list() call to give the components names
my_list <- list(my_vector, my_matrix, my_df)
names(my_list) <- c("vec", "mat","df")
# Print out my_list
print(my_list)

Creating a named list (2)
Being a huge movie fan (remember your job at LucasFilms), you decide to start storing information on good movies with the help of lists.
Start by creating a list for the movie "The Shining". We have already created the variables mov, act and rev in your R workspace. Feel free to check them out in the console.
Instructions
100 XP
Complete the code on the right to create shining_list; it contains three elements:
•	moviename: a character string with the movie title (stored in mov)
•	actors: a vector with the main actors' names (stored in act)
•	reviews: a data frame that contains some reviews (stored in rev)
Do not forget to name the list components accordingly (names are moviename, actors and reviews).
Take Hint (-30 XP)

# The variables mov, act and rev are available

# Finish the code to build shining_list
shining_list <- list(moviename = mov,actors=act,reviews=rev)

Selecting elements from a list
Your list will often be built out of numerous elements and components. Therefore, getting a single element, multiple elements, or a component out of it is not always straightforward.
One way to select a component is using the numbered position of that component. For example, to "grab" the first component of shining_list you type
shining_list[[1]]
shining_list[[1]]
取出shining list的第一个元素
A quick way to check this out is typing it in the console. Important to remember: to select elements from vectors, you use single square brackets: [ ]. Don't mix them up!
请注意区分单括号的[ ]和双括号的[[1]]
单括号用于从vector矢量中提取元素，不要搞混了。

You can also refer to the names of the components, with [[ ]] or with the $ sign.
您还可以使用[[]]或$符号来引用组件的名称。
 Both will select the data frame representing the reviews:
shining_list[["reviews"]]
shining_list$reviews
Besides selecting components, you often need to select specific elements out of these components. For example, with shining_list[[2]][1] you select from the second component, actors (shining_list[[2]]), the first element ([1]). When you type this in the console, you will see the answer is Jack Nicholson.
除了选择组件外，您通常还需要从这些组件中选择特定的元素。例如，使用shining_list[[2]][1]从第二个组件中选择actors (shining_list[[2]])和第一个元素([1])。当您在控制台中键入这个时，您将看到答案是Jack Nicholson。
Instructions
100 XP
•	Select from shining_list the vector representing the actors. Simply print out this vector.
•	Select from shining_list the second element in the vector representing the actors. Do a printout like before.
Take Hint (-30 XP)

For example, with shining_list[[2]][1] you select from the second component, actors (shining_list[[2]]), the first element ([1]).

# shining_list is already pre-loaded in the workspace

# Print out the vector representing the actors
shining_list[["actors"]]
print(shining_list[["actors"]])

在此应该可以使用这两种表达方式：从shining_list中选出
print(shining_list[["actors"]])
print(shining_list$actors)

# Print the second element of the vector representing the actors
print(shining_list$actors[[2]])
之前错解：print(shining_list[[2]][1])

Creating a new list for another movie
You found reviews of another, more recent, Jack Nicholson movie: The Departed!
Scores	Comments
4.6	I would watch it again
5	Amazing!
4.8	I liked it
5	One of the best movies
4.2	Fascinating plot
It would be useful to collect together all the pieces of information about the movie, like the title, actors, and reviews into a single variable. Since these pieces of data are different shapes, it is natural to combine them in a list variable.
movie_title, containing the title of the movie, and movie_actors, containing the names of some of the actors in the movie, are available in your workspace.
Instructions
100 XP
•	Create two vectors, called scores and comments, that contain the information from the reviews shown in the table.
•	Find the average of the scores vector and save it as avg_review.
•	Combine the scores and comments vectors into a data frame called reviews_df.
•	Create a list, called departed_list, that contains the movie_title, movie_actors, reviews data frame as reviews_df, and the average review score as avg_review, and print it out.
Take Hint (-30 XP)

# Use the table from the exercise to define the comments and scores vectors
scores <- c(4.6, 5, 4.8, 5, 4.2)
comments <- c("I would watch it again", "Amazing!", "I liked it", "One of the best movies", "Fascinating plot") 

# Save the average of the scores vector as avg_review  
avg_review<- mean(scores)

# Combine scores and comments into the reviews_df data frame
reviews_df<-data.frame(scores,comments)

# Create and print out a list, called departed_list
departed_list<-list(movie_title,movie_actors,reviews_df,avg_review)
print(departed_list)































Chapter 1
Chapter 1






