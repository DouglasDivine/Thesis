# Pyrolysis Data Analysis

Pyrolysis is a thermochemical conversion process used for the production of biofuels such as biochar, bio-oil, and syngas. The quality and yield of products obtained during biomass pyrolysis are dependent on several factors, such as biomass composition (proximate and ultimate analysis) and reaction conditions (temperature, heating rate, time). Therefore, it is imperative to understand the relationship between biomass composition, reaction conditions, and product yield during biomass pyrolysis.

## Project Overview

This project employs a data-driven machine learning (ML) approach to study the complex relationships between biomass composition, reaction conditions, and product yield in the context of pyrolysis. Additionally, we aim to make the findings interpretable, as many ML models are often regarded as black boxes.

## Key Findings

- Several machine learning models were compared to assess their performance in this context.
- Out-of-the-box models for Random Forest (RF), XGBoost, Artificial Neural Networks (ANN), and Gradient Boosting Regressor (GBR) performed exceptionally well and did not benefit significantly from hyperparameter optimization.
- In contrast, the performance of Stochastic Gradient Descent (SGD) and AdaBoost models improved substantially after hyperparameter optimization.
- The Gradient Boosting Regressor (GBR) model outperformed all other models due to its ability to handle various types of data and capture non-linear connections and interactions between variables.
- A notable conclusion from the permutation feature importance analysis is that the oxygen (O) content had the most impact on various parameters, including H/C ratio, O/C ratio, gas yield, oil yield, and biochar yield. This was closely followed by the pyrolysis temperature (PT).

## Repository Structure

- `data/`: Contains the dataset used for analysis.
- `notebooks/`: Jupyter notebooks used for data preprocessing, model training, and results interpretation.
- `scripts/`: Any relevant scripts used in the project.
- `results/`: Resulting plots, figures, and data outputs.

## Dependencies

- Python 3.x
- Jupyter Notebook
- Libraries (NumPy, Pandas, Scikit-learn, XGBoost, etc.)

## Getting Started

1. Clone this repository to your local machine.
2. Install the necessary dependencies using `pip install -r requirements.txt`.
3. Explore the Jupyter notebooks in the `notebooks/` directory for detailed analysis and findings.

## Contributors

- [Your Name]
- [Additional Contributors]

## License

This project is licensed under the [License Name] - see the [LICENSE.md](LICENSE.md) file for details.

## Acknowledgments

- Mention any sources of data, libraries, or tools that were helpful in this project.

Feel free to update and customize this README according to your project's specific needs.
