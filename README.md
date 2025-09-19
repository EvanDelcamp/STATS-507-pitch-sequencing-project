# pitch-sequencing-project
 This project explores the use of a multi-task LSTM model to predict pitch type, zone, and strike probability for MLB's top pitchers based on contextual features.

## Data

- Source: [MLB Statcast](https://baseballsavant.mlb.com/) via [pybaseball](https://github.com/jldbc/pybaseball)
- Pitchers: Top 20 MLB starters from 2023–2024 by FanGraphs WAR

## Features

- Target Variables:
  - Pitch Type (e.g., FF, SL, CH)
  - Custom Strike Zone Location
  - Strike vs Ball Classification
- Multi-task learning using LSTM
- Embedding layer for pitcher ID
- Custom strike zone and preprocessing logic

# How to run:
1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/pitch-sequencing-project.git
   cd pitch-sequencing-project

2. pip install -r requirements.txt

3. The "STATS 507 Final Project - Predicting Pitch Sequences Multiple Pitchers" Jupyter Notebook contains all code for pulling the dataset, setting up the LSTM model, as well as training and evaluating the model.

4. Occasionally, the Baseball Savant Server has errors loading data, so if an error occurs, rerunning the cell usually fixes it.

5. Trained .pt models are stored in the models folder, and the final model used for the paper is also stored in the notebooks folder, for easy access when running the notebook code.

# Results Summary
Strike F1 Score: 0.59
Pitch Type Accuracy: 44.71%
Zone Accuracy: 32.90%
Strike Accuracy: 56.81%

## Final Report

The final 2-page IEEE-style paper summarizing this project can be found [here](https://github.com/EvanDelcamp/STATS-507-pitch-sequencing-project/blob/main/Preparing_for_the_Pitch__Using_Deep_Learning_to_Anticipate_MLB_s_Toughest_Pitchers.pdf).

# Contact:
For questions or collaboration ideas, feel free to reach out at [evandelcamp@gmail.com].
