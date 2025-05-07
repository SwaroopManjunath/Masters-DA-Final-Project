# The Tale of Three Economies: India, Germany, and the World (2002-2023)

## Project Overview

This project analyzes the Gross Domestic Product (GDP) trends, in constant 2015 US dollars, for India, Germany, and the global economy from 2002 to 2023. It compares Germany's stable economic performance with India's dynamic growth trajectory, set against the backdrop of global economic expansion. The analysis includes data processing, visualization, statistical analysis, normality testing, Central Limit Theorem demonstration, and hypothesis testing to explore economic patterns and differences.

The project is structured to provide clear insights through time series plots, descriptive statistics, distribution fittings, Q-Q plots, rolling mean distributions, and a Welch's t-test comparing mean GDPs of India and Germany. All findings are supported by detailed mathematical calculations and visualizations with a consistent color scheme: green for World, orange for Germany, and blue for India.

## Repository Contents

- **Data Files**:
  - `gdp-worldbank-constant-usd.csv`: Contains GDP data (constant 2015 US$) for India, Germany, and the World from 2002 to 2023, sourced from Our World in Data.
  
- **Analysis Files**:
  - `Final Project GDP1.ipynb`: Jupyter Notebook containing Python code for data processing, visualization (e.g., time series and density plots), and statistical analysis. Libraries used include pandas, numpy, matplotlib, seaborn, and scipy.
  
- **Documentation**:
  - `Final Report Draft.pdf`: A comprehensive report detailing the project methodology, findings, and visualizations. It includes sections on data collection, descriptive statistics, normality testing, Central Limit Theorem, and hypothesis testing.
  - `README.md`: This file, providing an overview and guide to the project.

- **Visualizations** (Generated in Notebook):
  - Time series plots for India and Germany GDP (in trillions).
  - Time series plot for World GDP (in trillions).
  - Density plot of normalized GDP for India, Germany, and World.
  - Additional plots in the report (e.g., histograms, Q-Q plots, rolling mean distributions, and mean GDP comparison).

## Installation and Setup

To run the analysis, ensure you have Python 3.12 or later installed along with the required libraries. Follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/the-tale-of-three-economies.git
   cd the-tale-of-three-economies
   ```

2. **Install Dependencies**:
   Create a virtual environment and install the required packages:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install pandas numpy matplotlib seaborn scipy
   ```

3. **Run the Notebook**:
   Launch Jupyter Notebook and open `Final Project GDP1.ipynb`:
   ```bash
   jupyter notebook
   ```

4. **Data Requirements**:
   Ensure `gdp-worldbank-constant-usd.csv` is in the same directory as the notebook. The notebook assumes this file for data loading and processing.

## Usage

1. **Data Processing**:
   - The notebook loads the GDP data, filters for 2002–2023, and scales values to trillions (T) for clarity (e.g., dividing by 1e12 for values ≥ 1e12).
   - Separate datasets are created for India/Germany and World to handle different scales.

2. **Visualizations**:
   - **Time Series Plots**: Visualize GDP trends for India/Germany and World separately.
   - **Density Plot**: Compare normalized GDP distributions using kernel density estimation (KDE).
   - Additional visualizations (e.g., histograms, Q-Q plots) are described in the report.

3. **Statistical Analysis**:
   - **Descriptive Statistics**: Compute mean, median, standard deviation, and quartiles.
   - **Normality Testing**: Fit normal distributions and generate Q-Q plots to assess normality.
   - **Central Limit Theorem**: Demonstrate normality of 5-year rolling means.
   - **Hypothesis Testing**: Perform Welch's t-test to compare mean GDPs of India and Germany.

4. **Report**:
   - Refer to `Final Report Draft.pdf` for a detailed narrative, methodology, and visualizations (e.g., Graphs 1–14).

## Key Findings

- **India**: Exhibits rapid GDP growth with higher variability (mean: 1.88T, std: 0.72T), reflecting an emerging economy.
- **Germany**: Shows stable GDP with lower variability (mean: 3.32T, std: 0.27T), indicative of a mature economy.
- **World**: Displays steady growth in aggregate economic output (mean: 70.97T, std: 12.88T).
- **Normality**: GDP distributions for India and Germany are approximately normal, with minor deviations in extreme years (e.g., 2008, 2020).
- **Hypothesis Test**: Welch's t-test (t = -8.804, p < 0.001) rejects the null hypothesis, confirming a significant difference between India's and Germany's mean GDPs.
- **Central Limit Theorem**: 5-year rolling means approximate normal distributions, supporting statistical inference.

## Project Structure

The analysis is divided into five parts, as outlined in the report:

1. **Data Collection and Preparation**: Data retrieval, scaling, and time series visualization.
2. **Distributions**: Descriptive statistics and histogram/KDE comparisons.
3. **Normality Testing**: Normal distribution fitting and Q-Q plots.
4. **Central Limit Theorem**: 5-year rolling mean distributions.
5. **Hypothesis Testing**: Welch's t-test comparing India and Germany mean GDPs.

## Dependencies

- Python 3.12+
- pandas
- numpy
- matplotlib
- seaborn
- scipy
- Jupyter Notebook

## References

- Bolt, J., & van Zanden, J. L. (2024). *Maddison style estimates of the evolution of the world economy: A new 2023 update*. Journal of Economic Surveys.
- Roser, M., et al. (2023). *Our World in Data: Economic Growth*. https://ourworldindata.org/economic-growth
- Casella, G., & Berger, R. L. (2002). *Statistical Inference*. Duxbury Press.
- Field, A. (2013). *Discovering Statistics Using IBM SPSS Statistics*. SAGE Publications.
- Mankiw, N. G. (2020). *Principles of Economics*. Cengage Learning.

## Authors

- Varun Hirethotlukere Shamaraju
- Swaroop Kodagahalli Manjunathaswamy
- Divya Koriya
- Pooja Shreni Addisherla

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgments

- Data sourced from *Our World in Data* (https://ourworldindata.org).
- Statistical methods inspired by *Statistical Inference* by Casella and Berger.
