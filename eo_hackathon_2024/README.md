# Climate-Informed Risk Modeling for Sustainable Agriculture

## Introduction
Welcome to the Agricultural Climate Risk Modeling Hackathon! This challenge focuses on leveraging AI/ML techniques to develop sustainable agricultural solutions through climate risk modeling. We aim to help farmers and agricultural stakeholders make informed decisions by predicting and categorizing climate-related risks at the taluk (sub-district) level.

Quick overview of Rabi and Kharif seasons

- **Kharif Season (June-November)**:
  - Main cropping season during the south-west monsoon
  - Early sowing period (June-July) typically shows less vegetation coverage
  - Crops include rice, maize, sorghum, pearl millet, and cotton

- **Rabi Season (December-April)**:
  - Winter cropping season
  - Relies on residual moisture in soil and winter rainfall
  - Major crops include wheat, barley, peas, and mustard

## Problem Statement
The challenge is to develop a predictive model that:
1. Forecasts climatic parameters(mentioned in Dataset Description Section) at the taluk level using historical data
2. Assigns risk categories for each parameter
3. Create an overall risk assessment for each taluk at month level for Kharif 2024 (August, September, October, November)


### Risk Categories
Participants need to come up with appropriate ranges for these risk levels:
- Individual Parameters: Low, Medium, High, Very High
- Overall Taluk Risk: Low, Medium, High

## Dataset Description
All the following parameters are captured from 2019 to 2024 May.

### 1. Rainfall Data
 Rainfall is the amount of precipitation that falls in a specific area, directly affecting soil moisture, crop growth, and overall water availability for agriculture. We will consider average rainfall in mm at each day, Taluk level.

| region_id      | year | month | day | daily_sum |
|----------------|------|-------|-----|-------------|
| 91020002001000 | 2019 | 1     | 1   | 0.0        |
| 91020002002000 | 2019 | 1     | 1   | 0.0        |
| 91020002003000 | 2019 | 1     | 1   | 0.0        |

**Features**:
- `region_id`: Unique identifier for taluk
- `daily_sum`: Average rainfall in mm for each day at Taluk level

### 2. Land Surface Temperature (LST)
is the temperature in degree Celsius of the Earth's surface as measured from satellites. It indicates how hot or cold the land is at a given time and is important for understanding weather, climate, and environmental conditions. LST helps in monitoring changes in vegetation, water availability, and heat patterns in urban areas. For this parameter data availabilty starts from 2019 May.


| region_id      | year | month | day | daily_avg |
|----------------|------|-------|-----|-----------|
| 91020002001000 | 2019 | 5     | 1   | 31.747370 |
| 91020002002000 | 2019 | 5     | 1   | 31.424524 |
| 91020002003000 | 2019 | 5     | 1   | 31.748835 |

**Features**:
- `daily_avg`: Average temperature in degrees Celsius

### 3. Evapotranspiration (EVT)
Evapotranspiration is the total amount of water transferred from the land to the atmosphere through evaporation from the soil and transpiration from plants. It is a key indicator of water loss and crop water demand.

| region_id      | year | month | day | 8_day_sum |
|----------------|------|-------|-----|-----------|
| 91020002001000 | 2019 | 1     | 1   | 3.330133 |
| 91020002002000 | 2019 | 1     | 1   | 3.657354 |
| 91020002003000 | 2019 | 1     | 1   | 3.570744 |

**Features**:
- `8_day_sum`: Total evapotranspiration over 8-day periods

### 4. Groundwater
Groundwater, as measured by the GRACE (Gravity Recovery and Climate Experiment) satellites, refers to underground water stored in aquifers, detected through changes in the Earth's gravity field, providing insights into groundwater depletion and replenishment over

| region_id      | year | month | day | daily_avg |
|----------------|------|-------|-----|-----------|
| 91020002001000 | 2019 | 1     | 1   | 73.918510|
| 91020002002000 | 2019 | 1     | 1   | 78.260941|
| 91020002003000 | 2019 | 1     | 1   | 76.963333|

**Features**:
- `daily_avg`: Average daily groundwater level

## Data Access

### Download Instructions
1. All individual datasets are available in CSV format
2. Sample notebook for data loading can be accessed here: [download_data.ipynb](./download_data.ipynb)

### Data Resolution
All satellite data has been aggregated to Tehsil/subdistrict level for consistency and ease of analysis.

## Getting Started
1. Clone this repository
2. Review the starter notebook for data loading examples
3. Explore the datasets and develop your risk categorization methodology
4. Build your predictive model for Kharif 2024

For any questions or clarifications, please open an issue in the repository.

Good luck!