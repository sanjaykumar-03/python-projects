# 💰 Expense Splitter (Splitwise Clone)

A simple Python project to split expenses among friends and calculate who owes whom — just like Splitwise.

---

## 📌 Features

* Add shared expenses among multiple people
* Automatically split amounts equally
* Calculate final balances
* Show who should pay and who should receive
* Optimize settlements (minimum transactions)

---

## 🧠 How It Works

This project uses a **matrix-based approach**:

* Each row = person who paid
* Each column = person who benefited
* Calculates:

  * Total paid
  * Total owed
  * Final balance

---

## 🛠️ Tech Stack

* Python 🐍
* NumPy (for matrix calculations)
---
## 📂 Project Structure

```
expense_splitter.ipynb   # Main Jupyter Notebook
README.md                # Project documentation
```
---
## ▶️ Usage

1. Open the Jupyter Notebook:

```
jupyter notebook
```

2. Run all cells

3. Modify this section to add expenses:

```python
add_expense("Alice", ["Alice","Bob","Carol","Danial"], 600)
add_expense("Bob", ["Bob","Carol","Danial"], 200)
add_expense("Carol", ["Alice","Bob","Carol","Danial"], 400)
add_expense("Danial", ["Bob","Carol","Danial"], 200)
```

---

## 📊 Example Output

```
Final Balances:
Alice will receive ₹350.00
Bob should pay ₹183.33
Carol will receive ₹16.67
Danial should pay ₹183.33

Settlement:
Bob pays ₹183.33 to Alice
Danial pays ₹166.67 to Alice
Danial pays ₹16.67 to Carol
```
## 📖 Key Concepts

* **Expense Matrix**: Tracks who paid for whom
* 
* **Balance Calculation**:
  balance = total_paid - total_owed
  
* **Settlement Algorithm**: Matches debtors with creditors
## 🚀 Future Improvements

* Add GUI (Tkinter / Web app)
* Store data in database
* Support unequal splits
* Add user input system
  
## 🤝 Contributing
Feel free to fork this repo and improve the project!

## 📜 License
This project is open-source and free to use.

## 👨‍💻 Author
Sanjay Kumar
