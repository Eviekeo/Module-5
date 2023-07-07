# Module-5

# Description
As part of this module, 249 mice who were identified with SCC tumors received treatment with a range of drug regimens. Tumor development was observed and measured over 45 days to assess the performance of each drug. 
Analysis and outputs have been uploaded in the Jupyter Notebook titled "Module_5_Challenge.ipynb".

# Code source
	  duplicates = combined_study_df[combined_study_df.duplicated(subset=["Mouse ID","Timepoint"])]

The duplicate function was used in the abovecode, to identify any mice that had duplicate timepoints which was then subsequently removed. The code was obtained from the following stack overflow forum:
	  https://stackoverflow.com/questions/46640945/grouping-by-multiple-columns-to-find-duplicate-rows-pandas

	  clean_study_df = combined_study_df.drop(combined_study_df[(combined_study_df["Mouse ID"] == "g989")].index)
	
The drop function in the above code was used to remove the duplicated mouse ID from the dataframe. The code was obtained from the following stack overflow forum: https://stackoverflow.com/questions/71034567/python-pandas-how-can-i-drop-rows-using-df-drop-and-df-loc

	  flierprops = dict(marker='o', markerfacecolor='r', markersize=12,  linestyle='none', markeredgecolor='g')
	  plt.boxplot(Tumor_vol, labels=Drugs_list, flierprops=flierprops)

The above code was used to format and plot the outliers in the boxplot graph. Code source is from the following stack overflow forum: https://stackoverflow.com/questions/43342564/flier-colors-in-boxplot-with-matplotlib![image](https://github.com/Eviekeo/Module-5/assets/132751100/9650ffbc-42b9-4e88-b1d0-388ae3554715)

