The Jupyter notebook reads the data from "Credit Card Comparison Data.xlsx" that contains details regarding a list of credit cards. 

For the tool to be useful to you, you should adjust the data in the Excel file to be personalized based on your spending habits: 
1) identify which cards you own (you may need to add credit card data if I did not include it in my list) - "Card Data" worksheet: column C
2) in each of the merchant categories (affects cash back/rewards points) - "Personal Spending" worksheet: rows 2-3
3) based on vendors' credit card company acceptance (i.e. Amex and Discover may be less widely accepted vs Visa/Mastercard in the places that you frequent) - "Personal Spending" worksheet rows 4-7
4) valuation of the benefits associatd with each card - "Card Data" worksheet: columns Q-R


After personalizing the input data, you should update cell #2 of the Jupyter Notebook if you have modified any file names or column names from the default.

Now you can run the notebook! (Cell in the header > Run All) 

There are immediate function definitions and outputs if you are interested in getting a breakdown of the value currently provided by the cards that you currently own or want to know the best card in each spending category, but the most valuable information is contained in the last two cells. Each cell will output a DataFrame (aka table), that sorts all unowned cards based on the value that they provide and decompose that valuation based on sign-up bonus, rewards in spending categories, annual fees, etc. The difference between the two outputs is that the first one sorts by marginal value of cards in the first year, which is greatly influenced by sign-up bonuses and the second one sorts by marginal value of cards in all subsequent years, which is mainly driven by benefits and spending in merchant categories. If you would prefer to view this in an Excel file, you can uncomment out the code about these cells to write data to a file called "Incremental Value Output.xlsx"
