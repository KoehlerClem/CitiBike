# CitiBike Data Analysis

This repository analyzes NYC Citi Bike trip data, focusing on **trip duration, distance distribution, and visualization**.  
It uses **PySpark** for efficient data processing and **Matplotlib/Folium** for visualization.

---

## Data Download

Download Citi Bike trip data from:  
🔗 **[Citi Bike System Data](https://citibikenyc.com/system-data)**  

**Files to Download:**  
- [JC-202501-citibike-tripdata.csv.zip](https://s3.amazonaws.com/tripdata/JC-202501-citibike-tripdata.csv.zip)  
- [202501-citibike-tripdata.zip](https://s3.amazonaws.com/tripdata/202501-citibike-tripdata.zip)  

**Place the extracted CSV files into the correct folder** (`202501-citibike-tripdata/`).

---

## Setup (MacOS)

### Install Dependencies  
#### **Mac (Homebrew)**
```sh
brew install openjdk@11
echo 'export PATH="/opt/homebrew/opt/openjdk@11/bin:$PATH"' >> ~/.zshrc
brew install apache-spark
```

#### **Python Environment (Python 3.11)**
```sh
python -m venv venv
source venv/bin/activate  # Mac/Linux
pip install -r requirements.txt
```

### Start Jupyter Notebook
```sh
jupyter notebook
```

---

## Running the Analysis

- Open the **Jupyter Notebook** and execute the cells.
- The notebook will:
  - Load and clean the data.
  - Aggregate trip distances.
  - Generate **interactive maps** and **bar charts** for visualization.

---

## Exporting Notebook to HTML

To **export the executed notebook** as an HTML report:
```sh
jupyter nbconvert --execute analysis.ipynb --to html
```
This will generate a `analysis.html` file containing all **visualizations and results**.

