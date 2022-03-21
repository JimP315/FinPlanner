# In the personal savings section we are wanting to get the total savings of the crypto combined with the share investments. 
# We are also wanting to get an idea of whether the amount saved will suffice for emergency, ie rainy day purposes
# By calling in some if statements we are determining whether he has enough funds to provide for 3 months of emergency situation.  
# this seems to be the case, and yet we tested for whether the amount would be equal to 3 months, or whether it would be insufficient. 
# You could plug in a large figure say 30 or 50 months and see whether there was sufficient emergency funds based on some risk protection, for instance if unable to work for a time. 


# For the Monte Carlo sim I have decided to use most up to date data - so 5 years from last week.
# We have had a number of errors experienced and this is the lesson to note that with alpaca changes recently we needed a different system for getting in the data on the indexes.  No longer is it barset but bars for the import of the data and now that we have had this explained the data seems to run well again. 
# With the Retirement Planning it is important to note that compounding is the key and that it takes time
# this means that trying to short cut the process means that you miss out on compound opportunities.
# We are looking at a comparison of retirement planning for a normal working life ie say 30 years vs bringing forward, ie 5-10 years

## Had an error as it relates to the data that MC Simulation is expecting.  As such we now need to use get bars not get barset.  This is a recent change within Python and Alpacaenv and it will then allow the code to run without the 403 Error encountered before. 
## This also will not convert data into a format that MC Simulation expects.  It is done via a Concat since it will allow the ticker codes to be in the required format, rather than be returned row by row they are set by column, and the data that relates to each index is a sub header ie open close etc....
# as such we are trying to address the tradeoff between compounding over time vs, making up for lost time. It is difficult to make up for lost time, ie compound growth needs to be your friend and therefore you have to give it time. 