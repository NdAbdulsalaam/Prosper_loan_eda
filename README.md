## Investigation Overview
In this investigation, I wanted to look at the features of prosper loan that could be used to predict their delinquency. The main focus was on the prosper rating, monthly income, occupation, and employment status

## Dataset Overview
This data set includes customers who have paid off their loans, who have been past due and put into collection without paying back their loan and interests, and who have paid off only after they were put in collection. The original dataset contains 113937 rows and 81 columns out of which 12 features of intrest were selected.Eight hundred and seventy-one data points were removed from the analysis due to inconsistencies or missing information.

## Exploratory Analysis
The original dataset contains 113937 rows and 81 columns out of which 12 features of intrest were selected. After the dataset was loaded, this dataset contains 113937 rows and 12 columns, 113066 rows and 12 columns before and after cleaning respectively. Most of the variables are either numeric or string in nature, ListingDate is datetime and ProsperScore variable is ordered factor variable with the score ranges from 1-10, with 10 being the best, or lowest risk score

The dataset contain duplicated observattions and were removed. The outliers were also removed and log transformation was carried out on some variables.

The explanatory analysis is in three sections: univariate, bivariate and multivariate

## Explanatory_Analysis
Borrowers has an Alpha Prosper Rating of A, B, C and D (17.13%, 18.30%, 21.55%, 16.87%) these translate to 2.00–3.99%, 4.00–5.99%, 6.00–8.99%, 9.00–11.99% Estimated Average Annual Loss Rat respectively. The largest value, 21.55%, is observed at C Rating. This implies that investor, on average stands a risk of not bein paid back by 4% - 8% which a good risk to take

Most of the varibles are negatively correlated with delinquencies, Borrower's rate, however, is possively correlated with delinquencies wich is also much more expected. This implies that as these variables increase, the probability that the borrower won't pay back decreases and vice versa

Observing the first four high ratings, AA A, B, and C, majority of the borrowers are house owners while the reverse is for low ratings, D and E.

Prosper rating AA is commonly associated with high monthly income and low delinqueny. The reverse is seen for rating E. While rating B is somehow evenly distributed.
Borrowers with good prosper rating, AA, borrow less frequently and rearly default. The opposite is true for those with bad or poor rating, E and HR. The same logic hold for other ratings as well

Looking at this relatonship, it is logic to think that because this people earn good income, they don't usually borrow. Perhaps they do when they plan to carryout an important project such as buuilding a house and they are able to pay back when they are done with such a project. Less wonder while this kind of borrower always demand for long term loans.


## Conclusions
From the insights above, it is save to conclude that the monthly income, loan amount and borrower rate is a good predictor of the prosper rating with the later being a good predictor of delinquency.
