---
title: "Developing Data Product Week2 Assignment - Map by Leaflet"
output: html_document
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = FALSE)
```


```{r library, warning=FALSE}
library(leaflet)
```

## 2019.01.23
```{r mapCreate, echo = FALSE}
my_map <- leaflet() %>%
  addTiles()
my_map <- my_map %>%
  addMarkers(lat=47.507, lng=19.046, label = "Parlament", labelOptions = labelOptions(noHide = TRUE))
my_map <- my_map %>%
  addCircles(lat=47.507, lng=19.046, weight = 1, radius =  100)
my_map
```
