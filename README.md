A Strategic Approach to Restaurant Expansion

This project is a strategic analysis to guide the next steps in restaurant expansion. An overview of the restaurant data, covering key aspects such as geographical distribution, competition analysis, cuisine preferences, pricing dynamics, and more.

Some key aspects of the Excel data we have are:                                                                                                                                                                      
Restaurant ID | Restaurant Name | Country code | City | Address | Cuisines | Currency | Has Table booking | Has Online delivery | Is delivering now | Price range | Votes | Average cost for two | Ratings | Date Opened

Here we have the data of the restaurants opened between the years 2010 and 2018 and a total of 15 different countries.                                                                                               

Total number of opened restaurants present in the data: 9551                                                                                                                                                         

These restaurants are from 15 different countries.                                                                                                                                                                

The data provides us with the following:                                                                                                                                                                             
-- Names and IDs of individual restaurants.                                                                                                                                                                          
-- Country codes and cities in which they were located.                                                                                                                                                              
-- Detailed addresses of the restaurants.                                                                                                                                                                            
-- The type of cuisines they offer.                                                                                                                                                                                  
-- Details about whether they have table booking and online delivery.                                                                                                                                                
-- Price range from 1 to 4.                                                                                                                                                                                          
-- Number of votes provided by the customers.                                                                                                                                                                        
-- The average cost for two.                                                                                                                                                                                         
-- Ratings by the customers from 1 to 5.                                                                                                                                                                             
-- The date on which the particular restaurant was opened.                                                                                                                                                           

Analytical Approach and Tools:                                                                                                                                                                                       
Data cleaning:                                                                                                                                                                                                       
-- Identified rows with empty cells in the Cuisines column.                                                                                                                                                          
-- Applied a filter to the Cuisines column.                                                                                                                                                                          
-- Selected the blank cells within the filtered Cuisines column.                                                                                                                                                     
-- Removed the rows corresponding to the selected blank cells for better data integrity.                                                                                                                             

Data Enrichment:                                                                                                                                                                                                     
-- Noted the absence of country names in the dataset but found the presence of country codes in the Raw Data sheet.                                                                                                  
-- Located a country description sheet containing both country names and country codes.                                                                                                                              
-- Inserted a new column next to the country code column in the Raw Data sheet and named it "CountryName."                                                                                                           
-- Utilized the VLOOKUP function to populate the CountryName column using data from the country description sheet.                                                                                                   
-- Identified the need to separate the date of restaurant openings into year, month, and day.                                                                                                                        
-- Applied the Text-to-Columns feature to the column containing the opening dates.                                                                                                                                   
-- Split the date into three separate columns: year, month, and day.                                                                                                                                                 
-- Analyzed the newly created "year" column to determine the number of restaurants opened each year.                                                                                                                 

-- Identified the need to standardize the "Average cost for two" column to a single currency (INR).                                                                                                                                                               
-- Created a new column in the country description sheet named "Currency Exchange Rate INR."                                                                                                                                                               
-- Gathered current exchange rates for all relevant currencies from Google and updated the new column.                                                                                                                                                               
-- In the Raw Data sheet, used the IF formula to check the original currency of each entry.                                                                                                                          
-- If the currency was not Indian, multiplied the cost by the corresponding exchange rate to convert all values to INR.                                                                                              

Descriptive Analysis:                                                                                                                                                                                                
-- Created two pivot tables to summarize the number of restaurants opened in each country and in each year.                                                                                                          
-- Inserted pivot tables to display:                                                                                                                                                                          
------ Average of Ratings                                                                                                                                                                                            
------ Maximum of Ratings                                                                                                                                                                                            
------ Average of Votes                                                                                                                                                                                              
------ Average of "Average cost for two" in INR                                                                                                                                                                      
------ Type of Cuisine, for filtering by price range, table booking, and online booking options                                                                                                                      
-- Used the COUNTIFS function to calculate the number of restaurants in India within the price range of 4.                                                                                                           
-- Calculated the correlation between the rate and ratings using the CORREL function.                                                                                                                                

Visualizations:                                                                                                                                                                                                      
Created a dashboard:                                                                                                                                                                                                 
-- Inserted a table to display the count of restaurants in each country.                                                                                                                                             
-- Added two cards to show:                                                                                                                                                                                          
------ The count of restaurants in India within the price range of 4                                                                                                                                                 
------ The correlation between the rate and ratings                                                                                                                                                                  
-- Placed two pie charts to depict the number of restaurants with:                                                                                                                                                   
------ Yes and No segments for online bookings                                                                                                                                                                       
------ Yes and No segments for table bookings                                                                                                                                                                        
-- Inserted two bar charts to demonstrate the distribution of:                                                                                                                                                       
------ The count of restaurants based on the average of votes                                                                                                                                                        
------ The average cost for two                                                                                                                                                                                      
-- Placed a clustered column chart to display:                                                                                                                                                                       
------ The average ratings                                                                                                                                                                                           
------ The count of restaurants according to ratings                                                                                                                                                                 
