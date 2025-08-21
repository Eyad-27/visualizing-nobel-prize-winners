# Visualizing the History of Nobel Prize Winners 🏆

Analyze Nobel Prize winner data to uncover historical trends in gender, nationality, decade performance, first female laureates, and repeat winners.  
This project uses pandas for data manipulation and visualization to answer several guiding questions about Nobel Prize history.

---

## ❓ Guiding Questions
1. What is the **most commonly awarded gender and birth country**?  
   - Saved as `top_gender` and `top_country`.  

2. Which **decade had the highest ratio of US-born Nobel Prize winners**?  
   - Saved as `max_decade_usa`.  

3. Which **decade and category combination had the highest proportion of female laureates**?  
   - Saved as a dictionary `max_female_dict`.  

4. Who was the **first woman to receive a Nobel Prize**, and in what category?  
   - Saved as `first_woman_name` and `first_woman_category`.  

5. Which **individuals or organizations have won more than one Nobel Prize**?  
   - Saved as a list `repeat_list`.  

---

## 📊 The Data

### **nobel.csv**
| Column         | Description |
|----------------|-------------|
| `year`         | Year the Nobel Prize was awarded |
| `category`     | Prize category (Physics, Chemistry, etc.) |
| `full_name`    | Full name of the laureate |
| `birth_country`| Birth country of the laureate |
| `sex`          | Gender of the laureate |
| `affiliation`  | Organization or institution associated with the laureate |
| `motivation`   | Reason for the award/prize description |

---

## 🔎 How I Approached the Project  

### 1. Most common gender and birth country  
Filtered and counted `sex` and `birth_country` columns to determine `top_gender` and `top_country`.  

### 2. Decade with highest US-born ratio  
Created a flag for US-born winners, generated decade column, computed ratio per decade, and identified `max_decade_usa`.  

### 3. Decade & category with highest female laureate proportion  
Grouped data by decade and category, calculated female proportions, and extracted `max_female_dict`.  

### 4. First female Nobel Prize winner  
Filtered female laureates, found earliest `year`, and recorded `first_woman_name` and `first_woman_category`.  

### 5. Repeat winners  
Counted occurrences of each winner in the dataset, and saved names with two or more prizes in `repeat_list`.  

---

## 📌 Key Deliverables
- Filtered winners by gender and birth country using pandas DataFrames and Boolean logic.  
- Calculated decade-level ratios of US-born winners.  
- Identified decade-category combinations with highest female laureates.  
- Extracted first female Nobel Prize winner and her category.  
- Generated a list of individuals/organizations with multiple Nobel Prizes.  

---

## 🛠️ Skills Used
- **Python**: pandas, numpy  
- Data wrangling & filtering  
- Grouping, aggregation, and ratios  
- Dictionary & list manipulations  
- Relational line plots & multi-category visualizations  
