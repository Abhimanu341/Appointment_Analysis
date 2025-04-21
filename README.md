
# Medical Appointment No Shows Dataset Cleaning

This repository contains the cleaned version of the **Medical Appointment No Shows** dataset. The dataset was cleaned and preprocessed for analysis, focusing on handling missing values, removing duplicates, standardizing text values, and converting date formats.

## Objective
The goal of this project was to clean and prepare the raw dataset for further analysis, including handling:
- Missing values
- Duplicates
- Inconsistent formats (text values and date formats)
- Column name standardization
- Data type corrections

## Steps Performed:
1. **Handled Missing Values**: No missing values were found in the dataset.
2. **Removed Duplicates**: The dataset was checked for duplicates and none were found.
3. **Standardized Text Values**:
   - Ensured consistent gender values (`F` for Female, `M` for Male).
   - Standardized the `Handcap` column to numeric values.
4. **Converted Date Formats**:
   - Both `ScheduledDay` and `AppointmentDay` columns were converted to `datetime` format.
5. **Renamed Columns**:
   - Column names were standardized to be lowercase and without spaces (e.g., `No-show` became `no_show`).
6. **Checked and Fixed Data Types**:
   - Ensured that columns like `Age` were of the correct data type (integer), and `ScheduledDay` and `AppointmentDay` were set as `datetime`.

## Dataset Information
- **Number of Records**: 110,527
- **Columns**: 14

## Files:
- `cleaned_appointments.csv`: The cleaned dataset in CSV format.

## Requirements:
- Python 3.x
- pandas

## How to Use:
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/medical-appointment-no-shows.git
   ```
2. Install dependencies:
   ```bash
   pip install pandas
   ```
3. Load and analyze the cleaned dataset in your Python environment:
   ```python
   import pandas as pd
   df = pd.read_csv('cleaned_appointments.csv')
   ```

--
