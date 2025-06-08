# 🚫 Automating IP Allow List Removal

This project simulates a task performed by a security analyst at a healthcare company. The goal is to create a Python algorithm that updates a file (an allow list) by removing unauthorized IP addresses that should no longer have access to restricted information such as patient medical records or PII.

---

## 🧠 Project Scenario

As a security analyst, I was responsible for maintaining an allow list that controlled access to a restricted subnetwork. Employees were given access based on IP addresses stored in a text file. My task was to automate the process of identifying and removing IPs that should no longer have access.

---

## ⚙️ Technical Approach

### 1. Open the Allow List File
- Assigned the variable `import_file` to point to `allow_list.txt`
- Used the `with open(import_file, "r") as file:` structure to safely read the file

### 2. Read and Analyze the File
- Used `.read()` to store contents in a variable `ip_addresses`
- Verified all removable IPs were in the file

### 3. Convert String to List
- Applied `.split()` to `ip_addresses` to convert the string into a list of IPs

### 4. Iterate Through IPs
- Used a `for` loop to iterate through the IPs
- Printed each one to verify access to individual elements

### 5. Remove Unauthorized IPs
- Created a conditional `if` statement to check if IPs in the `remove_list` existed in `ip_addresses`
- Used `.remove()` to eliminate unauthorized entries

### 6. Overwrite File with Updated List
- Converted the cleaned list back to a string using `' '.join(ip_addresses)`
- Used `with open(import_file, "w") as file:` and `.write()` to overwrite the original file

---

## ✅ Summary of Tools & Concepts

- Python file handling: `open()`, `read()`, `write()`
- List methods: `.split()`, `.remove()`, `.join()`
- Iteration: `for` loop
- Conditional logic: `if` statements
- Access control logic through automation

---

## 📄 Supporting Document

- [Automating_IP_AllowList_Removal.pdf](Automating_IP_AllowList_Removal.pdf)

This document includes step-by-step screenshots, full explanations of the Python code, and output verification from the algorithm.

---

> 🗒️ *This project is based on a fictional lab scenario and is intended for educational purposes only.*
