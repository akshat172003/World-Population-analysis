# World Population Analysis

A comprehensive analysis of global population data using SQL queries in Jupyter Notebook, based on the CIA World Factbook database.

## 📊 Project Overview

This project explores demographic information from the CIA World Factbook, analyzing population statistics across 261 countries worldwide. The analysis focuses on understanding population distributions, growth patterns, and identifying densely populated countries.

## 🗂️ Data Source

The analysis uses data from the **CIA World Factbook**, a comprehensive compendium of statistics about all countries on Earth. The dataset contains demographic information including:

- **Population** - Country population as of 2015
- **Population Growth** - Annual population growth rate (percentage)
- **Area** - Total land and water area
- **Birth Rate** - Number of births per 1,000 people
- **Death Rate** - Number of deaths per 1,000 people
- **Migration Rate** - Net migration rate

## 📁 Project Structure

```
world population analysis/
├── Analysis.ipynb          # Main analysis notebook with SQL queries
├── factbook.db            # SQLite database containing CIA World Factbook data
└── README.md              # This file
```

## 🔍 Analysis Highlights

### Dataset Overview
- **261 countries** analyzed (excluding "World" aggregate)
- **11 columns** of demographic data
- **262 total rows** (including "World" entry)

### Key Findings
1. **Population Extremes**: Identified countries with minimum and maximum populations
2. **Outlier Detection**: Removed "World" aggregate and Antarctica (0 population) for accurate analysis
3. **Densely Populated Countries**: Found countries with above-average population and below-average area
4. **Population Density Analysis**: Bangladesh emerged as the most densely populated country

### Notable Results
- **Most Populous Country**: China (1.4 billion people)
- **Most Densely Populated**: Bangladesh (high population in small area)
- **Other Dense Countries**: Japan and Philippines

## 🛠️ Technical Details

### Technologies Used
- **Jupyter Notebook** - Interactive analysis environment
- **SQL** - Data querying and analysis
- **SQLite** - Database management
- **Python** - Data manipulation and visualization

### Database Schema
The `factbook.db` contains a single table `facts` with the following columns:
- `id` - Unique identifier for each country
- `code` - Two-letter country code
- `name` - Country name
- `area` - Total area (land + water)
- `population` - Population count
- `population_growth` - Annual growth rate
- `birth_rate` - Births per 1,000 people
- `death_rate` - Deaths per 1,000 people
- `migration_rate` - Net migration rate

## 🚀 Getting Started

### Prerequisites
- Python 3.x
- Jupyter Notebook
- SQLite support

### Installation
1. Clone or download this repository
2. Ensure you have Jupyter Notebook installed:
   ```bash
   pip install jupyter
   ```
3. Install SQL extension for Jupyter:
   ```bash
   pip install ipython-sql
   ```

### Running the Analysis
1. Open `Analysis.ipynb` in Jupyter Notebook
2. Run all cells to execute the complete analysis
3. The notebook will automatically connect to the `factbook.db` database

## 📈 Analysis Sections

1. **Database Connection** - Setting up SQL connection to the factbook database
2. **Data Exploration** - Understanding the dataset structure and content
3. **Population Extremes** - Finding minimum and maximum population values
4. **Outlier Detection** - Identifying and handling data outliers
5. **Density Analysis** - Finding densely populated countries
6. **Results Interpretation** - Drawing conclusions from the analysis

## 🎯 Key Insights

This analysis provides valuable insights into:
- Global population distribution patterns
- Countries with exceptional population density
- Data quality considerations in demographic analysis
- Effective SQL techniques for population data analysis

## 📝 Notes

- The dataset represents 2015 population data
- "World" entry (id: 262) represents global totals and is excluded from country-level analysis
- Antarctica is included in the dataset but has 0 population
- All area measurements include both land and water areas

## 🤝 Contributing

Feel free to extend this analysis by:
- Adding new SQL queries for different demographic insights
- Creating visualizations of the results
- Exploring additional demographic factors
- Comparing data across different time periods

## 📄 License

This project is for educational and analytical purposes. The data source (CIA World Factbook) is in the public domain.

---

*This analysis demonstrates the power of SQL for demographic data exploration and provides a foundation for more complex population studies.*
