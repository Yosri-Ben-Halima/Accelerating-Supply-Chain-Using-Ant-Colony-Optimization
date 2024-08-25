# Accelerating Supply Chain Using Ant Colony Optimization

## 1. Introduction

This project focuses on optimizing inventory management and shipping decisions for a network of 50 stores. The aim is to minimize overall replenishment costs by finding the best routes and associated costs for shipping goods between stores. We employ the Ant Colony Optimization (ACO) algorithm, a metaheuristic inspired by the foraging behavior of ants, to solve this problem. ACO has been successfully applied in various fields such as transportation, logistics, and telecommunications.

## 2. Code Breakdown

The code is organized into three main sections:

### 2.1. Setting up the Problem-Specific Parameters

This section defines the parameters specific to the multi-store inventory management problem, including:
- Number of stores
- Demand at each store
- Current inventory levels
- Lead times for each store
- Shipping cost matrix
- Replenishment costs

### 2.2. Setting up the ACO Algorithm Parameters

In this section, we set up the parameters that control the behavior of the ACO algorithm:
- Number of ants
- Relative importance of pheromone trail ($\alpha$)
- Relative importance of distance and cost ($\beta$)
- Pheromone evaporation rate ($\rho$)
- Amount of pheromone deposited by ants ($q$)
- Number of iterations

### 2.3. Defining the Probability Function

The probability function calculates the likelihood of an ant moving from one store to another based on pheromone levels and the cost between stores.

### 2.4. Updating the Pheromone Trails

The pheromone trails are updated based on the routes taken by the ants and their associated costs, reinforcing the shorter and more efficient routes.

### 2.5. Running the Independent ACO Algorithm

This is the main part of the code where the ACO algorithm is executed. It involves generating random routes for each ant, calculating costs, and updating pheromone trails iteratively to find the best route and minimize costs.

### 2.6. Algorithm

The algorithm involves:
1. Initializing the best route and cost.
2. Iterating through a specified number of iterations, generating routes, calculating costs, and updating pheromone trails.
3. Returning the best route and its associated cost, along with updated inventory levels.

## 3. Dependencies

The project requires the following Python libraries:
- `numpy`
- `pandas`
- `joblib`
- `IPython.display`
- `time`

## 4. How to Run

1. Clone the repository.
2. Install the required libraries using `pip install -r requirements.txt`.
3. Run the main script in a Jupyter Notebook or directly using a Python interpreter.

## 5. Project Structure

- `OR Project ACO.ipynb`: Main notebook with the code and explanations.
- `OR Project ACO.html`: HTML format of the main notebook.
- `README.md`: Project overview and instructions.
- `requirements.txt`: List of required libraries.

## 6. Contributing

If you'd like to contribute to this project, feel free to fork the repository and submit a pull request. For major changes, please open an issue first to discuss what you would like to change.

## 7. License

This project is licensed under the MIT License - see the LICENSE file for details.


## 8. Contact

For any questions or suggestions, please reach out via Email on [yosri.benhalima@ept.ucar.tn].
