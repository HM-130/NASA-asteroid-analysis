# Asteroid Data Analysis Project
*(Completed at age 14 - October 2024)*

## Overview
Conducted a comprehensive analysis of real-world asteroid orbital data to explore patterns and relationships based on Kepler's Laws of Planetary Motion. This project involved data cleaning, processing, and analysis using Python and Jupyter Notebooks.

## Project Motivation
I chose this as my first data science project because it allowed me to combine my interests in physics and computer science, solidifying my understanding of data analysis, astrophysics, and mathematics. 

Kepler's laws state:
1. Planets move in elliptical orbits with the sun as a focus.
2. A planet speeds up and slows down depending on its distance from the Sun but always covers equal areas in equal times.
3. A planet's orbital period is proportional to the size of its orbit (its semi-major axis).

I love learning about the universe, making this project an enjoyable experience. I particularly enjoyed the challenge of identifying and visualising relationships in orbital data inspired by real-world physics.

## Data Gathering
I found the data for this project on the NASA Jet Propulsion Lab’s small body database query website and downloaded it as a CSV file. I opened it in VSCode and analysed it in a Jupyter Notebook.

## Data Cleaning
- Renamed columns for readability.
- Removed columns of mostly NaN values.
- Ensured all columns had the correct data type.
- Replaced remaining NaNs with the mean/median/mode or 0, as appropriate.

## Correlations with Orbital Period
- Used the matplotlib library to produce scatter plots of the following variables against Orbital Period:
  - Eccentricity
  - Semimajor Axis
  - Inclination
  - Absolute Magnitude
- Used numpy and scikit-learn libraries for polynomial regression models.

### Polynomial Regression Models
- **Correlation Coefficient (Eccentricity vs. Orbital Period)**: 0.009385 (little to no linear relationship).
- **Kepler's 3rd Law Verification**: 0.986 (very strong correlation).
- **Additional Correlations**: Weak correlations observed for other variables.

## Brightness Grouping
- Used boolean masks to group asteroids based on Absolute Magnitude (brightness).
- Analyzed mean values for each group and produced bar charts comparing quantities.

## Plotting 2D Orbits
- Plotted the orbits of hypothetical asteroids with varying eccentricities.
- Plotted the 2D orbits of three asteroids based on their mean semimajor axis and eccentricity.

## Conclusions and Key Components
- Eccentricity has a weak correlation with orbital period, which is interesting because Kepler does not highlight this in his papers which can be found here: https://www.jstor.org/stable/4025081. Obviously this could just be coincidence in the data, but my model found an intriguing correlation nonetheless. 
- Non-linear regression models can be more effective than linear ones in analysing real-world data.
- Visualised the relationship between asteroid brightness and orbit size.

Completing this project enhanced my understanding of planetary motion and orbital mechanics. I learned that exploring non-linear relationships can provide valuable insights, and I strengthened my programming and data visualisation skills.

## Project Files
- [Analysis Notebook](analysis.ipynb): Main analysis performed on asteroid data.
- [Sample Data](sample_data.csv): A sample of the asteroid data used in the analysis.
