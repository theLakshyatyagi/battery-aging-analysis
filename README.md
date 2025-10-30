# Battery Aging Analysis
This project demonstrates a simulation-based study of battery degradation using Electrochemical Impedance Spectroscopy (EIS) and Incremental Capacity Analysis (ICA). It also includes a machine learning model to predict the current capacity of a battery as it ages through multiple charge–discharge cycles.

## Features
Task A – EIS Visualization:
Simulates impedance data (R(Z) vs Im(Z)) across 100 aging cycles and visualizes it in a 3-D plot.

Task B – Incremental Capacity Analysis (ICA):
Plots charge and discharge incremental-capacity curves and analyzes peak shifts with aging.

Task C – Capacity Prediction:
Trains a Random Forest Regressor to predict current capacity from EIS parameters and cycle count.

Comprehensive Visualizations:
Includes 3-D plots, ICA curves, and ML evaluation scatterplots.

## Technologies Used
Python 3

NumPy – numerical simulation

Pandas – data handling

Matplotlib / mpl_toolkits.mplot3d – visualization

Scikit-learn – machine-learning regression and metrics

## Project Structure
Battery_Aging_Analysis.ipynb   → Main notebook

README.md                      → Project documentation

## How to Run
1. Clone this repository:
   git clone https://github.com/<your-username>/battery-aging-analysis.git
   cd battery-aging-analysis
2. Install dependencies:
   pip install -r requirements.txt
3. Run the notebook in Jupyter or VS Code and execute all cells.

## Example Output
Task A – 3-D EIS Plot
Shows how impedance values evolve across 100 cycles.

Task B – Incremental Capacity Analysis
Displays charge/discharge curves (dQ/dV vs Voltage) and 3-D ICA peak evolution with aging.

Task C – Capacity Prediction
Sample Predictions:
Example	ActualCapacity	PredictedCapacity	Difference
   0	      0.5241	         0.5128  	      0.011
   1	      0.8356	         0.8222	        0.0134
   2	      0.2987	         0.3069	       −0.0082
   3	      0.6654	         0.6532	        0.0122
   4	      0.4021	         0.4107	       −0.0086

Model Evaluation:
RMSE: 0.0847
MAE: 0.0673

Scatter Plot:
Predicted vs Actual capacity shows a near-diagonal fit, indicating reliable predictions.

## Future Improvements
Use real EIS and ICA datasets instead of simulated values

Integrate temperature and SOC features for better predictions

Experiment with neural networks for advanced regression

Add automated report generation for each test cycle

# Author
Lakshya Tyagi

Delhi, India
