# PCPS-Based-Energy-Sharing-Case-Setting

<div align="center">
  <img src = "Title.png"/>
</div> 

# Overview  
This project is a instruction for the ***parameters*** of the case studies in our paper  ***"A Practical Network-Free Energy Sharing Based on Private Charge Pile Sharing"***. 

> _**Toy Case**_: The parameters of the PCPS matching and PCPS-Based energy sharing problem on Toy case, involving 4 households.  
> _**ShenZhen Case**_: The parameters of the PCPS matching and PCPS-Based energy sharing problem on ShenZhen case, involving 1615 households.

<div align="center">{:width="300px"}
  <img src = "Schematic diagram of Cases.png"/>
</div> 
Fig.1. Schematic diagram of Cases. (Red dots are PCP, blue dots are EV in ShenZhen Case)

# Parameters Description
The parameters for each case are recorded in **six** Excel files, including ***PCPParameters.xlsx***, ***EVParameters.xlsx***, ***HouseholdParameters.xlsx***, ***HouseholdLoad.xlsx***, ***HouseholdPV.xlsx***, and ***TOU&FIT.xlsx***

## PCPParameters.xlsx
This file contains all parameters for each private charging piles (PCP), where:

>_**'PCP_Index'**_ : The index of each PCP;  
>_**'Household_index'**_ : The index for the household associated with PCP;  
>_**'T_ksta'**_ : The available start time of PCP;  
>_**'T_kend'**_ : The available end time of PCP;  
>_**'P_powermax'**_ : The maximum discharge/charging power of PCP;  
>_**'p_sermin'**_ : The PCP's minimum acceptable service fee per kWh;  
>_**'x and y'**_ : The location of PCP;  

## EVParameters.xlsx
This file contains all parameters for each electri vehicle (EV), where:
>_**'EV_Index'**_ : The index of each EV;  
>_**'Household_index'**_ : The index for the household associated with EV;  
>_**'t_arp'**_ : EV's arrival times at PCP;  
>_**'t_lep'**_ : EV's departure times at PCP;  
>_**'t_arh'**_ : EV's arrival times at home;  
>_**'t_leh'**_ : EV's departure times at home;  
>_**'EEVexp'**_ : EV’s desired charging capacity at matched PCP;  
>_**'p_serHmax'**_ : EV's maximum acceptable service fee per kWh;  
>_**'x and y'**_ : The location of EV;  
>_**'ItaEV'**_ : The charging and discharging efficiencies of EV;  
>_**'aEV, bEV and cEV'**_ : The discharging degradation coefficients of EV;  
>_**'EEVarh'**_ : The initial energy of EV when arrive at home;  
>_**'EEVlehmin'**_ : The minimum energy of EV when departuring home;  
>_**'EEVtra'**_ : The energy consumption of EV during _**'t_leh'**_ to _**'t_arp'**_;  
>_**'EEVup'**_ : EV’s maximum capacity;  
>_**'EEVlow'**_ : EV’s minimum capacity.  


## HouseholdParameters.xlsx
This file contains the parameters of TG and ES for each household, where:

>_**'Household_index'**_ : The index of each household;  
>_**'aTG, bTG, and cTG'**_ : The quadratic, linear, and constant cost coefficients of TG;  
>_**'PTGup'**_ : The maximum power limit of TG;  
>_**'PTGlow'**_ : The minimum power limit of TG;  
>_**'PTGraup'**_ : The maximum downward ramp rate of TG.;  
>_**'PTGralow'**_ : The maximum upward ramp rate of TG;  
>_**'aES, bES, cES'**_ : The charging and discharging degradation cost coefficients of ES;  
>_**'ItaES'**_ : The charging and discharging efficiencies of ES;  
>_**'PESup'**_ : The index for the household associated with PCP;  
>_**'EESup'**_ :  The maximum energy limit of ES;  
>_**'EESlow'**_ : The minimum energy limit of ES;  
>_**'EESinit'**_ : The initial energy of ES;

In particular, when the household does not contain associated resources,  corresponding parameters are empty.

## HouseholdLoad.xlsx

This file contains the Load demand data of households, where each column represents a household. 

## HouseholdPV.xlsx

This file contains the Photovoltaic power data of households, where each column represents a household. 

## TOU&FIT.xlsx

This file contains the Time-of-use tariffs (TOU) and Feed-in-tariffs (FIT) for all households. 
