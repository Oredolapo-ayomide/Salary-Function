## Module 2 Assignment: Salary Function

### Assignment Overview

This project was developed for the **BAN 6420 - Module 2** assignment. It demonstrates data handling, error handling, file operations in Python, and basic data processing using R. The assignment performs the following tasks:

1. Import and process employee salary data.
2. Search for an employee and retrieve their details.
3. Export the employee’s data to CSV and compress into a ZIP folder.
4. Use an **R script** to unzip and display the data.

---

### Folder Structure

After unzipping the main folder (`Module 2 Assignment`), the structure should look like this:

```
Module 2 Assignment/
│
├── salary_data.csv
├── salary_function.ipynb
├── view_employee_profile.R
├── README.md
└── Employee_Profile/
    └── Nathaniel_Ford_Profile.csv (example)
```

---

### Python File: `salary_function.ipynb`

This Jupyter Notebook performs the following:

* Loads salary data from `salary_data.csv`
* Defines `get_employee_details(name)` function
* Stores employee data in a Python dictionary
* Handles input errors
* Exports matched employee details to CSV
* Zips the CSV file into a folder called `Employee_Profile.zip`

> **NOTE**: This zipped folder is automatically created when you run the notebook and search for a valid employee.

---

### R Script: `view_employee_profile.R`

This script performs the following:

1. Sets working directory (manually or by default).
2. Unzips the file `Employee_Profile.zip` into a folder.
3. Searches for `.csv` files inside the folder.
4. Loads and prints the employee details in the R console.

---

###  Important Notes

* **You must unzip** the entire `Module 2 Assignment.zip` folder before running the R script.
* Do **not** run the `.R` script directly from within the zipped folder. The script will not be able to access files.
* If testing the `.R` file manually:

  * Unzip to a known location like `Desktop`.
  * Open RStudio 
  * Set the working directory using `setwd()` if needed.
  * Run the script.

---

### How to Run

#### Run the Python Notebook

1. Open `salary_function.ipynb` in Jupyter Notebook.
2. Run all cells.
3. Use `get_employee_details("Employee Name")` to retrieve info.
4. The result is saved as a `.csv` file and zipped in `Employee_Profile.zip`.

#### Run the R Script

1. Ensure `Employee_Profile.zip` exists in the same folder.
2. Unzip the `Module 2 Assignment.zip` folder.
3. Open `view_employee_profile.R` in RStudio.
4. Click **Run**
5. The employee CSV data will be displayed in the R console.

---
