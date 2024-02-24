# Marketing Strategy Optimization

*This project was a part of MIT's course 15.093 Optimization Methods.*

## Purpose and Overview
The project aims to design a framework for optimizing a marketing strategy given a fixed budget, multiple marketing options, and varying constraints and optimization goals. Four marketing options are included here: Targeted Online Advertising, E-mail, Print Media, and Influencer Marketing. However, the frameworks and formulations we provide can be easily extended to fit any combination of marketing options.

## Data
The data for this project is synthetically generated. We have four different marketing options for a product: Targeted Online Advertising (max investment value: $990), E-mail (max investment value: $500), Print Media (max investment value: $700), and Influencer Marketing (Social Media) (max investment value: $600). For each of these options, we have the following variables in the data: 

- **Investment Amount:** Each row defines an investment amount that generates an expected number of views and purchases made. 
- **Number of People Reached:** Number of people who view the marketed advertisement
- **Sales Generated:** Number of people who purchase the product after getting influenced by the marketing through the given platform. 

For Data Pre-Processing: We interpolated the data to create a continuous function from our discrete data points, allowing the optimization model to work effectively with any investment amount within the provided ranges. 

## Methodology
- Two Baseline Models with only budgetary constraints with the following objectives: (a) Maximizing Views (b) Maximizing Sales
- Mixed Integer Optimization
- Additional Constraints: fixed budgetary allocation to specific marketing options, if-then constraint, balanced portfolio constraint
- Dual: The dual interpretation of our project is also a useful framework to consider as we begin adding constraints to our problem. Below we take the fixed allocation constraint example and extract the dual values from our model.

    <img width="850" height="300" alt="image" src="https://github.com/Sanya-Chauhan/Optimizing_Marketing_Strategies/assets/116647771/4a9b1313-950a-4724-910f-92be1b8444a2">





## Graphic User Interface
To have a user-friendly interface, we created a Streamlit web app that would allow the users to input their budget, choose an objective, and get the optimal investment amounts according to the model, as well as expected buys/views (based on the chosen objective). This image below is for a basic model only with one budgetary constraint. Additional constraints can be added based on the user’s needs.

<img width="850" height="500" alt="Screenshot 2024-02-24 at 6 41 05 PM" src="https://github.com/Sanya-Chauhan/Optimizing_Marketing_Strategies/assets/116647771/5af744e7-c421-434b-aacd-abe47a20f817">

## Impact and Conclusion
A Deloitte 2023 CMO Survey said that marketing makes up 13.6% of a company's annual expenditure. In the age of data-driven strategy, our modeling framework can help executives and decision-makers efficiently allocate marketing capital given a company's constraints and goals. Our model achieved up to a 14% increase in views for the same budget, and up to a 23% increase in buys, again given the same budget, when compared to the baseline. We also explore how a user could customize these models to best fit their needs using constraints and extensions, such as a time or a region index or a multi/weighted objective function. In conclusion, given the correct data, optimization is a useful framework that can be effectively applied to create business efficiencies in the marketing field. 

<!-- 
## For more details
Read the project report and presentation [here](https://drive.google.com/drive/folders/1InYuiOKOBdG6bBBSrPYW0WcpqTlEn5uc?usp=sharing).
-->
