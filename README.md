
# Group 2 MIST 4610 Project 2

## Team name
39217 Group 2

## Team members

1. Jenny Chen [@jennyc5](https://github.com/jennyc5)

2. Mathews Fluker [@mathewsfluker](https://github.com/mathewsfluker)

3. Justin Goldman [@justingoldman25](https://github.com/justingoldman25)

4. Connor Hawkins [@conehawk](https://github.com/conehawk)

5. Nixxon Idaewor [@NnixxonUGA](https://github.com/NnixxonUGA)

6. Aude-ellen Nangle [@audeellen](https://github.com/audeellen)

## Description of dataset:

The dataset we studied for this project details traffic violations/stops in Montgomery County (MC). MC is the most populous county in Maryland, so its traffic volume is ideal for data analysis. We sourced this dataset from the provided government source (https://catalog.data.gov/dataset/traffic-violations).
 
Traffic stops are the entity in this database. Each unique instance (row) is identified by the primary key, called “SeqID”, which is comprised of letters, numbers, and dashes. Many attributes describe each traffic stop. First, there is date/time information about when the traffic stop occurred. Next, geographic data includes street, state (some stops occur across county borders in DC/VA), latitude, longitude, and the police agency (stop location influences which agency handles the stop). There are also “yes/no” details about the characteristics of the violation. These include (but are not limited to) seat belt usage, personal injury, fatality, alcohol involvement, etc. The dataset further describes a search that may take place during a traffic stop. It explains if there was a search, the search’s disposition, the outcome, and the reasons for conducting one. The search information is all VARCHAR.
Additionally, there is info about the vehicle involved in the traffic stop. The dataset explains the vehicle type, year, make, model, color, etc. Finally, the dataset delves into the outcome of the traffic stop. It explains the type of violation, the charge (legal statute), and demographic information about the vehicle’s driver.

## Question 1:

Is there a relationship between major cities in Maryland and personal injury rate in accidents?

<img width="524" alt="Screenshot 2023-12-05 at 7 23 07 PM" src="https://github.com/audeellen/MIST4610/assets/148274722/d9c971dd-bde8-4c3b-a6d1-cf318bc806d4">










Importance:
This question is important to ask because the results can be used by EMS. By knowing where the geographic hotspots of injuries are, EMS know where to set up hospitals and where to have medical services stationed for the quickest possible response. Our initial hypothesis going in was that the hotspots would look extremely similar to a population chart, with cities with the most population having the most personal injuries in accidents. We thought that in particular, cities close to the DC/Marland border would have the most personal injuries. In order to measure for this, we first filtered by both the personal injury and accident column being “Yes”, as we only want results that are both an accident and result in a personal injury. We also limited the results to the state of Maryland. We took a count of personal injury and did a percentage of total quick table calculation in order to get a percentage of the total injuries from Maryland in each city.

Our results were interesting. On one hand, our initial hypothesis seemed to be mostly correct. We see three main hotspots on the border of DC and Maryland, consisting of around 40% of the total injuries. This would be an excellent place to focus medical attention. One thing that surprised us is we noticed a hotspot with 31.03% of personal injuries coming from a town called Germantown. This is extremely valuable information for EMS because it tells them that even though Germantown isn’t on the DC/Maryland border, it is a place that needs heavy medical attention. We wanted to get a better visualization of how many personal injuries in Germantown compared to the rest of the cities, so we created a pie chart. 
![1](https://github.com/justingoldman25/marylandtrafficviolations/assets/131189846/1689d6b5-b141-466b-89b1-2ffeab4527ad)


## Question 2:

What state within the DMV (DC, Maryland, Virginia) area has the most traffic violations? Within the states that has the most violations, where do citations and warnings occur the most within that state? 

<img width="391" alt="Screenshot 2023-12-05 at 6 59 26 PM" src="https://github.com/audeellen/MIST4610/assets/148274722/069bd776-3b45-40a2-be99-6084b5144f13">

<img width="627" alt="Screenshot 2023-12-05 at 7 20 17 PM" src="https://github.com/audeellen/MIST4610/assets/148274722/4ab130d0-01a1-4197-9f6d-e93c8363dfa8">

<img width="1214" alt="Screenshot 2023-12-05 at 7 21 59 PM" src="https://github.com/audeellen/MIST4610/assets/148274722/bb085ddf-e599-4ae5-8bb6-b13afa3e0d38">









Importance: 
This question is important because analyzing traffic violation data is crucial for improving road safety. Data-driven policies are essential for delivering effective laws and keeping people safe on the roads. These policies can be based on the insights gained from the analysis of traffic violation data, leading to more informed and strategic decision-making to address specific challenges and enhance overall road safety. Government officials can use this data to deploy additional law enforcement resources to high-violation areas, conduct targeted enforcement operations, and launch public awareness campaigns. Additionally, police stations in the surrounding areas with the most citations and warnings can collaborate on joint initiatives and share information to create a unified and coordinated approach in addressing traffic violations. By fostering communication and cooperation among police stations in areas with high citation rates, law enforcement agencies can develop comprehensive strategies. This may involve sharing best practices, coordinating enforcement efforts, and implementing consistent public awareness campaigns across neighboring jurisdictions. Such collaborative efforts can maximize the impact of interventions, create a more uniform approach to traffic safety, and contribute to a safer overall road environment.

<img width="1045" alt="Screenshot 2023-12-05 at 6 46 33 PM" src="https://github.com/audeellen/MIST4610/assets/148274722/df4c8e26-3a08-413c-af27-12d8394a56f2">


## The manipulations applied to the data set as part of the analysis:


Our data set did not need any manipulations for it to be utilized. However, since it had a vast number of records and columns it was harder to analyze. To deal with the vast amount of data, we added a variety of filters and marks to make the data easier to analyze and visually appealing. 


## Tableau packaged workbook
The packaged workbook containing the visualizations shown above is attached to this repository.

