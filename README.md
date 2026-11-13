# Supermarket Checkout System

A clean, interactive command-line billing application built in Python. This program simulates a standard retail checkout counter: you enter the items a customer is purchasing along with their quantities and prices, and the system automatically calculates subtotals, applies tiered purchase discounts, and outputs a neatly aligned, professional receipt.

I put this project together while practicing core Python programming concepts—focusing heavily on writing clean control flows, handling invalid user inputs gracefully, and structuring terminal output into an authentic retail format.

---

## Overview

In many introductory programming projects, data is hardcoded or error handling is ignored. The **Supermarket Checkout System** approaches things a bit more practically. It guides the cashier through a live transaction session step-by-step, validating every entry in real time to prevent crashes caused by typos, negative numbers, or empty strings.

Once all products are added, the application evaluates the total, computes the appropriate discount percentage, and prints a structured itemized receipt directly to the console.

---

## Key Features

* **Multi-Item Transactions:** Seamlessly record multiple distinct products within a single customer checkout session.
* **Robust Input Validation:** Rejects empty product names, non-numeric values, zeros, and negative numbers using `try / except` blocks and loops, prompting the user cleanly until valid data is provided.
* **Automated Calculations:** Instantly computes individual line totals (`price × quantity`), aggregates an overall pre-discount subtotal, and computes the exact discount amount.
* **Tiered Discount Engine:** Automatically assigns discount thresholds based on the scale of the customer's purchase without requiring manual operator math.
* **Structured Terminal Receipt:** Uses Python string formatting and alignment methods to produce a clean, classic receipt layout that looks right at home on a terminal screen.

---

## Discount Policy

Discounts are calculated dynamically based on the total purchase amount before deductions:

| Purchase Amount | Discount Applied |
| --- | --- |
| **Rs. 10,000 and above** | 10% |
| **Rs. 5,000 – Rs. 9,999** | 5% |
| **Below Rs. 5,000** | No discount |

---

## Sample Output

```text
========================================
       SUPERMARKET CHECKOUT SYSTEM
========================================

How many products? 2

Product 1
Name: Rice
Price: 1500
Quantity: 4

Product 2
Name: Cooking Oil
Price: 900
Quantity: 3

========================================
           SUPERMARKET BILL
========================================
Rice           4 x 1500   =    6000
Cooking Oil    3 x 900    =    2700
----------------------------------------
Subtotal                       Rs. 8700
Discount (5%)                  Rs. 435
========================================
FINAL BILL                     Rs. 8265
========================================
       THANK YOU FOR SHOPPING WITH US!
             PLEASE VISIT AGAIN
========================================

```

---

## Project Structure

```text
Supermarket-Checkout-System/
│
├── supermarket_checkout.py   # Core application logic and interface
├── README.md                 # Project documentation
└── .gitignore                # Standard Git ignore rules

```

---

## Getting Started & Installation

### Prerequisites

* **Python 3.x** installed on your system.
* A terminal environment or a lightweight code editor like **Visual Studio Code**.

### Step-by-Step Instructions

1. **Clone the repository:**
```bash
git clone https://github.com/Rammal-Ahmed/Supermarket-Checkout-System.git

```


2. **Navigate into the project directory:**
```bash
cd Supermarket-Checkout-System

```


3. **Run the application:**
```bash
python supermarket_checkout.py

```


4. Follow the interactive console prompts to enter the number of products, item names, unit prices, and quantities to view your generated receipt.

---

## Python Concepts & Practices Applied

This project serves as a hands-on sandbox for foundational programming techniques:

* **Data Collections:** Storing parallel records and item details cleanly using Python lists and loops.
* **Control Flow:** Managing execution paths using `for` and `while` loops for item iteration and validation re-prompts.
* **Conditional Logic:** Implementing `if / elif / else` structures for tiered discount evaluations.
* **Defensive Programming:** Using `try / except` exception handling to catch bad user inputs before they break the script.
* **Code Organization:** Structuring logic into modular blocks with clean, readable naming conventions.
* **Output Formatting:** Leveraging Python f-strings and padding techniques to align receipt columns neatly.

---

## Future Improvements

While the application is fully complete and functional for basic console billing, potential extensions on the roadmap include:

* **Decimal Pricing Support:** Enabling floating-point numbers to support fractional prices (e.g., `150.75`).
* **Receipt Archiving:** Automatically writing completed transaction receipts out to timestamped `.txt` files for record-keeping.
* **Product Lookup Catalog:** Integrating a pre-populated item dictionary or CSV file so cashiers can search product codes instead of typing names and prices manually.
* **Cart Management:** Adding options to review, modify quantities, or remove specific line items before finalizing the bill.

---

## About me

**Rammal Ahmed**

**AI & Data Science Enthusiast** | **Microsoft Dynamics 365 CRM Developer** | **Power Platform** | **UI/UX Designer** | **Graphic Designer & Illustrator**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/rammal-ahmed-58184b325)
[![GitHub](https://img.shields.io/badge/GitHub-Rammal--Ahmed-181717?style=flat&logo=github)](https://github.com/Rammal-Ahmed)

<div align="center">

⭐ If you found this useful, consider giving it a star ⭐

**I truly value your feedback and welcome any suggestions for improvement**

**Always open to fresh perspectives, constructive feedback, and new ideas**


## License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

**Project Status:** Completed

</div>
