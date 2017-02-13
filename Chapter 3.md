
###3.2.4 Exercises

**1.Run ggplot(data = mpg) what do you see?**

Nothing just an empty space

**2.How many rows are in mtcars? How many columns?**

```R
str(mtcars)
```

**3.What does the drv variable describe? Read the help for ?mpg to find out.**

```R
?mpg
```
Describes if the car is front wheel drive, rear wheel drive or 4 wheel


**4.Make a scatterplot of hwy vs cyl.**
```R
ggplot(data  = mpg) +
  geom_point(mapping = aes(x=hwy,y=cyl))
```

**5.What happens if you make a scatterplot of class vs drv. Why is the plot not useful?**
```R
ggplot(data  = mpg) +
  geom_point(mapping = aes(x=class,y=drv))
  ```
This plot doesn't help us as it doesn't give any useful information.
 It simply categorises the class of cars into drive type.
  

###3.3.1 Exercises

**1.What’s gone wrong with this code? Why are the points not blue?
```R
ggplot(data = mpg) + 
  geom_point(mapping = aes(x = displ, y = hwy, color = "blue"))
  ```

The points aren't blue because the aesthetic function is basing the colour of the points on the variable "blue"(which doesn't exist) not the colour blue.
If you want all the point to be blue the arguement "color=blue" needs to be placed outside the aes() function.






Which variables in mpg are categorical? Which variables are continuous? (Hint: type ?mpg to read the documentation for the dataset). How can you see this information when you run mpg?

Map a continuous variable to color, size, and shape. How do these aesthetics behave differently for categorical vs. continuous variables?

What happens if you map the same variable to multiple aesthetics?

What does the stroke aesthetic do? What shapes does it work with? (Hint: use ?geom_point)

What happens if you map an aesthetic to something other than a variable name, like aes(colour = displ < 5)?

3.4 Common 
