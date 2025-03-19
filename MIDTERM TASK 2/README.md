# 𝐌𝐢𝐝𝐭𝐞𝐫𝐦 𝐋𝐚𝐛 𝐓𝐚𝐬𝐤 𝟐: 𝐃𝐚𝐭𝐚 𝐂𝐥𝐞𝐚𝐧𝐢𝐧𝐠 𝐚𝐧𝐝 𝐓𝐫𝐚𝐧𝐬𝐟𝐨𝐫𝐦𝐚𝐭𝐢𝐨𝐧 𝐔𝐬𝐢𝐧𝐠 𝐏𝐨𝐰𝐞𝐫 𝐐𝐮𝐞𝐫𝐲 𝐄𝐝𝐢𝐭𝐨𝐫
To extract useful information from the file UncleanedDSJObs.csv taken from a Job Posting site available in Kaggle.  
## 𝐎𝐛𝐣𝐞𝐜𝐭𝐢𝐯𝐞𝐬: 
- to find out Which Job Roles pay the highest and least
- to find out What size companies pay the best
- to find out Where Job Roles or Job Titles pay the best and least in a specific state
## 𝐃𝐚𝐭𝐚 𝐒𝐞𝐭 𝐁𝐞𝐟𝐨𝐫𝐞 𝐂𝐥𝐞𝐚𝐧𝐢𝐧𝐠 𝐚𝐧𝐝 𝐓𝐫𝐚𝐧𝐬𝐟𝐨𝐫𝐦𝐚𝐭𝐢𝐨𝐧:

![image](https://github.com/user-attachments/assets/d35fed9c-0c58-4722-989f-b0dbb19798da)



## 𝐒𝐭𝐞𝐩𝐬 𝐏𝐞𝐫𝐟𝐨𝐫𝐦𝐞𝐝 𝐢𝐧 𝐃𝐚𝐭𝐚 𝐂𝐥𝐞𝐚𝐧𝐢𝐧𝐠 𝐚𝐧𝐝 𝐓𝐫𝐚𝐧𝐬𝐟𝐨𝐫𝐦𝐚𝐭𝐢𝐨𝐧:
- Duplicated the raw data to preserve the original.  
- Cleaned the salary estimate column by removing everything after the "(" symbol.  
- Created Min Sal and Max Sal columns from the salary estimate.  
- Added a new column Role Type to classify jobs as "data scientist", "data analyst", "data engineer", "machine learning engineer", or "other" based on the job title.  
- Corrected the location column with custom states and split it into city and state abbreviation.  
- Replaced incorrect state entries (e.g., "anne rundell" to "ma").  
- Split the company size column to extract MinCompanySize and MaxCompanySize, and removed the word "employees".  
- Replaced invalid or negative values:  
- Competitors: replaced -1 with "n/a".  
- Revenue: replaced negatives with 0.  
- Industry: replaced -1 with "other".  
- Cleaned company name by removing extra ratings or numbers at the end.  
- Removed unnecessary columns like job descriptions.  
- Duplicated the cleaned data as Sal By Role Type dup, selected Role Type, Min Sal, and Max Sal, converted salaries to currency, multiplied by 1000, and grouped by - Role Type to get average salaries.  
- Created a reference as Sal By Role Size ref, selected Size, Min Sal, and Max Sal, multiplied salaries by 1000, and grouped by Size to get average salaries.  
- Imported a State Mapping file to map state abbreviations to full state names and merged it with the dataset.  
- Created a reference as Sal By State ref, selected State Full Name, Min Sal, and Max Sal, multiplied salaries by 1000, and grouped by State Full Name to get average salaries.  
- Checked query dependencies to confirm correct relationships.  

## 𝐅𝐢𝐧𝐚𝐥 𝐎𝐮𝐭𝐩𝐮𝐭
### 𝐂𝐥𝐞𝐚𝐧𝐞𝐝 𝐃𝐚𝐭𝐚
![image](https://github.com/user-attachments/assets/5bd26fdf-2453-4516-9c58-227acb6bfad3)

### 𝐒𝐚𝐥 𝐁𝐲 𝐑𝐨𝐥𝐞 𝐓𝐲𝐩𝐞 𝐝𝐮𝐩
![image](https://github.com/user-attachments/assets/6f63d3bb-ff22-4bba-ad81-a63479b108a3)


### 𝐒𝐚𝐥 𝐁𝐲 𝐑𝐨𝐥𝐞 𝐒𝐢𝐳𝐞 𝐫𝐞𝐟
![image](https://github.com/user-attachments/assets/94b376e0-ee80-4a51-81d9-189ab2d592be)

### 𝐒𝐚𝐥 𝐁𝐲 𝐒𝐭𝐚𝐭𝐞 𝐫𝐞𝐟
![image](https://github.com/user-attachments/assets/0ba06df9-28c3-4fe6-8a51-b75f6c3931e5)


### 𝐐𝐮𝐞𝐫𝐲 𝐃𝐞𝐩𝐞𝐧𝐝𝐞𝐧𝐜𝐢𝐞𝐬
![image](https://github.com/user-attachments/assets/d3b6545e-895f-4866-bb47-0fd988194832)



 
