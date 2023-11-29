# West Nile Virus Prediction
**Description :**  Predict West Nile virus in mosquitoes across the city of Chicago

**Data Dictionary**

| Feature          | Dataset(CSV)         |   Description                            |                               
|:----------------:|:----------:|:-------------------------------------:|
| **id**   | train,test|  the id of the record | 
| **Date** | train,test   | date that the WNV test is performed | 
| **Address** | train,test   | approximate address of the location of trap| 
| **Species** | train,test   | the species of mosquitos | 
| **Block** | train,test   |  block number of address | 
| **Street** | train,test   | street name | 
| **Trap** | train,test   | Id of the trap| 
| **AddressNumberAndStreet** | train,test   | approximate address returned from GeoCoder | 
| **Latitude** | train,test   | Latitude returned from GeoCoder| 
| **Longitude** | train,test   | Longitude returned from GeoCoder | 
| **AddressAccuracy** | train,test   | accuracy returned from GeoCoder| 
| **NumMosquitos** | train  | number of mosquitoes caught in this trap | 
| **WnvPresent** | train  | whether West Nile Virus was present in these mosquitos. 1 means WNV is present, and 0 means not present.  | 
| **Tavg** | weather | Average temperature | 
| **DewPoint** | weather | Average dewpoint | 
| **WetBulB** | weather | Average Wetbulb | 
| **Sealevel** | weather | Average Sealevel pressure | 
| **ResultSpeed** | weather | Resultant wind speed | 
| **ResultDir** | weather | Resultant wind direction | 
| **AvgSpeed** | weather | Average wind speed | 
| **StnPressure** | weather | Average pressure at station | 
| **PrecipTotal** | weather | Water Equivalent (inches & hundredths) | 














## Problem Statement
The West Nile virus is primarily transmitted to humans through infected mosquitoes, with around 20% of infected individuals exhibiting symptoms ranging from persistent fever to severe neurological illnesses, potentially leading to death. The virus was first reported in humans in Chicago in 2002. In response, the City of Chicago and the Chicago Department of Public Health (CDPH) established an ongoing surveillance and control program in 2004.

As part of this program, mosquitoes in  traps throughout the city are regularly tested for the West Nile virus from late spring to fall. (May-Oct) The results of these tests play a crucial role in determining when and where the city will conduct airborne pesticide spraying to control adult mosquito populations.

There is a competition hosted by CDPH seeks predictive models based on weather, location, testing, and spraying data to forecast when and where various mosquito species are likely to test positive for the West Nile virus. Improving the accuracy of these predictions can aid the City of Chicago and CPHD in allocating resources more efficiently to prevent the transmission of this potentially fatal virus. The initiative aims to enhance public health efforts and contribute to a more proactive approach in addressing West Nile virus outbreaks. Our team decided to take part in this challenge.


## Conclusions

Utilizing `XGBoost with SMOTE` to Enhance Classification Performance

After conducting thorough evaluation and experimentation, the decision has been reached to employ the `XGBoost algorithm in conjunction with the Synthetic Minority Over-sampling Technique (SMOTE)` to address class imbalance. This strategic choice is grounded in the compelling performance metrics observed during the model evaluation process.

- High `Test Score (Kaggle)` and `ROC-AUC Score`
      The application of XGBoost with SMOTE yields a notable Kaggle Score of `0.73` and an ROC-AUC Score of `0.82`. These elevated scores not only signify effective performance on the provided dataset but also indicate a robust potential for generalization to previously unseen data.

- Improved `Recall` for Class 1 (Present WNV)
    The recall for Class 1, achieved through the use of XGBoost and SMOTE, stands at `0.167`. This showcases a substantial improvement when compared to the recall of 0 observed without the implementation of SMOTE. This enhancement holds particular significance in scenarios where accurately identifying instances of Class 1 is of paramount importance.


## Recommendations for West Nile Virus Prevention and Control

In light of the understanding that a higher mosquito population correlates with an increased likelihood of West Nile Virus (WNV) presence, it is imperative to implement strategic measures to mitigate the risk. The key actions proposed for effective prevention and control are as follows:

**1. Mosquito Population Control:**
   - **Geographical Focus:**
      - Prioritize both northern and southern regions of Chicago.

   - **Identified Locations for Wide Coverage Spraying:**
      - Chicago O’Hare International Airport
      - South Doty Ave.
      - North Oak Park Ave.
      - South Stony Ave.
      - Milwaukee Ave.

   
   - **Elimination of Breeding Sites:**
      - Undertake comprehensive efforts to eliminate potential mosquito breeding sites in the specified locations.

**2. Vulnerable Target Residences:**
   - **Identified High-Risk Areas:**
      - Hospitals
      - Elderly care centers

**Key Action:** Implement extra surveillance and monitoring measures in these vulnerable areas.

**Seasonal Surveillance and Monitoring:**
   - **Time Frame:**
      - Conduct heightened surveillance and monitoring activities from June to September each year.

   - **Temperature Consideration:**
      - Acknowledge the influence of warmer temperatures on mosquito activity and reproduction; adjust surveillance efforts accordingly.

   - **Historical Infected Locations:**
      - Prioritize monitoring of areas with a history of WNV outbreaks; investigate for the presence of favorable mosquito breeding sites.

By formalizing and adhering to these recommendations, we aim to enhance the proactive measures in preventing and controlling the spread of West Nile Virus, particularly in identified high-risk locations and during the critical months of heightened mosquito activity.
