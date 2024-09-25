**Quick recap**

Daniel led a session on preparing for a code challenge, covering topics such as list and dictionary structures, interacting with pandas and data frames, and visualization code. The team also discussed handling missing data, feature engineering, and data analysis techniques, including the use of value counts, normalization, and histograms. They also worked on creating visualizations such as bar charts and scatterplots, and explored strategies for extracting track names and artist information from a dataset.

**Next steps**

All students to review the completed version of the notebook posted by Daniel for preparation for the code challenge.

All students to have necessary materials (previous lectures, checkpoints, completed lectures, personal notes) ready for the code challenge tomorrow.

All students to be prepared for pandas operations, descriptive statistics, column manipulation, and visualizations in the code challenge.

All students to be ready for questions on nested data structures at the end of the code challenge.

All students to answer the stand down question poll that Daniel will post in Discord.

Daniel to post the completed version of the notebook in the completed lectures folder.

Daniel to post the recording of the session for students to review.

Students to send any questions that arise to Daniel, even if they come up tonight.

All students to be present for the pre-code challenge session in the morning.

**Summary**

Preparing for Code Challenge and Loading Facebook Data

Daniel led a session on preparing for a code challenge, which would replace the morning lecture. The challenge would cover topics such as list and dictionary structures, interacting with pandas and data frames, and visualization code. Daniel also introduced a special call on function for random student selection and shared a terminal window for the code challenge. He emphasized that the challenge would not cover tableau, as it was a new topic. The session ended with Daniel providing the necessary import for pandas. Daniel guided the team through the process of loading Facebook data into a data frame using pandas. He emphasized the importance of using the correct path and file name. The team successfully loaded the data and observed that the data was not in the expected format, with one column containing all the data that should be in separate columns. Daniel encouraged the team to think about how to separate these columns. Daniel and Jeesoo discussed issues related to reading CSV files. They highlighted the importance of checking the actual CSV file to identify the correct delimiter, which could be a semicolon, comma, or tab. They also mentioned the possibility of encountering a TSV file, which is essentially the same as a CSV file but separated by tabs. Daniel emphasized the need for careful checking and suggested running commands like dot head or dot tail immediately after loading data to ensure accuracy. Jeesoo was asked to handle the next CSV file.

Understanding Data Frames and Column Information

Daniel discussed the importance of understanding the data frame when loading in data. He highlighted the need to look at the information about each column, including null values and data types. He also emphasized the importance of having a holistic view of the data frame, which can be achieved through the use of 'info' and 'describe' functions in pandas. Daniel pointed out that long column names can cause issues with the view, and suggested renaming columns for better clarity. He also noted the presence of null values and the need to investigate the data types, particularly the use of floats and integers. Elijah added that most of the data was numerical, which Daniel agreed with. Daniel also mentioned the need to investigate the binary representation of the 'paid' column and the use of scientific notation in some data.

Handling Numerical Data With Extreme Values

Daniel and Ricky discussed the challenges of dealing with a wide range of numerical data in their analysis, including significant differences in scales and units. They noted the presence of extreme values in their data, which could skew the analysis, and agreed that these extreme values might be desirable in certain contexts. They also discussed handling outliers in data analysis, such as highly successful movies that appear as extreme values. Anbita suggested using filler values such as mean, median, or mode to handle null values, while Daniel proposed using a "reasonable value" or a measure of single tendency. They also considered using the string "missing" to represent unknown values. However, no clear decision was made on which approach to take.

Handling Missing Data in Datasets

Daniel discussed the handling of missing data in datasets. He explained that the decision to drop rows or columns depends on the amount of missing data and the size of the dataset. He emphasized that dropping rows could lead to losing a significant portion of the data, while dropping columns might not be as impactful. Daniel also highlighted the importance of understanding the pattern of missing data and suggested creating an indicator column to carry the information about missing data through the analysis process. He cautioned against blanket filling of missing data, suggesting that it should be done with consideration for the type of data and its impact on the analysis.

Handling Null Values in Dataset Discussion

Daniel and Elijah discussed handling null values in a dataset. They decided to drop rows with null values in the'share' column and considered dropping columns with null values, but focused on rows for now. Daniel demonstrated how to use the 'drop' function in pandas to achieve this and suggested saving the updated dataset under a different name for clarity. Daniel also discussed the use of the 'dropna' function in data manipulation, its default behavior, and how it can be customized. He emphasized the importance of feature engineering in data science and analytics, suggesting the creation of new columns by combining existing features. Daniel also mentioned the concept of polynomials in mathematics and its potential relevance in data manipulation. He concluded by noting the potential need to remove null values after a merge join operation.

