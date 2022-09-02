# **BCHPCA-Financial-Analysis-Outlook**

## **About Stakeholder**

The BC Hospice Palliative Care Association (BCHPCA) is a not-for-profit, membership organization, which has been representing individuals and organizations committed to promoting and delivering hospice palliative care in British Columbia, Canada for over 34 years to people in need across the province of BC and the Yukon who are dying, their loved ones who are grieving and caregivers.

## **Business problem**

Over the past 10 years, the popsicles have grown in service delivery and size, but the one challenge **BCHPCA hears** time and time again from the hospices is that their funding from the health authority is not reflecting the change in growth and cost of living. With that said, ***BCHPCA wants to look at the past 4–5-year trend regarding funding, service delivery and hospice growth and the correlation with government funding, in comparison to donor and grant funding (which hospices source themselves) to better understand how government funding has supported this growth, if any***.
The finished product will be used for advocacy for regular funding planning in the provincial government.

## **Analytical problems**

1.	Analysis of shares and trends in hospices’ revenue sources.
2.	Analysis of trend in services growth.
3.	Analysis of correlation between the government funding and services growth.
4.	Analysis of correlation between services cost and the main cost influencer. Assess the possibility of cost prediction for the next years.

## **Methodology**

1.	Build a database sourced from Canada Revenue Agency, BC Stats and Statistics Canada.
2.	Verify and clean the data, engineer new variables.
3.	Analyze BCHPCA revenue growth.
4.	Analyze revenue trends per health region and hospice type. 
5.	Analyze services expenditures trend.
6.	Cross-reference with BC Stats (65+ elderly population, price indexes of goods and health care services).
7.	Analysis of correlation between services growth, 65+ elderly population growth, and the government funding in linear regression.
8.	Generate insights for actions.

Analytical tools: Excel, Python libraries, Statsmodels, Sklearn Linear regression.

## **Data Understanding**

*Years*:  2017, 2018, 2019, 2020 years have complete data and are well represented by total BC hospices. 

*Number of hospices*: 70 hospices. 

*Health regions in BC*: 5 regional health territory where the hospices are registered and operating.

*Hospice Type*: C-community based, R- residential (hospital based).

![image](https://user-images.githubusercontent.com/95148782/188041598-38b0199d-d931-45f4-995d-3cceb4bf936c.png)

![image](https://user-images.githubusercontent.com/95148782/188041404-d595fd42-71a7-4635-8e25-4507aea94c3d.png)

***65+Population***: the domain expert advised that the major influencing factor of services growth is growing aging population.

***Charitable expenditure***:  a variable that reflects the volume of services provided by hospices (based on description in Canada Revenue Agency).

## **Key Insights**

1.	Total BC Hospice Revenue avg growth is 5.8% in 4 years driven by growth from Other Revenue sources which are fundraising + gifts from other charities.
![image](https://user-images.githubusercontent.com/95148782/188040058-07da6f9e-ecea-4bab-814f-e4ae9947faf8.png)

2.	Within Other Revenue, growth drivers are namely, Island Health, Vancouver, and Fraser Health. Island and Northern Health are very dependent on donations as this is the largest portion of their income in the first place, and thus may be forced to depend on Government Funding or Other Revenue to maintain their regular operations.
![image](https://user-images.githubusercontent.com/95148782/188040352-83d5d5d3-2c69-41da-9e87-0a6faf2feec4.png)

3.	Community hospices in general have very little funding with a 19% share of government funding last year 2020 alone, but they have broader coverage of 65+ population, accounting for 64% of BC's total older population, while Residential type, which has the largest share of government funding at 81%, serves only 36% of the 65+ population.
![image](https://user-images.githubusercontent.com/95148782/188040458-0c7025ff-81c7-469d-96cb-b56ab2faf9ef.png)

![image](https://user-images.githubusercontent.com/95148782/188040501-8ac47d30-e2b5-4b5b-b695-c2bd1548b28f.png)

4.	 Charitable Expenses (volume of services) is the major chunk of the total expenses. It is also a growing expense type across BC hospices increasing from 49% of total expenses in 2017 to 63% in 2020. 
![image](https://user-images.githubusercontent.com/95148782/188040609-4928dfd6-1c0b-4ee8-ac66-3e28f970dcef.png)

5.	Charitable Expenses (volume of services) grew by 16% avg yearly. Since the growth of Government funding, averaging 2.9% per year, is not as fast as the growth of Charitable expenses, this means that growth in services is sustained by other sources of revenue. 
![image](https://user-images.githubusercontent.com/95148782/188040753-bd510a07-2344-4779-8e88-4c2a05870f94.png)

6.	Charitable expenses, as mentioned above, is closely related to hospice services, not to mention its sheer size, so it's a good variable to predict future budget needs.
7.	Government Funding is growing at an average of 2.9% per year, which is not as high as elderly population, which is growing at an average of 6.8% per year. It may impact sooner or later operational expenses, and thus should be considered in the budget planning.
Although the average growth in Government funding appears to outpace the average growth in the health and service price indexes per year, the latter are on an ongoing positive trend, while Government funding has the growth in 2019 and the sharp fall in 2020.
![image](https://user-images.githubusercontent.com/95148782/188040856-47915639-a990-40ef-9e4e-c71768d80ccd.png)

8.	Community hospices cannot rely on government funding as correlation analysis shows less support for Services expenses compared to residential ones. At the same time their expenses are linked to 65+population more strongly than in residential hospices.
9.	Evaluation metrics of linear regression confirm that relationships between Services expenses and 65+population dynamics are statistically significant, but this indicator alone is not enough to explain and help predict future expenses.

## *Conclusions and Recommendations*

1. Government funding is growing at 2.9% average in 4-year period with increase in 2019 and drop in 2020. Compared to other growth rates Services Expenses (16%), and 65+population (6.8%) over the same period it is obvious that government funding is lagging behind. Consequently, hospices have to double revenues coming from other sources to compensate and to ensure each hospice addresses the growing demand of its services. Thus, currently it would be recommended planning yearly funding increase linked to Health Care Price Index increase and senior population increase. 
2. The current financial model is not sustainable because increasing demand for services (services expenses) is mainly supported by increasing income from fundraising events and gifts from other charities. This is the only source of income with a stable growth trend, due to which the share of government funding and donations declined in 2019-2020. At the same time, the source is unstable and depends on external circumstances such as COVID. Indeed, the share of fundraising revenue was 65% in other revenue source until 2019 and dropped to 57% in 2020. Thus, it would be recommended to deploy social media platforms and explore ways to conduct fundraising events there. 
 3. Ageing population growth fuels the services expenses increase; however, this growth alone cannot explain the difference in the amount spent by different hospices. There should be additional influencing indicators such as types of services provided and terminal illness statistics in different health regions or even at the community level. Thus, if there will be need in forecasting services expenses for the next years it is recommended conducting surveys to find out these indicators. Hospices organizations can report the services they provide in numbers (for each service hours, staff, supplies), and experts from a medical field can provide the statistics for predominant terminal illness in health regions and communities. 
4. After exploring the financial data, it was assumed that hospice organizations have relationships with each other and, for example, share fundraising and donations revenue. If it is true situation, it would be recommended exploring the hospices network to identify the relationships and gifts directions. Revealed financial relationships may be useful for budget and funding planning. It may be possible, as well, to determine hospice organizations that are center for smaller ones and can take a role in finance management. 











