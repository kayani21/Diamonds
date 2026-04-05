# Load the diamonds dataset
data("diamonds")

# Check structure and summary statistics 
str(diamonds)

summary(diamonds)
## Introduction

This project analyzes the **diamonds dataset** from the 'ggplot2' package.  
The dataset contains approximately **54,000 diamonds**, with attributes such as:

- `price`: The price of the diamond in US dollars.  
- `carat`: The weight of the diamond.  
- `cut`: The quality of the diamond's cut (Fair, Good, Very Good, Premium, Ideal).  
- `color`: The diamond's color grade, ranked from **D** (best) to **J** (worst).  
- `clarity`: The number of inclusions and blemishes in the diamond.  

## Including Plots
## Bar Chart of Diamond Cut

ggplot(data = diamonds) + 
  geom_bar(mapping = aes(x = cut))

ggplot(data = diamonds) + 
  geom_bar(mapping = aes(x = cut, y = after_stat(prop), group = 1))

ggplot(data = diamonds) + 
  geom_bar(mapping = aes(x = cut, fill = clarity))

ggplot(data = diamonds) + 
  geom_bar(mapping = aes(x = cut, fill = clarity))

  ggplot(data = diamonds) + 
  geom_bar(mapping = aes(x = cut, fill = clarity), position = "fill")

  ggplot(data = diamonds) + 
  geom_bar(mapping = aes(x = cut, fill = clarity), position = "dodge")

  ggplot(data = diamonds) + 
  geom_bar(mapping = aes(x = cut, fill = clarity)) +
  coord_flip()
