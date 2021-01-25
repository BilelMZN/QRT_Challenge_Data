# QRT_Challenge_Data
This repository contains my work on the QRT Data Challenge which aims at predicting the return of a stock in the US market using historical data over a recent period of 20 days. 

3 datasets are provided as csv files, split between training inputs and outputs, and test inputs.

Input datasets comprise 47 columns: the first ID column contains unique row identifiers while the other 46 descriptive features correspond to:

• DATE: an index of the date (the dates are randomized and anonymized so there is no continuity or link between any dates),
• STOCK: an index of the stock,
• INDUSTRY: an index of the stock industry domain (e.g., aeronautic, IT, oil company),
• INDUSTRY_GROUP: an index of the group industry,
• SUB_INDUSTRY: a lower level index of the industry,
• SECTOR: an index of the work sector,
• RET_1 to RET_20: the historical residual returns among the last 20 days (i.e., RET_1 is the return of the previous day and so on),
• VOLUME_1 to VOLUME_20: the historical relative volume traded among the last 20 days (i.e., VOLUME_1 is the relative volume of the previous day and so on),
Output datasets are only composed of 2 columns:

• ID: the unique row identifier (corresponding to the input identifiers)
and the binary target:
• RET: the sign of the residual stock return at time tt
The solution files submitted by participants shall follow this output dataset format (i.e contain only two columns, ID and RET, where the ID values correspond to the input test data). An example submission file containing random predictions is provided.

418595 observations (i.e. lines) are available for the training datasets while 198429 observations are used for the test datasets.

The metric considered is the accuracy of the predicted residual stock return sign.

More details about the data and the csv files can be found on <html> https://challengedata.ens.fr/participants/challenges/23/.
