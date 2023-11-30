# symmetrical-enigma

# Terminal commands 
~ # means home  
mkdir # make new working directory
cd # change working directory  
pwd # print working directory   
absolute file path can be used from anywhere; relative must be specific (utilizes .. cd)  
cp # copy   
ls # list the contents of the directory   
wc # word count   
head # shows the top lines, use n -2 for the top two lines     
tail # shows the last lines, use n -2 for the last two lines     
grep # searches for the lines that contain a specific keyword     
less # read the whole file, show all the data   
nano # allows you to edit the whole text file  
echo # repeats what the previous command's output was

| # pipe operator, uses the last output as the input for the next command, example: grep line copy_me.txt | wc -l # shows the word count of the lines found with the keyword "line" in them



# R commands
getwd () # get working directory   
matrix(c(), ncol = X, byrow = TRUE) # creates a matrix with X columns, fill by row (byrow = TRUE) with the items inside the combine command.  
c() # combine into a vector or list; concatenate   
head(data_name)  # shows first 6 rows of data, tail(data_name) shows the last 6 rows   
names(data_names) # shows the names of the variables  
summary(data_name) # shows the five-number summary of the dataset   
table(data_name$variable_name) # creates a table of the specified variable   
sd(dat_name$variable_name) # standard deviation   
var(data_name$variable_name) # variance  
IQR(data_name$variable_name)  # interquartile range   
hist(data_name$variable_name, breaks =, xlab = "", ylab = "", main = "")
boxplot(data_name$variable_name) or boxplot(quantitative_variable_name ~ categorical_variable_name, data = data_name) # creates a boxplot  
pnorm(q, mean = , sd = ) [default is lower.tail = T) # for X~N(mean, sd) to get P(X < q), to get X > q set lower.tail = F  
x = rnorm(n =, mean = , sd =,) # randomly generate a sample of n observations from N(mean, sd)  
pbinom(k, size = n, prob = p) # find the proportion of the Bin(n, p) distribution that is less than or equal to k, set lower.tail = F to find the proportion above k  
dbinom(k, size = n, prob = p) # input the number of success k in dbinom() to obtain probability values if X ~ Bin(n, p), find P(X=x)  
sum() # adds up whatever is inside the parentheses  
dir.create() # makes a new directory inside current working directory, need to include the new name   
abs() # takes absolute value of whatever is inside the parentheses  
log() # takes the natural logarithm of whatever is inside of the parentheses  
colSums() # sums the columns inside the table   
rownames() # alters row names, colnames() alters column names   
data.frame() # creates a new data frane; like a matrix but more flexible and may have different types of data   
ggplot(framename.df, aes(x = Xlabel, y = ylabel, fill = maintitle)) + geom_bar(stat = ) # creates a stacked bar plot with source of the data framename.df, aesthetics (x label, y label, main titles)   
merge() # merges multiple data files into one 
combine() # 
head() # shows the heading lines of the data, top lines
read.table() # imports tables   
intersect() # finds data from 2+ datasets that are the same   
as.matrix() # creates a matrix from the data   
shapiro.test() # creates a Shapiro-Wilk normality test, p-values less than 0.1 indicate the data are significantly different   
wilcox.test() # Wilcoxon Rank-Sum test, tests for differences in the data, does not require a normal distribution   
names() <- c() # renames the dataset column names     
for(i in 1:(length(groups)-1)){ # Set 2 counters, 'i' starts at 1 and goes until one less than the number of groups; 'j' will start at 2, and go up tot he full number of groups
  for(j in (i+1):length(groups)){
    # Use this to pick the groups assigned to 'i' 
    ix.metric.i <- metadata$BodySite == groups[i]
    # use this to pick the groups assigned to 'j'
    ix.metric.j <- metadata$BodySite == groups[j]
    # stores the p-value from the test 
    pvalue <- wilcox.test(alpha[ix.metric.i, "shannon"],
                          alpha[ix.metric.j, "shannon"])$p.value
    # appends the new p-value to the list 
    pw.pvalues <- c(pw.pvalues, pvalue)
    # sets the names of the groups tested
    test.name <- paste(groups[i], "_vs_", groups[j], sep = '')
    # appends the names of the groups tested to the list 
    pw.names <- c(pw.names, test.name)
  }
}
names(pw.pvalues) <- pw.names  
p.adjust(dataname, 'fdr') # corrects for type I errors (false positives)






