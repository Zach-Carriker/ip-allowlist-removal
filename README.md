# ip-allowlist-removal

# 🚫 Automating IP Allow List Removal

This project simulates the role of a security analyst at a healthcare company tasked with updating a restricted subnetwork's allow list. The goal: remove unauthorized IP addresses from a list that grants access to sensitive patient information and Personally Identifiable Information (PII).

## 🧠 Scenario

In this fictional lab environment, access to internal systems is controlled via IP-based allow lists. A group of employees have had their access revoked, and their IPs need to be automatically removed from the file `allow_list.txt`.

## 🛠 Process Overview

The project walks through a Python-based automation workflow to:

1. Open and read the allow list file (`allow_list.txt`)
2. Parse the file contents into a list using `.split()`
3. Use a `for` loop and `if` condition to check and remove any IPs from a defined `remove_list`
4. Convert the updated list back to a string with `.join()`
5. Overwrite the original allow list using `.write()` and file handling with `with open(..., "w")`

## 🧪 Tools & Methods Used

- Python file I/O (`open()`, `read()`, `write()`)
- String and list methods (`split()`, `join()`, `remove()`)
- Iterative and conditional logic (`for` loops and `if` statements)
- File update automation

## ✅ Skills Demonstrated

- Scripting for access control management
- Data manipulation for security automation
- Writing and refining defensive algorithms
- Practical understanding of access control concepts

## 📄 Supporting Document

- [Automating_IP_AllowList_Removal.pdf](docs/Automating_IP_AllowList_Removal.pdf)

---

> 🗒️ *Note: This project is educational and based on a fictional scenario.*
