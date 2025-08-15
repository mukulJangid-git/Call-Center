# Call-Center

Call Center Operations Optimization: A Simulation-Based Approach
📝 Overview
This project utilizes a simulation-based approach to analyze and optimize the operations of a call center. By modeling customer arrivals, service times, and various real-world scenarios, this analysis provides data-driven insights into staffing levels, operational costs, and overall customer experience. The simulations are built from the ground up using Python, with a focus on applying queueing theory to solve practical business problems.

This project is highly relevant for roles in operations management, marketing analytics, customer experience, and business consulting, as it demonstrates how to analyze, simulate, and optimize real-world service systems.

✨ Features & Key Concepts Modeled
This simulation models a multi-server (M/M/s) queueing system and explores several scenarios to provide a comprehensive analysis:

👥 Staffing Level Analysis: Simulates the call center with varying numbers of agents to determine the optimal staffing level required to meet specific service level agreements (SLAs), such as keeping the 95th-percentile wait time under 5 minutes.

🕒 Time-Varying Demand: Models fluctuating customer arrival rates to reflect real-world demand patterns, including morning and afternoon rush hours and midday lulls.

🚶 Customer Abandonment: Simulates realistic caller behavior by introducing a "patience threshold," where customers may hang up if their wait time exceeds a certain limit. This helps in analyzing customer loss due to inadequate staffing.

☕ Agent Break Scheduling: Observes the operational impact of scheduling 15-minute agent breaks, which temporarily reduces the number of available agents.

💰 Cost-Based Optimization: Balances labor costs against customer wait costs to determine the most cost-effective number of agents, minimizing total operational expenses.

📊 Sensitivity & Risk Analysis: Runs simulations over multiple days to analyze the day-to-day variability in performance metrics and identify potential worst-case scenarios.

📈 Performance Metrics & Visualization: Calculates and visualizes key performance indicators (KPIs) including:

Mean and 95th percentile wait times

Average queue lengths

Abandonment rates

Wait-time distributions using histograms to mimic an operations dashboard.

🛠️ Technologies & Libraries Used
Python: The core programming language used for the simulation.

NumPy: For numerical operations and generating random numbers based on statistical distributions (Poisson and Exponential).

Matplotlib: For creating visualizations and plotting the results of the simulations.

Pandas: For organizing and displaying the simulation results in a structured tabular format.

🚀 How to Run the Project
To run this project, you will need to have Python and Jupyter Notebook installed.

Clone the repository:

Bash

git clone <your-repository-url>
Navigate to the project directory:

Bash

cd <your-project-directory>
Install the required libraries:

Bash

pip install numpy matplotlib pandas
Run the Jupyter Notebook:

Bash

jupyter notebook Call_Center.ipynb
This will open the notebook in your browser, where you can run the code cells to see the simulations and their results.

⚙️ Simulation Parameters
The core parameters of the simulation can be adjusted in the notebook to model different scenarios:

Lamda (λ): The average rate of incoming calls per hour (Poisson process).

Mu (μ): The average number of calls an agent can serve per hour (Exponential service times).

shift_hours: The duration of the simulation, typically an 8-hour shift.

s: The number of agents (servers) available.

By modifying these values, you can explore how different call volumes, service efficiencies, and staffing levels impact the overall performance of the call center.
