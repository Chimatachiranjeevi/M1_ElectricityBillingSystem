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