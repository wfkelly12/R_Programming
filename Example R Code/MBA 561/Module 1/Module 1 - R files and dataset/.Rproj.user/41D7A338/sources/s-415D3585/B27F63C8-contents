#############GETTING TO KNOW YOUR DATA PART 1#############
# Read in data----
df <- read.csv('jan17Items.csv', stringsAsFactors = F, header = T)
dfw <- read.csv('jan17Weather.csv', stringsAsFactors = F, header = T, sep = '\t')

# Explore Structure of Data Frame----
##Summary of Data
str(df)    # This tells you the structure of the Items dataframe.
str(dfw)   # This tells you the structure of the Weather dataframe.

##Dimensions
dim(df)
dim(dfw)

##Rows
nrow(df)
nrow(dfw)

##Columns
ncol(df)
ncol(dfw)

##Names of Columns
names(df)
names(dfw)

# Referencing and Subsetting vectors by location----
v1 <- c(18:23)
v1[1]
v1[3]
v1[2:4]
v1[c(1,5)]
v2 <- v1[c(1,5)]

# Referencing and Subsetting dataframes by location----
dfw[1:5,1:3]
dfw[1:5,]
dfw[1:5,c(1,3)]
dfw2 <- dfw[,1]

# Referencing and Subsetting dataframes by column name----
dfw$date
dfw[1:5,c('date','PRCP')]
df$BarCode <- NULL

# Explore the shape of the data----
summary(df)
summary(dfw)
summary(df$Price)
summary(df[,c('Price','Cost')])

# Visually Explore shape of the data----
hist(dfw$TMAX)
boxplot(dfw$TMAX)
plot(dfw$TMAX)
?plot
plot(dfw$TMIN,dfw$TMAX)
plot(dfw$TMAX, type = 'l')
plot(dfw[,c('TMIN', 'TMAX', 'PRCP')])


