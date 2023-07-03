# matplotlib-challenge
Module 5 Challenge
Submission contains:

Final.ipynb in main folder

Mouse_metadata.csv and Study_results.csv in Data folder

Code "flierprops = dict(markerfacecolor="red", markersize=14" to change format of outlier on boxplot came from StackOverflow at https://stackoverflow.com/questions/65648502/how-to-change-outlier-point-symbol-in-python-matplotlib-pyplot

The following code came from Sathwick from AskBCS:

dup_values = combined_data.loc[combined_data.duplicated(subset = ["Mouse ID", "Timepoint"]), "Mouse ID"].unique()
duplicated_values = combined_data[combined_data["Mouse ID"] == "g989"]
tidy_data = combined_data[combined_data["Mouse ID"].isin(dup_values) == False]
len(tidy_data["Mouse ID"].unique())
outliers = tumor_vol.loc[(tumor_vol < LB) | (tumor_vol > UB)]

