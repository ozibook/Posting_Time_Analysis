# Posting Time Analysis

## Task Description
The goal of this task is to conduct a comprehensive analysis of the posting times of our competitors' LinkedIn content. By examining the correlation between post timestamps and key engagement metrics such as likes, comments, and engagement rate, this analysis aims to provide valuable insights into the optimal timing for sharing LinkedIn posts. The primary objective is to determine when our company's LinkedIn posts are most likely to resonate with the audience and achieve higher levels of engagement. This research will enable us to make informed decisions about the timing of our LinkedIn content sharing, ultimately enhancing our outreach and impact within the LinkedIn community.

[Go to the notion page for detail understanding of the task↗️](https://docs.google.com/document/d/1lpqrSfYIm4M5RGakFS-gzObmP9jVybTxDKrgsuAAelc/edit#heading=h.7ivjt4pr8s80)

## Task Objective🎯
The Objective of this task is to determine the optimal time slots for posting on LinkedIn based on data-driven analysis and experiments for Ozigen.

## File Details📁
### 1. **Timestamp-Extractor.ipynb** :

 <details>
 <summary>
  Code Explanation
 </summary>
 

### 1. Excel File Format:
File Type: Ensure the file you want to process is in .xlsx format.

Columns:

URL: This column should contain URLs with embedded 19-digit post IDs. The code in this notebook will extract these post IDs to derive timestamps.

Sample Excel File Structure:

URL
[Go to File↗️](https://example.com/post/1234567890123456789)

### 2. Using the Code in This Notebook:
Navigate to the cell containing the line:

input_file = "trial.xlsx"

Modify this line to point to the path of your Excel file. For example:

input_file = "path_to_your_file.xlsx"
- [Go to File↗️](https://drive.google.com/file/u/0/d/1C8d5gYXj38MtC7MrWZBh_WZrp07EfvSZ/edit)
### 3. Running the Code:
Execute the cell containing the code by selecting it and pressing Shift + Enter.

### 4. Checking the Results:
After the cell execution completes, open the Excel file you provided.

You should now see the 'Timestamp UTC' and 'Timestamp IST' columns populated with the extracted timestamps in human-readable date formats for each URL in the 'URL' column.

### 5. Notes:
* The code assumes that the URLs in the 'URL' column contain a 19-digit post ID from which a Unix timestamp can be extracted.

* The extracted Unix timestamp is then converted to human-readable date formats in both UTC and IST.

* The updated data is saved back to the original Excel file.

### 6. Code:
Extracting Timestamps of Posts
![image](https://github.com/ozibook/Posting_Time_Analysis/assets/144370840/b4dd6bee-2614-4a84-b81c-6d617e43644d)
</details>

### 2. **Automated_Time_Analysis.ipynb**
 <details>
 <summary>
  Code Explanation
 </summary>

  ### 

1. This Python script imports necessary modules: `re` for regular expressions, `datetime` for working with dates and times, `pandas` as `pd` for data manipulation. It defines functions for extracting a post ID from a URL, converting      the ID to a Unix timestamp, and converting a Unix timestamp to a human-readable date in either UTC or IST timezones.
2. The `process_xlsx_file` function processes a given DataFrame, adding 'Timestamp UTC' and 'Timestamp IST' columns, and populates them by extracting post IDs from the 'URL' column. Finally, it applies the `process_xlsx_file` function    to a DataFrame named `df_merged`, producing a new DataFrame `result_df` with additional timestamp information in both UTC and IST, which can be used for further analysis or display.
 
  ![image](https://github.com/ozibook/Posting_Time_Analysis/assets/144370840/76280690-2515-4ee5-ad43-51b1fe21228f)
</details>



3. This code snippet imports the `datetime` module, which is used to work with date and time data. It modifies the 'Timestamp IST' column in the `df_merged` DataFrame by applying a lambda function that removes the ' IST' substring from each element in the column. This effectively cleans the data.
4. Next, it converts the modified 'Timestamp IST' column to a Pandas datetime format. The `pd.to_datetime` function is used with the specified format to parse the date and time values from the column strings and convert them into datetime objects. After executing these lines of code, the 'Timestamp IST' column in `df_merged` will contain datetime objects instead of strings, making it easier to work with and analyze time-related data.

![image](https://github.com/ozibook/Posting_Time_Analysis/assets/144370840/1dd54eac-67f6-46ca-b433-2f176b2f48ea)
</details>

5. DataFrame will be sorted in ascending order based on the 'Timestamp IST' column, which means the rows will be arranged from the earliest date/time to the latest date/time.
   ![image](https://github.com/ozibook/Posting_Time_Analysis/assets/144370840/87772cce-39dc-475d-a186-b028807f3f6a)
</details>

6. 



## Installation Guide👨‍💻
The following libraries are required to run the code<br>
1. Import re <br>
```
import re
```
2. Install datetime <br>
```
!pip install datetime
```
3. Install Pandas <br>
```
!pip install pandas --quiet
```

# FAQs❓
 * Which environment to choose?
   - It is recommended to use Jupyter Notebook.

# Author & Contributions
* Atharva Kaushik
* Jai Goyal
