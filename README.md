# Posting Time Analysis

### Task Description
The goal of this task is to conduct a comprehensive analysis of the posting times of our competitors' LinkedIn content. By examining the correlation between post timestamps and key engagement metrics such as likes, comments, and engagement rate, this analysis aims to provide valuable insights into the optimal timing for sharing LinkedIn posts. The primary objective is to determine when our company's LinkedIn posts are most likely to resonate with the audience and achieve higher levels of engagement. This research will enable us to make informed decisions about the timing of our LinkedIn content sharing, ultimately enhancing our outreach and impact within the LinkedIn community.

### Task Objective🎯
The Objective of this task is to determine the optimal time slots for posting on LinkedIn based on data-driven analysis and experiments for Ozigen.


### 📁File Details
#### 1. Excel File Format:
File Type: Ensure the file you want to process is in .xlsx format.

Columns:

URL: This column should contain URLs with embedded 19-digit post IDs. The code in this notebook will extract these post IDs to derive timestamps.

Sample Excel File Structure:

URL
https://example.com/post/1234567890123456789

#### 2. Using the Code in This Notebook:
Navigate to the cell containing the line:

input_file = "trial.xlsx"

Modify this line to point to the path of your Excel file. For example:

input_file = "path_to_your_file.xlsx"
- [Go to File↗️] https://drive.google.com/file/u/0/d/1C8d5gYXj38MtC7MrWZBh_WZrp07EfvSZ/edit
#### 3. Running the Code:
Execute the cell containing the code by selecting it and pressing Shift + Enter.

#### 4. Checking the Results:
After the cell execution completes, open the Excel file you provided.

You should now see the 'Timestamp UTC' and 'Timestamp IST' columns populated with the extracted timestamps in human-readable date formats for each URL in the 'URL' column.

#### 5. Notes:
* The code assumes that the URLs in the 'URL' column contain a 19-digit post ID from which a Unix timestamp can be extracted.

* The extracted Unix timestamp is then converted to human-readable date formats in both UTC and IST.

* The updated data is saved back to the original Excel file.
 
 


# Installation Guide👨‍💻
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
