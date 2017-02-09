
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
  This plot doesn't help us tell the performance of the cars, it simply categorises the class of cars into drive.
  
