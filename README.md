# Module5Challenge
The task is to create:
1. A financial planner for emergencies.The members will be able to use this tool to visualize their current savings. The members can then determine if  they have enough reserves for an emergency fund.
2. A financial planner for retirement. This tool will forecast the performance of their retirement portfolio in 30 years. To do this, the tool will make an Alpaca API call via the Alpaca SDK to get historical price data for use in Monte Carlo simulations.
# Technologies
- python 3.9.12
- JupyterLab
- libraries: pandas, matplotlib, os, requests, json, dotenv, alpaca-trade-api, MCForecastTools
- MacOs
# Installation
If you want to run the program yourself and/or enter different data, do the following:
1. To install the project files, go to the GitHub page for the workshop, click on the green Code button, then download the repository as a ZIP file. 
![image](https://user-images.githubusercontent.com/111472420/193461124-3e1c4693-e6b7-435b-a4cb-68ac726ac1fe.png)

2. Unpack a zip file into the directory you can operate from in JupyterLab. 
<img width="965" alt="Screen Shot 2022-10-17 at 7 41 28 PM" src="https://user-images.githubusercontent.com/111472420/196323543-2c0e0058-c38e-4339-af6a-761123050e21.png">

3. Create environmet file with your Alpaca API key, Alpaca Secret key and Alpaca URL via Terminal.
<img width="596" alt="Screen Shot 2022-10-17 at 8 32 52 PM" src="https://user-images.githubusercontent.com/111472420/196329414-28ca083b-e09c-4ad5-9922-4e57402cad5b.png">

4. Open financial_planning_tools.ipynb and Run the code!
<img width="828" alt="Screen Shot 2022-10-17 at 8 34 11 PM" src="https://user-images.githubusercontent.com/111472420/196329709-0c0d8c50-fb10-4367-9e48-27fba82c8907.png">
# Financial planner for emergencies 
There are 3 possible outcomes:
- total portfolio value succeeds the emergency fund value
- total portfolio value equals to the emergency fund value
- total portfolio value fails the emergency fund value
<img width="821" alt="Screen Shot 2022-10-17 at 8 39 06 PM" src="https://user-images.githubusercontent.com/111472420/196330262-77131450-6b6e-43ce-8988-4d92b5d125c2.png">
# Financial planner for retirement
There are two ready for use MCSimulator templates (for 30 and 10 years).
You can adjust:
- start and end dates for collective data
- number of trading days (252 * years)
- stocks/bonds ratio (weights)
- number of simulations

<i>The visualized results of your calculations will be saved in the same directory.</i>

<img width="1145" alt="Screen Shot 2022-10-17 at 8 54 05 PM" src="https://user-images.githubusercontent.com/111472420/196331751-e7844c2a-75c3-4777-b30e-f92cada81482.png">

![MC_10year_sim_plot](https://user-images.githubusercontent.com/111472420/196332183-25b85e23-990a-495c-8ae5-0297c3ca9ce5.png)
![MC_10year_dist_plot](https://user-images.githubusercontent.com/111472420/196332206-87bc050a-0fb9-4943-a758-d154b3d48f8f.png)
