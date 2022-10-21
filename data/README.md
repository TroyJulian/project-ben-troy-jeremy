# data

Place data file(s) in this folder.

```{r cars}

colors <- c("blue", "yellow", "green", "orange", "brown", "black", "white", "purple", "red", "tan")
dates <- c("2010", "2011", "2012", "2013", "2014", "2015", "2016", "2017", "2018", "2019")
sizes <- c("S", "M", "L", "XL")
need_to_have <- c("yes", "no")
season <- c("Winter", "Spring", "Summer", "fall")
type <- c("pants", "shorts", "shirts", "jackets", "sweaters", "socks", "underwear", "hats", "shoes", "dresses")
state_of_repair <-c("very good", "good", "fiar", "poor", "very poor")
sentimental_value <-c("yes", "no")
material <- c("wool", "cotton", "Polyester", "leather")



clothes_use <- data.frame(
  "Asset ID" = 1:100,	
  "Type" = sample(rep(type, 10, replace = FALSE)),
  "Color" = rep(colors, 10),
  "Acquired date"	= rep(dates, 10), 
  "State of Repair" = rep(state_of_repair, 20), 
  "Size" = rep(sizes, 25), 
  "Need to have" = rep(need_to_have, 50),
  "Season" = rep(season, 25),
  "Sentimental Value" = rep(sentimental_value, 50),
  "Material" = rep(material, 25)
)

write.csv(clothes_use, file = "data/clothes_use.csv")

```
Then, include codebooks (variables, and their descriptions) for your data file(s)
using the following format.

## name of data file

- `variable1`: Description of variable 1
- `variable2`: Description of variable 2
- `variable3`: Description of variable 3
- ...
