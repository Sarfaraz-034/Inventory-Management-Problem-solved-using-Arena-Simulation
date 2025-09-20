## Inventory Management Problem Simulation using Arena
This project presents a simulation model for an inventory management system, developed using Rockwell Arena. The model analyzes the performance of a standard (s, S) inventory policy for a company that sells a single product.

### 📝 Problem Statement
A company aims to simulate its inventory system to optimize its ordering strategy. The key characteristics of the system are as follows:
Customer Arrivals: The time between customer arrivals follows an exponential distribution with a mean of 1 day.
Demand Size: The quantity demanded by each customer is uniformly distributed between 4 and 8 units.
Inventory Policy: The company uses an (s, S) policy. When a customer demand arises, it is satisfied immediately if the current inventory level is sufficient. If the inventory level is less than the demand, the sale is lost, and the customer leaves.
Ordering Process: An inventory manager checks the stock level every day. If the inventory is below the safety stock level (s), an order is placed for production.
Production: The production time for each product follows a normal distribution with a mean of 0.1 days and a standard deviation of 0.01 days. Production stops once the inventory level reaches the target stock (S).
Simulation End Condition: The simulation will run until it has processed 140 customers.
The management's goal is to measure the performance parameters of this inventory system through simulation.


### 🎯 Project Objectives
The primary goals of this simulation are:
Develop a Model: Construct a detailed simulation model of the inventory management system described above using Arena.
Simulate and Visualize: Run the model to observe the system's dynamics and visualize the flow of customers and inventory.
Measure Performance: Analyze key performance metrics, including:
Average inventory level
Number of lost customers
Total demand met
Production time

## 🛠️ Model Details & System Logic
Here is a breakdown of the components and logic used to build the Arena model:
System Requirements: Windows OS and Rockwell Arena simulation software.
Entities:
Customers: Arrive to place orders.
Raw Materials: Used in the manufacturing process.
Resource:
Operator 1: A resource required for the manufacturing process.
Process: Manufacture.
Process Action: The manufacturing process is modeled using a Seize Delay Release logic, where the operator is seized for the duration of the production time.
Queue Discipline: All queues operate on a First-Come, First-Served (FCFS) basis.

### 🚀 How to Run the Simulation
Ensure you have Rockwell Arena installed on a Windows operating system.
Clone this repository or download the .doe model file.
Open the file in Arena.
Run the simulation to observe the model and generate the results report.
📊 Results & Analysis
After running the simulation, Arena will generate a comprehensive report. The key metrics to analyze from this report are the average inventory level, the total number of lost customers, and the percentage of demand met. These results will provide valuable insights into the effectiveness of the current (s, S) inventory policy and help identify areas for improvement.
