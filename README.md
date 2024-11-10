# CALL CENTER DASHBOARD

### Dashboard Link : https://1drv.ms/u/c/a7974a392170cc2e/EeeYGsq2iLlLg18loBd1cIEBLjnyXkpDUazvu0fKwgg4Tg?e=B4yZzL

## Problem Statement

This dashboard helps Phonenow telecom company to identify an accurate overview of long term trends in customer agent behaviour.We can identify On which topic more call is coming,customer is satisfied or not,On which area we need to improve

Since,

Total number of calls received is 5000,In that 72.92 % issue is resolved.More call coming is related to Streaming and the average rating given by customer is 3.40


### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a csv file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4 : It was observed that if customer call is not attended, average talk duration,satisfication rating,speed of answer in seconds leaves blank
- Step 5 : For calculating average talk duration,average customer rating,speed of answer in seconds null values were not taken into account.
- Step 6 : In the report view, under the view tab, theme was selected.
- Step 7 : Visual filters (Slicers) were added for two fields named "Agent", "Topic".
- Step 8 : Six card visuals were added to the canvas to represent
Total calls received,No of agents,Total calls answered,Total calls Unanswered,Average speed of answer,Average customer rating given by customer.

           Although, by default, while calculating average, blank values are ignored.

All these values have been ignored while calculating average rating for each of the parameters mentioned above.

        
- Step 9 : New measure was created to find total count of customers.

Following DAX expression was written for the same,
        
        Total No of calls = COUNT(call id)
        
A card visual was used to represent count of calls received

![image](https://github.com/user-attachments/assets/1e507107-5e18-4a2a-a9f9-b5a352416719)


        
 - Step 16 : New card visual was created to find total number of agents
 
 Following DAX expression was written to find Total number of Agents
 
         Total Agents = Count(Sheet1[Agent])
 
 
 # Snapshot of Dashboard
 
 
![image](https://github.com/user-attachments/assets/f783ac5d-a81c-44f9-ab29-e4568dee3236)



# Insights

A single page report was created on Power BI Desktop.

Following inferences can be drawn from the dashboard;

### [1] Total Number of Calls received

   Total number of calls received = 5000

   Number of calls attended = 4054
   Number of calls not attended = 946
           
### [2] Average Measures

    a) Average speed of answer in seconds - 67.52
    b) Average customer rating - 3.40
    c) Average talk duration - 30.21 
  

 ### [3] Some other insights
 
 ### Topic
 
 1.1) Most of the calls received on the topic Streaming
 
 1.2) 72.92% Calls are resolved 
 
 1.3) 81% calls attended 

 1.4) Average speed of answer in seconds 67.52 seconds

