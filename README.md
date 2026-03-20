## Game monetization analysis (SQL)

### Overview
This project analyzes player behavior and in-game purchases in an online RPG. The focus is on understanding monetization patterns, payer behavior, and the impact of player characteristics (such as race) on revenue generation.

All analysis was performed using SQL.

---

### Objectives
- Calculate payer share across all users
- Analyze payer behavior by player race
- Explore in-game purchase patterns and transaction distribution
- Identify anomalies in purchase data
- Evaluate popularity of in-game items
- Analyze purchasing activity across player segments

---

### Dataset
- **users** — player attributes (race, class, etc.)
- **events** — in-game purchases using premium currency

---

### Tools
- SQL (data extraction, aggregation, analysis)

---

### Key results

####  Payer share
- Overall payer share: **17.68%** (3,929 out of 22,214 users)
- Highest payer share: **Demon (19.36%)**, **Hobbit (18.04%)**
- Lowest payer share: **Elf (17.07%)**, **Angel (17.26%)**

---

####  Purchases
- Total purchases: **1,307,678**
- Total revenue: **686,615,040**
- Avg purchase: **525.69**, Median: **74.86**
- High variance indicates presence of large transactions

---

####  Anomalies
- **907 zero-value purchases** (0.07%)
- All related to *Book of Legends*

---

#### User behavior
- Purchasing users: **13,793**
- Non-payers are more active (more transactions per user)
- Payers generate higher total revenue per user
- **Northman payers spend significantly more per purchase**

---

####  Item popularity
- *Book of Legends* — **76.87% of all purchases**
- *Bag of Holding* — **20.81%**
- **38 items were never purchased**

---

### Ad hoc analysis (player activity by race)

- Most active races: **Orc**, **Northman**
- Lowest payer share among buyers: **Elf**, **Angel**
- **Demon**: fewer purchases but highest payer share
- **Northman & Elf**: highest average spend and total spend per user

---

### Business insights

- Strong monetization potential in **Demon** and **Hobbit** segments  
- **Northman players** show high spending behavior → opportunity for targeted monetization  
- **Elf players**: low payer share but high spend → possible imbalance in game economy  
- Large share of revenue concentrated in **one item (Book of Legends)**  
- Presence of unused items and zero-value transactions indicates optimization opportunities  

---
