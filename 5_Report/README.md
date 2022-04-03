## Domestic Electricity Bill System

## Description

The Domestic Power Bill Calculation Processes project is a web application designed to automate the electricity board's billing system. The goal of this project is to create a system that will partially computerise the job done by the Power Board, such as creating monthly electricity bills, keeping track of consuming units of energy, keeping track of customers, and keeping track of previous unpaid bills. It primarily focuses on calculating the number of units utilised over a given period of time and the amount of money that must be paid to electricity offices. Visual studio code was used to write the code for this project. This project employs a multi-file and multi-platform strategy (WSL).

## Features
- Architecture of project is simple and easy to understand the code.
- Calculating the total load and units consumed.
- Calculating the cost per unit based on the area and units consumed.
- Displaying the amount.

## SWOT Analysis

![Screenshot (13)](https://user-images.githubusercontent.com/101035721/160985201-e87b3862-c4b3-4a8b-82f0-32e753134119.png)

## 5W's & 1H
![Screenshot (16)](https://user-images.githubusercontent.com/101035721/160987420-69acef7b-8744-4d5c-8899-f42870fd5262.png)

## Requriements

## High Level Requriements
<html>
<body>
<!--StartFragment-->

HLR(ID) | Description
-- | --
HLR01 | Calculates electricity bill at Rural areas
HLR02 | Calculates electricity bill at Urban areas
HLR03 | Calculates total Amount at Domestics places
HLR04 | Calculates total unit consumed at Domestics places

<!--EndFragment-->
</body>
</html>

## Low Level Requriements
<html>
<body>
<!--StartFragment-->

LLR(ID) | Description
-- | --
LLR01_HLR_01 | Electricity bill calculation at Rural areas if(units<30)
LLR02_HLR_01 | Electricity bill calculation at Rural areas if(units>30 && units <100)
LLR03_HLR_01 | Electricity bill calculation at Rural areas if(units>101 && units <200)
LLR04_HLR_01 | Electricity bill calculation at Rural areas if(units<200)
LLR05_HLR_02 | Electricity bill calculation at Urban areas if(units<30)
LLR06_HLR_02 | Electricity bill calculation at Urban areas if(units>30 && units <100)
LLR07_HLR_02 | Electricity bill calculation at Urban areas if(units>101 && units <200)
LLR08_HLR_02 | Electricity bill calculation at Urban areas if(units<200)

<!--EndFragment-->
</body>
</html>

# **Behavior Diagrams**
## High Level Behavioural Diagram
![b diag](https://user-images.githubusercontent.com/101035721/160991074-9520623b-a4db-4cf1-95c8-23f02467d59a.jpg)

## Low Level Behavioural Diagram
![lb dia](https://user-images.githubusercontent.com/101035721/160991261-0d075f3e-7181-426e-9667-dcd594b7fbe0.jpg)

# **Structural Diagram**
## High Level Structural Diagram
![s dia](https://user-images.githubusercontent.com/101035721/160991645-a22227d3-774d-430c-9e38-d0f88f74ae21.jpg)

## Low Level Structural Diagram
![ls diah](https://user-images.githubusercontent.com/101035721/160991781-b8e571e9-d81c-40df-bc6a-c0d57ad0b016.png)

# **Test Plan and Output**
## High-Level Requriements
<html>
<body>
<!--StartFragment-->

Test ID | HLR | Description | Inputs | Expected O/P | Actual O/P
-- | -- | -- | -- | -- | --
TD01 | HLR01 | Calculating Rural areas electricity bill | Choice | Sucess | Sucess
TD02 | HLR02 | Calculating Urban areas electricity bill | Choice | Sucess | Sucess
TD03 | HLR03 | Calculating total amount at Domestics places | Choice | Sucess | Sucess
TD04 | HLR04 | Calculates total unit consumed at Domestics places | Choice | Sucess | Sucess

<!--EndFragment-->
</body>
</html>

## Low-Level Requriements
<html>
<body>
<!--StartFragment-->

Test ID | LLR | Description | Inputs(Units) | Expected O/P (Amount) | Actual O/P (Amount)
-- | -- | -- | -- | -- | --
TD01 | LLR01_HLR01 | Electricity bill calculation at Rural areas if(units<30) | 25 | 78.75 | 78.75
TD02 | LLR02_HLR01 | Electricity bill calculation at Rural areas if(units>30 && units <100) | 45 | 198.0 | 198.0
TD03 | LLR03_HLR01 | Electricity bill calculation at Rural areas if(units>101 && units <200) | 112 | 666.4 | 666.4
TD04 | LLR04_HLR01 | Electricity bill calculation at Rural areas if(units<200) | 235 | 1598.0 | 1598.0
TD05 | LLR05_HLR02 | Electricity bill calculation at Urban areas if(units<30) | 15 | 48.75 | 48.75
TD06 | LLR06_HLR02 | Electricity bill calculation at Urban areas if(units>30 && units <100) | 55 | 258.5 | 258.5
TD07 | LLR07_HLR02 | Electricity bill calculation at Urban areas if(units>101 && units <200) | 101 | 631.25 | 631.25
TD08 | LLR08_HLR02 | Electricity bill calculation at Urban areas if(units<200) | 201 | 1467.3 | 1467.3

<!--EndFragment-->
</body>
</html>

# **Output ScreenShots**
![Screenshot (3)](https://user-images.githubusercontent.com/101035721/161391501-513e331a-89ce-44f5-99a5-1f49b75b4c7f.png)
![Screenshot (4)](https://user-images.githubusercontent.com/101035721/161391504-17a0b305-df5b-4cef-b735-e0368b960d76.png)