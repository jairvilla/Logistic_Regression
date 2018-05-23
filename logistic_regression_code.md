# Logistic_Regression
# This is a practical Logistic regression. 
# dataset: OSA patients, Variables related to sleep disorder 
# dataset: dtreat.xlxs

# Determine row to split on
set.seed(456)
split <- round(nrow(dtreat3)*.70)  ## dtret3 omited NA values 

# Create train set
train <- dtreat3[1:split,]

# Create test 
test<- dtreat3[(split + 1):nrow(dtreat3), ]

