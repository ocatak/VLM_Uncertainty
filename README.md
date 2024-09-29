# LLM Uncertainty Quantification via Convex Hull Analysis

This repository contains code and analysis for uncertainty quantification in large language models (LLMs) using **Convex Hull Analysis**. The notebook focuses on comparing different conditions and calculating statistical correlations to assess the model's uncertainty.

## Project Overview

Uncertainty quantification is an important aspect when dealing with large language models, especially in high-stakes applications where confidence in model predictions is critical. This project employs **Convex Hull Analysis** to examine uncertainty across various conditions and utilizes statistical methods (Pearson correlation) to quantify relationships.

## Features

- **Convex Hull Analysis**: 
  - Convex Hull Areas are calculated for each condition, allowing for a comparison of uncertainty across different settings.
- **Statistical Correlation**:
  - Pearson correlations and p-values are calculated between the mean Convex Hull Area per image and values under various conditions.
  - Results are presented in a summary table for easy interpretation.

## Repository Contents

- **`Data-Analysys-LLM-Uncertainty.ipynb`**: The main Jupyter notebook that includes data loading, analysis, and results.
- **Data**: The repository assumes a `comparison_df` DataFrame, which should be preloaded or provided in the appropriate section.

## Requirements

To run this project, you'll need the following Python libraries:
- `pandas`: For data manipulation and DataFrame operations.
- `scipy`: For statistical computations (Pearson correlation).
- `numpy`: For numerical operations.

You can install these dependencies using:
```bash
pip install pandas scipy numpy
```

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/LLM-Uncertainty-Quantification.git
   cd LLM-Uncertainty-Quantification
   ```

2. Install the necessary dependencies as outlined above.

3. Run the Jupyter notebook `Data-Analysys-LLM-Uncertainty.ipynb`:
   ```bash
   jupyter notebook Data-Analysys-LLM-Uncertainty.ipynb
   ```

4. Follow the notebook steps:
   - The code will load the `comparison_df` dataset, perform Convex Hull Analysis, and calculate Pearson correlations.
   - Results will be displayed as tables summarizing correlations and p-values.

## Example Output

The notebook provides the following output for each condition:

| Condition | Correlation | P-value |
|-----------|-------------|---------|
| 0.001_all | 0.072       | 0.028   |
| 100_all   | 0.497       | 3.60e-59|
| 25_all    | 0.676       | 2.35e-125|
| 50_all    | 0.814       | 1.25e-221|
| 75_all    | 0.749       | 6.84e-168|

## Contributions

Feel free to fork this repository, submit issues, or make pull requests. Contributions to improve the analysis or extend the methods are welcome.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
