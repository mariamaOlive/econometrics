# You can learn more about package authoring with RStudio at:
#
#   http://r-pkgs.had.co.nz/
#
# Some useful keyboard shortcuts for package authoring:
#
#   Install Package:           'Cmd + Shift + B'
#   Check Package:             'Cmd + Shift + E'
#   Test Package:              'Cmd + Shift + T'


#Reading data from file
peopleData <-read.table("/Users/mariamaoliveira/Desktop/econometrics-coursera/project1/TrainExer11.txt", header = TRUE)

#Plot scatterplot Age vs Expenditures
ggplot(data = peopleData) +
  geom_point(mapping = aes(x = Age, y = Expenditures))

#Plot histogram Age
ggplot(peopleData, aes(Age)) +
  geom_bar() +
  scale_x_binned()

#Plot histogram Expenditure
ggplot(peopleData, aes(Expenditures)) +
  geom_bar() +
  scale_x_binned()

#Calculate the mean of the sample of expenditure
sampleMean <- mean(peopleData$Expenditures)
print(sampleMean)

#Calculate the mean of two samples clientes over forty and clients below forty
sampleMeanOver40 <- mean(peopleData$Expenditures[peopleData$Age>=40])
print(sampleMeanOver40)

sampleMeanUnder40 <- mean(peopleData$Expenditures[peopleData$Age<40])
print(sampleMeanUnder40)

