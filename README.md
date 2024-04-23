# Setting Up dbt and dbt-mysql

## Prerequisites
- Python 3.9 installed on your system.

## Installation Steps

### 1. Create a Python Environment for dbt
```bash
python -m venv dbt-env
```
```bash
source dbt-env/bin/activate         # activate the environment for Mac and Linux OR
```


### 2. Install dbt-mysql Adapter (Includes dbt-core)
```bash
pip install dbt-mysql
```

### 3. Check dbt Version (Optional)
```bash
dbt --version
```
![image](https://github.com/anhnhatcs/dbt-mysql-installation/assets/161874308/79f85543-a0dc-4aaf-a56c-67313a0c94a9)

### 4. Initialize dbt Project
```bash
dbt init dbt
```
Follow the prompts and provide necessary information.
![image](https://github.com/anhnhatcs/dbt-mysql-installation/assets/161874308/8aa930f0-50b5-40f8-9f06-e4af17c7b3f3)

### 5. Debug After Initialization
```bash
dbt debug
```
![image](https://github.com/anhnhatcs/dbt-mysql-installation/assets/161874308/009bd3e7-abe3-49c9-98f6-9f1664ada235)

### 6. Run dbt Project
```bash
dbt run
```
### 7. Ochestration tools (Airflow, Dagster) will be updated by a docker yaml file

## Additional Notes
- Make sure to activate your Python environment (`dbt-env`) before running any dbt commands.
- Ensure that your MySQL database is configured and accessible before running dbt commands.
- Recommendation for dbt orgnization: https://docs.getdbt.com/best-practices/how-we-structure/1-guide-overview
