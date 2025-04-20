# README - Motor Vibration Analysis

## Description
This project performs vibration analysis of a motor by comparing collected data against a known vibration pattern to identify potential issues. The code uses data processing and visualization techniques to assist in anomaly detection.

## Features
- Loads and processes motor vibration data
- Splits data into 256-sample intervals
- Calculates correlation between collected data and vibration pattern
- Identifies potential motor issues based on a correlation threshold
- Allows saving identified problem patterns
- Generates comparative visualization graphs

## Requirements
- Python 3.x
- Libraries:
  - numpy
  - pandas
  - matplotlib

## Data Files
- `PADRAOVIBRACAOMOTORSTREAM009CC.txt`: File containing standard vibration data from a properly functioning motor
- `VIBRACAOMOTORSTREAM009CC.txt`: File containing vibration data from the motor being analyzed

## Usage
1. Ensure data files are in the same directory as the script
2. Run the code in a compatible Python environment
3. Follow interactive prompts to:
   - Analyze correlation between collected data and standard pattern
   - Identify potential issues
   - Save new problem patterns when detected

## Correlation Threshold
The code uses a correlation threshold of 0.75 to determine whether the motor is functioning normally or may have issues. This value can be adjusted as needed.

## Visualizations
The code generates graphs comparing:
- Standard vibration pattern (blue)
- Collected data (green for normal, red for problem)
- Known problem patterns (pink)

## Output
The program provides:
- Correlation values between data and standard pattern
- Alerts when problems are detected
- Similarity percentage with known problems
- Option to save new problem patterns
