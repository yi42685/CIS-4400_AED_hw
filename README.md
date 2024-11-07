# CIS-4400_HOMEWORK
New York City Automated External Defibrillator (AED) Inventory

## Business requirement:
the goal is to determine whether there was enough of AEDs provided at coordinate location based on the population density of each area.

## Functional requirement:
1.	Classify each council district and zip
2.	Identify the number of AEDs provided of each council district and zip
3.	Identify the population density of each council district and zip
4.	Integrate the population density of the public area and assess the ratio of AEDs to population density

## Data requirement:

## Information Architecture:
**Information Architecture Diagram** 


<img width="732" alt="Screen Shot 2024-11-07 at 3 17 12 AM" src="https://github.com/user-attachments/assets/be707015-1c44-425f-8226-8edaa98c1b92">

**Information Architecture Description** 
I am doing OLAP to analyze if there are enough of Automated External Defibrillator (AED) provided for each area in NYC. Government department employee, supplier and stakeholder will have the access of the data. The data is important to make BI solutions about NYC residents’ public health.

My first stage is to gather data from New York City Automated External Defibrillator (AED) Inventory, then clean, reformat, transform, and load them to data warehouse. The second stage will be data franchising, which I will filter and subset the data, restructure, aggregate and store them into three different data marts. When I finished this process, the data is ready to be use for OLAP to do business analysis/reports/data visualization etc.




## Data Architecture:

**Data Architecture Diagram** 

<img width="665" alt="Screen Shot 2024-11-07 at 6 02 28 PM" src="https://github.com/user-attachments/assets/99550e14-29d4-4e3d-a518-ef28e90cea6c">


**Data Architecture Description** 

The raw data is collected by department of health and mental hygiene (DOHMH) for NYC REMSCO. The raw data is already integrated by DOHMH, which includes the address, locations, and populations etc. However, data can’t directly be used. It still needs to be ETL and reformat the data that is needed. After that, data will be store in three different data marts (number of AED, council district and zip, population data) by using Bottom-Up method. Finally, data from three different data marts will goes to data warehouse and ready to be use for data mining or analysis.












