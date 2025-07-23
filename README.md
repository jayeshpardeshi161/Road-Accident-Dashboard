# 🚧 Road Accident Dashboard

# 🗂️ Project Summary
This project is a Tableau-based interactive dashboard developed to analyze and monitor road accident data in the UK. The dashboard allows for comprehensive drill-downs across accident severity, vehicle types, weather, road conditions, and geographical location with YoY comparisons and filtering capabilities.

--

# 🎯 Project Goals
Identify key trends and patterns in road accidents.

Analyze casualty severity over time (Fatal, Serious, Slight).

Enable dynamic filtering by severity, year, and location.

Visualize accidents by vehicle type, road condition, weather, and more.

Generate actionable insights to support road safety improvements.

--

# 🧾 Dataset Overview

File: Road Accident Data.csv

Rows: 66,079

Columns: 14

**Primary Fields:**

Accident Date

Accident Severity

Number of Casualties

Vehicle Type

Weather Conditions

Road Surface Conditions

Road Type

Latitude, Longitude

etc.

--

## ❓ Problem Statement

Accident data often exists in raw, fragmented formats, making it difficult to extract insights quickly. This project solves that by creating an interactive, visual interface to:

Track changes in accident trends over time.

Examine the role of weather, road, and vehicle factors.

Support public policy and road safety strategy.

--

## 📊 KPIs (Key Performance Indicators)

**KPI	Description**

Total Accidents	Count of all accident records.
Total Casualties	Sum of all casualties reported.
Fatal Casualties	Number of people killed.
Serious Casualties	Number of people seriously injured.
Slight Casualties	Number of people slightly injured.
Casualties by Vehicle Type	Breakdown of casualties by grouped vehicle types.

--

## 🧮 Calculations & Measures

Year-over-Year (YoY) Metrics:

Current Year Accidents
Previous Year Accidents
YoY Accident Change

Current Year Casualties
Previous Year Casualties
YoY Casualty Change
Severity-based YoY Calculations:


CY Fatal Casualties
PY Fatal Casualties
YoY Fatal Casualties

CY Serious Casualties
PY Serious Casualties
YoY Serious Casualties

CY Slight Casualties
PY Slight Casualties
YoY Slight Casualties

**Grouped Measures:**

Vehicle Type Group: Motorcycle, Bus, Car, Van, Others

Weather Group: Fine, Rain, Snow/Fog, Others

Road Surface Group: Wet, Frost/Snow, Unknown

--

## 🧪 EDA (Exploratory Data Analysis) Steps

Null/NA value handling.

Outlier detection in latitude/longitude.

Convert Accident Date to datetime.

Derive Year, Month from date.

Group and summarize categories:

Vehicle Type

Weather

Road Surface

Road Type

--

## 📈 Visualizations in Tableau
Visualization	Description
KPI Cards	Real-time numbers for accidents/casualties.
Pie Chart	Casualties by Weather & Road Surface
Bar Chart	Casualties by Road Type
Map	Geo-plot of casualties by location
Horizontal Bar	Casualties by grouped Vehicle Type
Parameter Controls	Filters for Year, Severity
Dynamic Titles	Change based on selected filters

--

## 🔑 Key Findings
Majority of accidents occur under fine weather but also involve serious casualties during rainy/snowy conditions.

Cars and Motorcycles account for the largest share of casualties.

Urban roads have higher accident frequency, while rural roads show higher severity (fatal/serious).

YoY comparisons reveal a decrease/increase in certain accident types depending on the year (requires dynamic parameter input).

--

## 💼 Business Impact

Helps transport departments and policy-makers understand risk factors.

Supports urban planning with hotspot detection.

Enables insurance providers to assess location-based risks.

Encourages public awareness via open dashboards or government data portals.

--

## 🔍 Insights & Inference

Environmental factors (weather & road surface) significantly influence accident severity.

Real-time, parameterized dashboards provide data democratization.

Severity-based filtering helps targeted interventions.

--

## ✅ Conclusion

