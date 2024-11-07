# College Data Analysis

This project analyzes a dataset of college student demographics, academic performance, and enrollment details. The analysis addresses research questions related to factors influencing student graduation rates.

## Project Structure

- **assignment7.ipynb**: Jupyter notebook with code for data cleaning, analysis, and hypothesis testing.
- **assignment7.html**: HTML version of the notebook.
- **collegeData.csv**: Dataset containing various attributes of college students.

## Dataset Description

- **Demographics**:
  - `SexCode`: Sex of the student.
  - `MaritalCode`: Marital status of the student.
  - `AgeAtStart`: Age of the student at the start of their education.
- **Academic Performance**:
  - `GPA`: Grade point average.
  - `HoursAttempt`: Course hours attempted.
  - `HoursEarned`: Course hours earned.
  - `gradFlag`: Graduation status.
- **Enrollment Details**:
  - `DaysEnrollToStart`: Days between enrollment and semester start.
  - `TransferCredits`: Transfer credits received.
  - `MinEFC`: Minimum expected family contribution.

## Research Questions and Hypotheses

1. **Transfer GPA and Graduation**:
   - Hypotheses for transfer GPA differences based on graduation status.
2. **Enrollment Timing and Graduation**:
   - Hypotheses regarding time between enrollment and semester start.
3. **Entrance Exam Scores and Graduation**:
   - Hypotheses about entrance exam scores based on graduation status.

Each hypothesis test uses a 5% significance level and excludes rows with missing values for the relevant feature.

## Requirements

To run the notebook, install these packages:

```bash
pip install numpy pandas scipy
```

## Instructions

1. **Open the Notebook**: Use Jupyter Notebook or JupyterLab to open `assignment7.ipynb`.
2. **Execute Cells**:
   - Run each cell sequentially to clean the data, test hypotheses, and evaluate results.

## Questions Answered

- Does transfer GPA differ significantly between students who graduate and those who do not?
- Does time between enrollment and semester start differ by graduation status?
- Are entrance exam scores significantly different for students based on graduation outcomes?

## License

This project is provided for educational purposes.
