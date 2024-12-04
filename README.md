# Nurse_Staffing_Data


## Nursing Staffing Data – Overview

To provide insights into the staffing needs of long-term care facilities, we began with an initial review of the PBJ Daily Nurse Staffing Data from the Centers for Medicare & Medicaid Services for the first quarter of 2024 (Payroll Based Journal Daily Nurse Staffing | CMS Data). For future in-depth location analysis, we merged the County and State columns to ensure accurate identification of counties, as some county names are repeated across different states.

This report analyzes the distribution and workload of healthcare providers across the United States, focusing on daily hours per resident, contractor hours, and staffing hours for each nursing position. Key findings include: 

1. State-Level Distribution:
  - The highest concentration of residents at healthcare providers, synonymous with the distribution of work hours, is on the East Coast, especially in cities like New York, Washington D.C., Miami, and Chicago. New York has the largest average resident numbers, about 50 residents more than other regions.
  -Outside of the East Coast, notable hotspots include Denver, Phoenix, Portland, Los Angeles, and San Francisco.

![image](https://github.com/user-attachments/assets/5bbcbf0d-32f2-46c2-ba7a-2813585e1ffb)

2. Daily Hours per Resident:
  - Daily hours per resident can indicate workload intensity at healthcare facilities. Overall, weekends see a lower workload, with the highest demand on Wednesdays at 4.6 hours per resident.
  - Remote locations, such as Alaska and Puerto Rico, have notably high daily hours per resident (7.05 and 6.86 hours, respectively), suggesting potential nursing shortages.

![image](https://github.com/user-attachments/assets/36e4b0db-2b5f-4650-95cf-91fba81c306e)

3. Contractor Hours:
  - There’s a higher reliance on contractor staffing in East Coast states like New York, New Jersey, and Pennsylvania, especially over the weekends, with average contractor hours exceeding 55 hours per day.
  - This suggests a trend toward filling weekend staffing gaps with contractors in these areas.

![image](https://github.com/user-attachments/assets/79e63c5d-915d-43a3-b643-7c5e811c9138)

4. Opportunities for Med Aide Technicians: 
  - Central states, including Nebraska, Oklahoma, and Kansas, have a significant demand for Med Aide Technician roles, averaging over 30 hours per day.

![image](https://github.com/user-attachments/assets/fefd12bc-56aa-476f-b741-0355df157b95)


### Contractor Staffing Hours Focus:

Let’s focus on providers with dependence on contractor staffing. Our analysis focuses on identifying providers with higher contractor usage or more complex staffing needs. The dataset includes 11,523 providers in total. To narrow the scope, we calculated the average contractor hours across all providers, which is 2,286 hours. By filtering out providers with total contractor hours below this average, we are left with 3,088 providers. This refined dataset allows us to focus on facilities that rely more heavily on contractor staffing. Additionally, we calculate data features to help us better understand the staffing requirements of different facilities.

1.	Total Contractor Hours - Sum of contractor hours at a provider.
2.	Total Employee Hours - Sum of fixed Employee hours at a provider.
3.	Percentage of Contractor Hours - Reliance on contractor hours in terms of total working hours.
4.	Contractor Hours-to-Resident Ratio - Reliance on contractor hours in terms of residents at the facility.
   
I obtain the median value of percentage contractor hours as 18.85% and a median value for contractor hours per resident as 0.7. These values help me create a baseline to measure to providers heavily reliant on contractor staffing solutions. Next, we utilize the Provider Information table (from the Provider Data Catalog) to classify certain providers. Key features such as the Case Mix Ratio (a higher ratio indicates more demanding roles), overall ratings, ownership and institution type and inspections offer valuable insights into the healthcare providers quality, and staffing conditions.

![image](https://github.com/user-attachments/assets/cef4d674-aa03-4ce1-8263-af591d624ee2)

### Healthcare Companies Analysis

This analysis targets providers with significant reliance on contractor staffing. With 11,523 providers in total, the average contractor hours across all providers are 2,286. By filtering out providers with contractor hours below this average, we narrow the focus to 3,088 providers who depend more heavily on contractor staffing.

To deepen our understanding of staffing needs, the following features are calculated:

1.	Total Contractor Hours – Sum of contractor hours at a provider.
2.	Total Employee Hours – Sum of fixed employee hours at a provider.
3.	Percentage of Contractor Hours – Reliance on contractor hours relative to total working hours.
4.	Contractor Hours-to-Resident Ratio – Contractor hours in relation to the number of residents at the facility.
   
The median percentage of contractor hours is found to be 18.85%, and the median contractor hours per resident is 0.7. These values provide a baseline for measuring the degree of reliance on contractor staffing at individual providers.

![image](https://github.com/user-attachments/assets/f64a8113-5d9e-4512-aad7-e8725d2730ad)
 
#### Jonathan Bleier & Yaakov Sod:

•	Average Contractor Hours: Over 18000 hours in Q1 2024, across 15 providers.
•	Percentage Contractor Hours: 37%, which is highest in the group.
Jonathan Bleier Management shows a significant reliance on contractor staffing, with notably high contractor hours across its facilities. However, these facilities have a relatively low overall rating of 2, indicating potential challenges in management or operations. This suggests an underlying issue that could be addressed through a more efficient and reliable staffing solution, which could improve operational efficiency and care quality.


#### Cassena Care:

•	Average Contractor Hours: 18,000 hours per provider, with a significant reliance on contractor staffing, accounting for 24% of total staffing.
•	Overall Rating: 3.14, reflecting effective management and a strong commitment to patient care.
Cassena Care’s ability to efficiently manage a larger resident base—nearly 80 more residents per facility compared to others—coupled with a relatively high reliance on contractors and favourable ratings of 3.14, provides valuable insights into effective management practices. This is particularly relevant in one of the highest-operating regions (New York and Connecticut) in terms of healthcare staffing hours. Their approach could serve as a model for other healthcare providers in similar regions, offering best practices for balancing staffing needs while maintaining quality care.

### Healthcare Provider Analysis

![image](https://github.com/user-attachments/assets/0c97a946-dcf5-4da3-9a4b-3cf92e3c0064)

For this analysis, I look at care providers with the highest contractor hours and contractor hours to resident ratio. As mentioned earlier this allows us to focus on providers with the highest measures of dependency on contractor hours.



#### Coral Reef Subacute Care Center (Miami Dade, Florida)

•	Contractor Hours: Over 55,000 in Q1 2024, with 100% reliance on contractor staffing.
•	Contractor Hours-to-Resident Ratio: 3.66, significantly higher than the median of 0.7.

#### Michigan Veteran Homes (Michigan)

•	Contractor Hours: Over 60,000 contractor hours in Q1 2024.
•	Contractor Hours-to-Resident Ratio: 5.59, the highest ratio in the dataset.

![image](https://github.com/user-attachments/assets/4c732389-916b-479c-972d-adff69030073)

## Conclusion

Since the COVID-19 pandemic, the demand for safe and reliable nursing care has surged. In response to this increased demand, many nurses who feel overworked and stressed have left their positions for more lucrative opportunities. This study aims to review the PBJ nursing staffing data to assess its potential for predicting workflow demands and developing more effective staffing solutions for healthcare providers to combat the nursing shortage.

The report suggests that by conducting a deeper analysis beyond Q1 and examining data across different providers, we can develop customized staffing plans tailored to each facility. This would focus on identifying specific days and months with significant surges in staffing hours, addressing the ongoing nurse staffing challenges. By narrowing down regions and providers, stakeholders can gain a clearer understanding of workforce characteristics, potential staffing gaps, and regional variations in nursing demand. The insights generated from this analysis will be valuable for resource allocation, recruitment strategies, and targeted workforce planning, as well as providing an overview of nursing role demands geographically.

For nurses, this analysis provides an overview of each facility, highlighting peak staffing days and work complexity. By developing a targeted contractor workforce strategy, we can offer nurses the opportunity to work with multiple organizations, helping them find roles that align with their skills and preferences. This approach not only addresses staffing challenges but also enhances flexibility for nurses, allowing them to pursue roles that best suit their professional goals and personal needs.

