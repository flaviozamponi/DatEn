# DatEn  
Miscellaneous collection of my Data Engineering activities.  
I tried to put some of the pieces of code I used to connect to a server, get data, perform data cleaning, store data on a database.  

I always used Jupyter notebooks for my work. Nevertheless, servers do prefer plain python files. So I used the trick of Jeremy P. Howard (fast.ai) to conjugate the advantages of a notebook with the frugality of the plain .py file: the script `notebook2script.py` converts from-top-to-bottom the code of a noteboook into a python file. The appealing feature is that only those cells beginning with '#export' are exported. That means, you can use the power and clarity of the notebook to perform tests, debug, etc. but you take only the relevant cells to the .py file!

Here below, I put some comments to the notebooks you will find in the repository:

* `DataFromEcondaSalesforce_toPostgresql.ipynb`. It collects data from an existing report in Econda via RestAPI to fill a pandas DataFrame. Similarly, it gets data from a Salesforce .csv report file to fill a second DataFrame. The two are joined and the results are stored in a Postgresql table.

* `DataFrom_ATInternet.ipynb`. Very similar to the previous notebook but now the data are taken from an account of AT Internet.

* `HarvestAPI_Interactions.ipynb`. In my old company Harvest was used to account the amount of hours used for the different projects. The notebook here is a small collection of typical activities: if a new colleague comes to the group copy the activities of an existing account into the new one, rename some prejects, etc.
