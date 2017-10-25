**Healthcare Analytics: Focus on clinic efficiency**       
    *HIPAA BREACHES* 


The motivation with this project is to increase clinic efficiency and focus into resources that will be most beneficial. 
Besides patient care, one of the lead things that effects clinic efficiency is the way data is controlled. When HIPAA is breached then clinical efficiency goes down. **Can we predict if there will be a data breach?** Are there characteristics that are likely to lead to a breach in data? Which is the **most insecure** way to have information stored?

I acquired data from data.world:
    [HIPAA Breaches](https://data.world/health/health-data-breaches)
     
     
   
This data is tabulated and I used both R and Python to extract insight. The first thing I did after the initial data cleaning in R was begin the EDA by mapping out the amount of breaches by the year.
![hipaayear](https://user-images.githubusercontent.com/23061309/31903069-9bc27be8-b7ec-11e7-85e9-02b3683329c7.png)
This EDA was proven useful because you can visualize the current trend. The next thing that I did in R was an EDA of which establishments are the most likely to report a HIPAA data breach.
![hipaaEntityType](https://user-images.githubusercontent.com/23061309/31903419-a423e564-b7ed-11e7-9bac-c2f71ea75051.png)
As you can see, healthcare providers are the most vulnerable. I wanted to also do an EDA of the breach type or the way that the breach occured. This was also done in R.
![hipaaBreachType](https://user-images.githubusercontent.com/23061309/31903567-1a619dd4-b7ee-11e7-9de9-35bc90ec9ea3.png)
Now that I was able to get a quick glimpse, I switched to python on the jupyter platform to do some extended EDA. Below is the extended type of HIPAA breach in descending order. 
![extendedhipaaBreachType](https://user-images.githubusercontent.com/23061309/31904005-9796071c-b7ef-11e7-8ecc-f670cc3d3fbe.png)
I also wanted to see the location of all of the places that the HIPAA breaches occured.
![locationofhipaabreach](https://user-images.githubusercontent.com/23061309/31904160-0be786fe-b7f0-11e7-9fb2-db6e89eaebe7.png)
Surprisingly, the laptop and server locations weren't number one. In clinical environments there often is a hesitance about technology because of fear of it being not as secure as paper. This chart helps to clearly ascertain the true top vulnerable location.

![state](https://user-images.githubusercontent.com/23061309/31904409-ca94fe42-b7f0-11e7-97d4-8bcc95d79edd.png)
This was a quick EDA I did for location and in the future I would like to clean it up by controlling for the population.

Below is the quantile of amount of people effected by the HIPAA breaches.
![quantile](https://user-images.githubusercontent.com/23061309/31904522-22fdae08-b7f1-11e7-9cab-8a5253ee353b.JPG)


**Summary** 

-CA is most affected (would like to further expand by controlling for population)


-Paper/Films are the most vulnerable culprit to HIPAA breaches


-The average amount of people effected is around 2300. 

**Further Analysis**


Included in this repo is a separate CSV containing just the web description of the HIPAA breaches. I am currently working on performing sentiment analysis on this description in order to gather some insight. I would also like to find the average amount of people effected for each breach type.

**HIPAA BREACH WORD CLOUD**
[cloud](https://user-images.githubusercontent.com/23061309/32005986-389a85bc-b96b-11e7-87a4-8063bb674e9c.JPG)
