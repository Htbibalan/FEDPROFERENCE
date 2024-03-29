# FEDPROFERENCE
The repository stores the codes and data files collected in an experiment in which protein restricted and non-restricted mice were placed in choice boxes to choose between diets varying in nutritional value to test their preference as a function of their diet history.

#### Number of animals: 40 mice, 20 male and 20 female

#### Age: 6 weeks at the time of arrival, ~8 weeks at the begining of the experiment depending on batch number

#### Strain:  C57BL/6NRj



![paradigm](https://github.com/Htbibalan/FEDPROFERENCE/blob/main/source/FEDXD_paradigm.png)
![protocol](https://github.com/Htbibalan/FEDPROFERENCE/blob/main/source/FEDXD_protocol.png)
*The figures show the overview of the 4 batches used in this experiment, plus the overall protocol for each cohort of animals and the choices in "food preference sessions"*


#### Cohorots
* 2 main cohorts of protein-restricted and non-restriced mice, each containing 20 mice distributed in 4 batches
* **FEDXD01-10 F** and **FEDXD01-10 M** are protein-restricted(PR) mice
* **FEDXD11-20 F** and **FEDXD11-20 M** are non-restricted(NR) mice
* This [Metafile](https://github.com/Htbibalan/FEDPROFERENCE/blob/main/FEDXD_METAFILE.xls) shows the corresponding batches for each mouse 

#### Experiment protocol details
* All the mice started with 3 days of training with FEDs filled with a 50%-50% mix of Casein 5% and 20% pellets. On the **first day the FEDs are set on free-feeding mode** and for the **next 2 days on FR1 mode**.
*  After training, depending on the batch number, the mice experienced 0-2 days of gap in standard cages with access to regular chow.
*  Susbsequently PR mice were maintained on 5% Casein pellets(large pellets in standard cages, not FED cages) for 7 days.
* NR mice were maintained on 20% Casein pellets (large pellets in standard cages, not FED cages) for 7 days.

* After 7 days on diet, mice were placed in choice boxes(each mouse in a FED cage with access to two separate FED units at the same time)
* As shown in the figure at the top of this page, the routine of choice sessions for each diet group(PR and NR ) is as follows:
7 days standard cage with large pellets special diet &#8594; 1 day choice session 1 (**FR1 20% vs 5% casein**) &#8594; 3 days standard cage/large pellet/special diet &#8594; 1 day choice session 2 (**FR1 20% casein vs Sucrose**) &#8594; 3 days standard cage/large pellet/special diet &#8594; 1 day choice session 3 (**FR 5% casein vs Suc**) &#8594; 3 days standard cage/large pellet/special diet &#8594; choice session 4 (**CE 5% casein vs Suc**)

*  ***Auxiliary procedure:*** After all choice sessions were over, mice spent 3-7 days in standard cages maintained on their original special diet and then finally were scanned in EchoMRI mahchine. 

#### Food and bodyweight measurment
* From the first day of training, bodyweight was measured every 3 days, i.e. 9 times in total.
* The weight of the pellets in the standad dispenser was once measured after 7 days on special diet &#8594; then measured every 3 days , i.e. on each choice session day when the animals were transfered to choice boxes.



#### GitHub respository structure
* **/data** stores FED files obtained during training and choice sessions

***note1:*** 
FED015_041223_00.CSV and FED016_041623_00.CSV are **corrupted**, i.e FED15 and FED16 **did not save the data** on choice session 1 and 2 for mouse FEDXDM18, so **must be excluded from analysis.**

***note2:***
Due to failure in some of the FED units, mice **FEDXD12F** because of FED JAMMING on the 3rd session and, **FEDXD15M, FEDXD20F and FEDXD20M** because of program error on FED units did not have their choice session on the designated dates. Therefore after the last session for the rest of the mice, these 4 mice experienced 3 more days on special diet in standard cages and afterwards were placed in choice boxes for their corresponding sessions.

* **/notebooks** will store python scripts to analyse or plot data
* **/plots** contains plots generated either via python script or plots obtained from FED3VIZ
* **/results** This file [FEDXD_CHOICE_RESULTS_OVERALL.xlsx](https://github.com/Htbibalan/FEDPROFERENCE/blob/main/results/FEDXD_CHOICE_RESULTS_OVERALL.xlsx) stores all the data of bodyweight, food intake, EchoMRI and data extracted from FED files via FED3VIZ
* **/source** containes figure files or any potential .py fi

Look at the [Metafile](https://github.com/Htbibalan/FEDPROFERENCE/blob/main/FEDXD_METAFILE.xls) for an overview of diets, batches, session numbers, etc.




