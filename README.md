# Uber Pickup Data Analysis - August 2014

## Project Overview
Analysis of 1.5 million Uber pickups from August 2014 in New York City, revealing key patterns in ridership behavior and operational insights.

## 🔍 Key Findings

### ⏰ Temporal Patterns
- **Peak pickup time**: 18:30 (90 pickups in 15-min interval)
- **Lowest activity**: 03:15 AM
- **Busiest day**: August 7, 2014 (32,759 pickups)
- **Weekly pattern**: 
  - Thursday = Highest ridership 
  - Sunday = Lowest ridership

### 🚗 Service Analysis
- **Top performing base model**: B02617
- **All base models**:
  | Code      | Service Name   |
  |-----------|----------------|
  | B02598    | Hinta          |
  | B02682    | American       |
  | B02684    | Danish-NV      |
  | B02665    | Green          |
  | B02635    | Quick          |
  | B02636    | Driven         |

## 📊 Visualizations
1. **Time-based patterns**:
   - Heat maps of pickup density
   - Daily line graphs (15-min intervals)
  
2. **Geographical distribution**:
   - Scatter plot of pickups by location
  
3. **Service comparison**:
   - Bar chart of rides by base model
   - Pie chart of weekly distribution
  
# Analyze peak periods
peak_hour = df.groupby(df['Date/Time'].dt.hour).size().idxmax()

# Insights Summary
Daily pattern: Evening commute (17:00-18:30) = Critical demand period
Weekly pattern: 22% higher ridership on Thursdays vs Sundays
Top performer: Base B02617 handles 31% of total rides

**Operational recommendation**: Boost supply during 16:00-19:00 on weekdays

