# symmetrical-enigma

# Terminal commands 
~ # means home  
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

| # pipe operator, uses the last output as the input for the next command, example: grep line copy_me.txt | wc -l # shows the word count of the lines found with the keyword "line" in them



# R commands
getwd () # get working directory   
matrix(c(), ncol = X, byrow = TRUE) # creates a matrix with X columns, fill by row (byrow = TRUE) with the items inside the combine command.  
c() # combine into a vector or list; concatenate   
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

