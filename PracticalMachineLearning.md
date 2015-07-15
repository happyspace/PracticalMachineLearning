# Practical Machine Learning
Eddie Warner  

## Synopsis

Human activity recognition - HAR - examines data gathered through monitors like *Jawbone Up*, *Nike FuelBand*, *Fitbit*, *Apple Watch*, *Basis Peak* etc. to quantify activity to address any number of applications.  Applications include, energy expenditure for weight-loss programs, monitoring of the elderly and monitoring fitness activity of a person or population to reach fitness goals. A novel question posed by the data set examined by this anlysis **Weight Lifting Exercises Dataset** is if training or qualitative measure like training can measured through the data. For a more complete description for the questions that initialed the study 



## Data Processing


```r
file.name.train <- "pml-training.csv"
file.url.train <- "https://d396qusza40orc.cloudfront.net/predmachlearn/pml-training.csv"

file.name.test <- "pml-testing.csv"
file.url.test <- "https://d396qusza40orc.cloudfront.net/predmachlearn/pml-testing.csv"

if(!file.exists(file.name.train)) {
    download.file(url = file.url.train, destfile = file.name.train)
}

if(!file.exists(file.name.test)) {
    download.file(url = file.url.test, destfile = file.name.test)
}

train_data <- as.data.table(read.csv(file.name.train, stringsAsFactors=FALSE, strip.white=TRUE))

test_data <- as.data.table(read.csv(file.name.test, stringsAsFactors=FALSE, strip.white=TRUE))
```

## Data Exploration

## Analysis

## References

## Appendix


