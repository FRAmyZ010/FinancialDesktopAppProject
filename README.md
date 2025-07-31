July 30, 2025

# Personal Finance Management App

A desktop application for managing your income, expenses, and financial goals.  
Built using [Electron.js](https://www.electronjs.org/), HTML, CSS, and JavaScript.

---

## 🔍 Concept

The core idea behind this project is to create a personal finance management and tracking tool — all in one place.  
It also aims to support recording investment activities, promote financial discipline, and encourage consistent tracking habits.

Additionally, this is my very first solo project.  
If there are any mistakes or oversights, I sincerely apologize and genuinely welcome all feedback and suggestions for improvement.

> ⚠️ **Please note:**  
> This is only an initial idea, and **many changes may occur** in future development.


## 🎯 Features

- Record income and expenses
- Choose where to store money (e.g., cash, SCB, KTB)
- Create financial goals (e.g., saving for a product)
- Visual reports and charts
- Export data as CSV/Excel
- Offline support — all data is stored locally

---

## 📁 Data Model Overview

### `transaction` table

| Field       | Type     | Description                   |
|-------------|----------|-------------------------------|
| `id`        | int   | Unique transaction ID         |
| `type`      | string   | `"income"` or `"expense"`     |
| `amount`    | number   | Amount of money               |
| `account_id`  | string   | Category (e.g., food, travel) |
| `user_id`      | string   | Optional notes                |
| `date`      | string   | Date of transaction           |

---

### `User` table

| Field            | Type     | Description                    |
|------------------|----------|--------------------------------|
| `user_id`             | int   | Unique user ID              |
| `user_name`           | string   | Name     |
| `balance`           | int   | |


---

### `account` table

| Field       | Type     | Description                        |
|-------------|----------|------------------------------------|
| `account_id`        | int   |        |
| `user_id`      | int   |                    |
| `balance`| int   |          |
| `account_name`  | string   |                   |

---
<img width="901" height="607" alt="image" src="https://github.com/user-attachments/assets/b0bf6fe7-a696-4bf9-89c3-5175733b83a9" />
---


## 📦 Technologies Used

- [Electron.js](https://www.electronjs.org/)
- [Express.js](https://expressjs.com/)
- HTML, CSS, JavaScript
- [Chart.js](https://www.chartjs.org/) – For visual reports
- [xlsx](https://www.npmjs.com/package/xlsx) – For Excel export
- [LowDB](https://www.npmjs.com/package/lowdb) or local JSON for data storage
- [SQLite](https://www.sqlite.org/)

---

## 🚀 Getting Started

1. Clone this repository:
   ```bash
   git clone https://github.com/FRAmyZ010/FinancialDesktopAppProject.git
