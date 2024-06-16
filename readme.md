Empirical Question:

Using data from the UN, I wanted to measure the history of aquaculture exploitation from each continent, compare them and measure the trend it will potentially follow in the future.

Methods:
Data was read, and then cleaned, only taking the columns which we wanted.
Since we only cared about the continent, we made a categorical variable which assigned a number to each continent. 1 being Asia, 2 Americas, 3 Oceania, 4 Africa, 5 Europe.
However, the years were X-values while the continent identifiers were y values, so we transposed the dataset.
Taking this transposed dataset, we plotted a combined graph of fishing numbers through the years for each continent.

After achieving this, I tried using Sarimax and Prophet to create a prediction of trend of where the numbers for each continent will go for next year, however I was not able to get it to work.
The dataset separates time series data into separate years and when transposed, I could not change the column years into a format that could be used by the model prediction function. I tried multiple methods to correct this, splitting and remerging the columns, resetting the index of the dataset, etc. but none were successful. The dataset when transposed seems to have made the column of years unable to be edited, which is very puzzling.