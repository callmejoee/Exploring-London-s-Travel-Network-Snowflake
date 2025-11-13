# 🚇 Exploring London’s Public Transport Journeys with Snowflake

## 🏙️ Introduction

**London**, or as the Romans called it, **“Londinium,”** is home to over **8.5 million residents** who collectively speak **more than 300 languages**.  
While the historic **City of London** spans just over a single square mile (earning it the nickname *“The Square Mile”*), **Greater London** now consists of **32 boroughs** covering more than **600 square miles**.

![Tower Bridge](london.jpg)

---

## 🚉 A Growing City Needs a Modern Transport Network

![Underground train](tube.jpg)

London’s roads were originally designed for *horse and cart*. With massive population and geographic expansion, the city needed a transport system capable of handling millions of daily journeys.

Since **2000**, this responsibility has been overseen by **Transport for London (TfL)** — the mayoral body that manages:

- London Underground  
- Overground  
- DLR (Docklands Light Railway)  
- Buses  
- Trams  
- River services  
- TfL Rail  
- Emirates Airline cable car  
- Major roads  
- Taxis  

TfL makes much of its data publicly available. For this project, we work with a simplified version of their **journey volume dataset**, hosted in a **Snowflake** database.

---

## ❄️ Snowflake Dataset Overview

The data is stored in the `TFL` database, inside a single table called **`JOURNEYS`**.

### **📄 TFL.JOURNEYS**

| Column | Description | Data Type |
|--------|-------------|-----------|
| `MONTH` | Month number (e.g., 1 = January) | INTEGER |
| `YEAR` | Year | INTEGER |
| `DAYS` | Number of days in the month | INTEGER |
| `REPORT_DATE` | Reporting date | DATE |
| `JOURNEY_TYPE` | Transport mode (e.g., Bus, Underground & DLR) | VARCHAR |
| `JOURNEYS_MILLIONS` | Millions of journeys | FLOAT |

*Note: In Snowflake, databases, schemas, tables, and columns appear in **UPPERCASE** by default.*

---

## 🎯 Project Goals

You will use **Snowflake SQL** to answer the following:

1. **Which transport types are the most popular?**  
2. **How popular was the Emirates Airline cable car, and in which months?**  
3. **What are the least popular years for the Underground & DLR?**

---
