### Project status: 
This repository is linked to a 2 part blog series titled 'Build and train ML models with a data mesh design pattern on AWS
# Practice ML in a Data Mesh environment
## Description
This project allows to:
1. Build a Data Mesh enviroment with 3 different accounts using Lake Formation (LF) tags and include ML()
2. Run a ML lifecycle in a Data Mesh environment

## Usage
To use this workshop, you need to first have 3 different accounts that will represent a Producer, Central, and Consumer in a Data Mesh architecture. In each of those accounts you need to run the cloud formations template provided. You first run the the cloud formation for the Central account, then for the Producer account and finally for Consumer account. The cloud formation templates should each be run separetely in each account one at a time. 

Next you need to follow the step-by-step guide to pass a dataset from the Producer account to the Consumer account.

Finally you can start using the notebook(s) to perform machine learning.

## Roadmap
We are planning in the near future to add the resource access manager instead of LF tags

## Authors and acknowledgment
Special thanks to:
- Hasan Poonawala
- Karim Hammouda
- Benoît de Patoul