The Road Accident Dashboard is a powerful tool for analyzing historical accident trends and drawing attention to key risk areas. With dynamic filters, grouped categories, and YoY comparisons, it can serve multiple stakeholders from analysts to policymakers in building safer roads.

--

## 📷 Images

<img width="1138" height="637" alt="Road Accident Dashboard" src="https://github.com/user-attachments/assets/2530140b-c3ce-45ec-a6f9-5703a1743419" />

--

## ✅ Review Steps :

### ✅ KPI Section (Top Left 3 Cards + 3 Below)

| KPI                    | Requirement                                | Review                                               |
| ---------------------- | ------------------------------------------ | ---------------------------------------------------- |
| **Total Accidents**    | Count of accidents by year with YoY change | ✔️ Present and correctly calculated                  |
| **Total Casualties**   | Sum by year with YoY change                | ✔️ Present, aligned with formula                     |
| **Fatal Casualties**   | Filtered by severity + YoY                 | ✔️ Correct; reflects 26.4% YoY drop                  |
| **Serious Casualties** | Filtered by severity + YoY                 | ✔️ Matches 16.3% YoY drop                            |
| **Slight Casualties**  | Filtered by severity + YoY                 | ✔️ Correct; -10.82% drop                             |
| **Vehicle Type KPI**   | Top 6 vehicle groups + YoY change          | ✔️ Grouped and YoY metrics shown clearly for 6 types |

--

### ✅ Vehicle Type KPI Section

Requirement: Group 16 vehicle types into 6 (Motorcycle, Bus, Car, Van, Others).

Dashboard View: Pie or bar chart with images + YoY and CY values.

Dynamic Title: "All Casualties by Vehicle Type" (dynamic title used ✔️)

✔️ Fully implemented and accurate based on your description.


### ✅ Pie Charts

***1. Casualties by Weather Condition***
| Requirement                               | Review                   |
| ----------------------------------------- | ------------------------ |
| Grouped into Fine, Rain, Snow/Fog, Others | ✔️ Done                  |
| Dynamic Title with Severity Parameter     | ✔️ Dynamic title visible |
| Total 195.7K matches total casualties     | ✔️ Yes                   |

***2. Casualties by Road Surface***
| Requirement                                | Review              |
| ------------------------------------------ | ------------------- |
| Grouped into Dry, Wet, Frost/Snow, Unknown | ✔️ Correct grouping |
| Dynamic Title                              | ✔️ Present          |
| 195.7K total used again                    | ✔️ Matched ✔️       |

### ✅ Map – Casualties by Location
| Requirement                        | Review                                               |
| ---------------------------------- | ---------------------------------------------------- |
| Dots plotted by accident locations | ✔️ Map is responsive and detailed                    |
| Dynamic Title based on severity    | ✔️ "All Casualties by Location" (severity-driven ✔️) |

### ✅ Bar Chart – Casualties by Road Type
| Requirement                                                                       | Review                                              |
| --------------------------------------------------------------------------------- | --------------------------------------------------- |
| Road types such as: Single/dual carriageway, roundabout, one way, slip road, etc. | ✔️ 7 types shown with correct totals                |
| Dynamic Title using severity param                                                | ✔️ Present: "<severity> Casualties by Road Type" ✔️ |

### ✅ Parameters
| Parameter                 | Used?                                             | Review |
| ------------------------- | ------------------------------------------------- | ------ |
| Current Year              | ✔️ Yes                                            |        |
| Previous Year             | ✔️ Yes                                            |        |
| Select Accident Severity  | ✔️ Fully applied across dashboard elements        |        |
| Dynamic Filtering Applied | ✔️ Everywhere, including title updates and charts |        |

### ✅ Calculated Fields 
Each calculation provided is reflected correctly in the dashboard:

--

## 🔗 License

MIT License © 2025 [Jayesh Pardeshi]

--

## 🔗 Author

📧 Gmail	:[jayeshpardeshi161@gmail.com]  
📌 LinkedIn:[]
