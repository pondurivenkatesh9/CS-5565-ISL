college <-read.csv("college.csv")
print(college)
head(college[, 1:5])
rownames <- college[, 1]
college <- college[, -1]
head(college[, 1:8])
summary(college)
pairs(college[, 1:5])
plot(college$Outstate, college$Private, xlab = "Out of State tuition in USD", ylab ="Private University", main = "Outstate Tuition Plot")
boxplot(college$Outstate, college$Private, xlab = "Out of State tuition in USD", ylab ="Private University", main = "Outstate Tuition Plot")
Elite <- rep("No", nrow(college))
Elite[college$Top10perc > 50] <- "Yes"
Elite <- as.factor(Elite)
college$Elite <- Elite
summary(college$Elite)
plot(college$Elite, college$Outstate, xlab = "Elite", ylab ="Out of State", main = "Outstate Tuition Plot")
par(mfrow = c(2,2))
hist(college$Apps, col = 2, xlab = "Apps", ylab = "Count")
hist(college$Enroll, col = 5, xlab = "Enroll", ylab = "Count")
hist(college$PhD, col = 4, xlab = "PhD", ylab = "Count")
hist(college$perc.alumni, col = 8, xlab = "% alumni", ylab = "Count")
summary(college$Books)
No.Books <- college[college$Books == 2000, ]
nrow(No.Books)
rownames[as.numeric(rownames(No.Books))]