Feature Engineering and Data Frame Operations

Daniel led a discussion on feature engineering, using the example of a Celtics analyst who used a linear regression to quantify player interactions. The team then practiced creating new columns in a data frame, such as 'likes per impression' and 'percent of likes per impression'. They also discussed the use of lambda functions and the efficiency of using 'dot map' for certain operations. Lastly, Elif and Daniel worked on counting the examples of each type of post based on the 'type' column.

Data Analysis Techniques and Normalization

Daniel and Ricky discussed data analysis techniques, focusing on categorical data types and the use of value counts. They explored the concept of normalization and its application to data sets. Daniel suggested using a histogram to analyze discrete data types like month. Ricky proposed a method to find the 5 photos with the highest likes per impression ratio, which involved subsetting the data frame to only include photos and then finding the top 5 values. The team agreed on the usefulness of these techniques for their data analysis. They also discussed how to find the highest likes per impression based on a specific column in their data frame, with Ricky suggesting using the'sort\_values' function and setting 'ascending' to False to get the highest values. Anbita asked a question about the 'dot' syntax, but the details of her question were not provided in the transcript.

Exploring Dot Look, Indexing, and Data Visualization

Daniel explained the usage of dot look for finding by index and clarified its differences from normal look. The team discussed using 'ilok' versus 'iloc' in Python for indexing rows in a dataframe. They planned to implement a method to find the most liked photos using the 'max' function. Daniel and Elijah discussed the flexibility of 'look' over 'iloc' for subsetting rows and columns, and the use of 'enlarge' for handling ties. Jeesoo asked about finding the mean of total interactions, and Daniel guided her through the process using 'describe' and 'group by'. They planned to visualize the data using matplotlib.

Creating Bar Chart for Monthly Post Counts

Daniel and Elif discussed creating a bar chart to visualize the number of posts per month. They agreed to use the 'value\_counts' function on the 'post\_month' column to obtain the monthly post counts from a Pandas series. Daniel instructed Elif to create the bar chart using the discussed data and formatting. They also discussed the automatic sorting of data in a graph, with Daniel considering sorting by month or by value, and deciding on the former for better understanding. They also discussed the need for labeling the graph and setting the ticks to show every month. Elif suggested using semicolons to improve the text's appearance. Daniel and Elijah encountered some challenges with the sorting order and the way matplotlib was interpreting the data, but decided to revert to their previous method and explore other options to address the issue.

Scatterplot Creation and Dictionary Exploration

Daniel and Jayla worked on creating a scatterplot to visualize the relationship between total interactions and likes. They successfully created the plot and added a title. They also discussed the concept of loading data from a pickled file, which Daniel mentioned is a way to compress data, particularly models. Daniel and Elijah then discussed how to access and navigate through a dictionary containing data about top 20 songs, identifying the keys and nested structures within the dictionary. They concluded that the 'items' key in the dictionary represents a list of dictionaries, each containing information about a song, and noted the presence of additional keys such as 'albums', 'artists', and 'available markets'. The discussion ended with the understanding that further exploration into the dictionary is necessary to extract the desired song data.

Extracting Track Names and Artist Information Strategies

Daniel, Jeesoo, Anbita, and Ricky discussed strategies for extracting track names and artist information from a dataset. Anbita explained her method of creating a Song Dictionary, where each track name was a key and the value was a tuple of the artists. The team agreed on the effectiveness of Anbita's method and discussed the process of creating a dictionary of song names and artists. They also considered the possibility of writing a function to retrieve a list of songs written by a specific artist from the dictionary. Ricky proposed a method to loop through the dictionary and construct a list of songs for a given artist, which the team agreed to continue working on.

Programming Problem and Code Challenge Discussion

Ricky and Daniel discussed a programming problem involving a tuple, focusing on the need to return the name from the tuple and the challenges of comparing the tuple to a string. They considered using the 'in' operator and a for loop with dot items as potential solutions. They also discussed a method to loop through a dictionary and extract specific information, emphasizing the importance of correctly passing arguments into the function. Daniel hinted at a similar question in an upcoming code challenge and outlined the format of the challenge, which would involve pandas, descriptive statistics, column manipulation, and nested structures. He encouraged the team to take a break and study further if needed, and assured them of his availability for any questions.

