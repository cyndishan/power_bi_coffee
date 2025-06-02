# ☕ Coffee Shop Sales Report — Power BI Project

Welcome to my Power BI showcase project: **Coffee Shop Sales Dashboard**. This report provides a detailed analysis of sales patterns across different time periods and product categories, helping business stakeholders understand customer behavior and make data-driven decisions.

---

## 📊 Report Overview

This interactive Power BI report includes the following visualizations:

1. **Line Chart** — Tracks sales trends for Morning, Afternoon, Evening, and Snacks throughout the week.
2. **Pie Chart** — Displays the proportion of total sales contributed by each category.
3. **Line & Clustered Column Chart** — Shows distribution of Morning, Afternoon, and Evening sales with a line chart for Snack sales trend.
4. **Bar Chart** — Highlights the number of customers per weekday.

---

### 🔎 Slicers
- **Promotion Active:** Yes / No  
- **Day of the Week**

---

## 💬 Q&A Feature — Interactive Dialogue

This report includes the Power BI **Q&A visual**, allowing users to type natural language questions and receive instant visual responses based on the data.

### 📥 Suggested Questions You Can Ask:

- **"average snacks sale"**
- **"total morning sale"**
- **"compare snacks sale and customer"**
- **"total customer"**

This interactive element empowers users to explore insights without navigating filters or visuals directly.

---

## ✅ Problem Solved: Incorrect Weekday Order

Power BI by default sorts weekday names alphabetically (e.g., Friday before Monday), which can distort trends in line charts.

To solve this, I created a **separate Weekday Table** with a `DaySort` column. I then sorted weekday names (e.g., "Monday", "Tuesday") by this numeric column to ensure charts display the **correct calendar order** from Monday to Sunday.

```DAX
WeekdayTable = DATATABLE(
    "Day", STRING,
    "DaySort", INTEGER,
    {
        {"Monday", 1},
        {"Tuesday", 2},
        {"Wednesday", 3},
        {"Thursday", 4},
        {"Friday", 5},
        {"Saturday", 6},
        {"Sunday", 7}
    }
)
```

---

## 🖼️ Report Screenshot

Here’s a preview of the full Power BI report:

![image](https://github.com/user-attachments/assets/28ed61ce-066d-47cd-8465-ce4c63350233)


---

## 📈 Key Insights

1. **Afternoon consistently drives the highest sales** across all days, followed by Evening, then Morning, and Snacks.  
   - Notably, **Thursday and Friday Morning sales are equal to Snack sales**, indicating a potential for improvement.
2. **Sales breakdown by category:**
   - Afternoon: **38.75%**
   - Evening: **24.92%**
   - Morning: **19.60%**
   - Snacks: **16.72%**
3. **Trend analysis:**
   - Morning and Evening sales rise steadily from **Monday to Saturday**, with a drop on **Sunday**.
   - Afternoon and Snack sales rise overall, but drop on **Wednesday** and again on **Sunday**.
4. **Customer count by day:**
   - **Monday** has the **fewest customers and lowest sales**.
   - **Saturday** sees the **highest traffic and revenue**.
5. **Customer trend:**
   - Upward trend from **Monday to Saturday**.
   - Drops **midweek (Tuesday to Wednesday)** and sharply from **Saturday (300 customers) to Sunday (250)**.

---

## 💡 Actionable Recommendations

- **Boost Afternoon Engagement:** Build on peak performance with combo deals, loyalty points, or limited-time promotions.
- **Improve Sunday Sales:** Introduce themed events or "Sunday Specials" to mitigate weekend fatigue and increase footfall.
- **Reinvigorate Mondays:** Launch motivational discounts or loyalty boosters to attract customers on the slowest day.
- **Midweek Snack Promotion:** Test snack bundle deals or midweek flash discounts to increase engagement on Wednesdays.
- **Investigate Weekend Drop-Off:** Analyze internal or external factors contributing to Sunday’s performance drop and take corrective action.

---

## 🛠 Tools Used

- **Power BI Desktop**
- **Power Query Editor**
- **DAX (Data Analysis Expressions)**
- **CSV file as data source**
- **Q&A Visual** for natural language exploration

---

## 📂 Files

- `Coffee Shop Sales Report.pbix` — Main Power BI dashboard file
- `data/CoffeeShop.csv` — Source dataset 

---

## 📌 About This Project

This project was created as part of my data analytics portfolio to demonstrate:

- Data modeling and cleaning in Power BI
- Time-based sorting using custom weekday tables
- Effective use of slicers and Q&A natural language visuals
- Extracting actionable business insights from sales data
- Professional data storytelling for non-technical stakeholders

---

## 🔗 Contact

**Cyndi Li Shan** — Aspiring Data Analyst  
📧 Email: [cyndi.shan0101@gmail.com]  
🌐 Portfolio: [[github]](https://github.com/cyndishan)
💼 LinkedIn: [[LinkedIn]](https://www.linkedin.com/in/cyndi-li-shan/)
