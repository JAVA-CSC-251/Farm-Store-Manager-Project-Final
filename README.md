# 🐄 Farm Store Manager
**CSC-251 Advanced Java Programming – Module 4 Group Project**

A Java Swing application that simulates management software for a small family farm store.  
It tracks store inventory (with SKU numbers), animals, services, and employees—saving all data to CSV files for persistence.

---

## 🧭 Project Story
You inherited your aunt and uncle’s 10-acre farm, which includes a house, animals, and a store.  
They tracked everything with pencil and paper, so you decided to modernize operations with a computer program.

This program replaces the manual system and helps manage:
- 🛒 Items sold through the store  
- 🩺 Services (basic veterinary & grooming)  
- 🐇 Animal sales and breeder resales  
- 👩‍🌾 Employees and their time entries  

---

## 🧰 Technologies Used
- **Language:** Java 17 or newer  
- **IDE:** Visual Studio Code (Extension Pack for Java)  
- **GUI Framework:** Swing / JOptionPane  
- **Data Storage:** CSV files in the `data/` folder  
- **Version Control:** Git & GitHub  

---

## ⚙️ How to Run the Program

### ▶ Option 1 – Visual Studio Code (easiest)
1. Open the project folder in VS Code.  
2. Open `src/main/java/edu/ftcc/farmstore/App.java`.  
3. Click **▶ Run Java** (top-right of the editor).  
4. Use the tabs to explore:  
   - **Store** → manage products  
   - **Animals** → track animal sales  
   - **Services** → manage appointments  
   - **Employees** → track staff  

### 💻 Option 2 – Command Line
```bash
# Windows
javac -d bin src\main\java\edu\ftcc\farmstore\**\*.java
java -cp bin edu.ftcc.farmstore.App

# macOS / Linux
javac -d bin src/main/java/edu/ftcc/farmstore/**/*.java
java -cp bin edu.ftcc.farmstore.App

### 🧩 Option 3 – Maven (optional)
mvn clean package
java -jar target/farmstore-manager-1.0.0.jar

### 📂 Project Structure
Farm-Store-Manager-Project/
│
├── src/
│   └── main/java/edu/ftcc/farmstore/
│        ├── model/     → data classes (Item, Animal, ServiceType, Employee)
│        ├── repo/      → repositories handling CSV persistence
│        ├── ui/        → Swing GUI panels
│        ├── util/      → helpers (CSV, PathsCfg, Ids)
│        └── App.java   → main entry point
│
├── data/               → CSV files created on first run
│
├── README.md           → this file
└── pom.xml             → Maven build (optional)

🧪 Features / Testing Checklist
Feature	Description	CSV File
Store	Add/Edit/Delete items (SKU, name, category, price, qty, taxable)	inventory.csv
Animals	Add/Edit/Toggle Hold/Mark Sold/Delete animals	animals.csv
Services	Add/Edit/Delete available services	services.csv
Employees	Add/Edit/Delete employees	employees.csv
Persistence	All changes saved automatically	All CSV files

🧠 Lessons Learned

Organizing large Java projects into packages and classes

Implementing object-oriented design for reusability

Managing persistent data without a database

Collaborating via Git & GitHub

Building and testing Swing GUI applications


👥 Group Members
Name	  Role
Joey Ackerman-Lowery - Developer
Alexander Brinson - Developer
Joshua Carter - Developer
Haylee Paredes - Developer

🏁 Status

✅ Functional prototype completed
💾 Data persistence verified
🎨 GUI fully interactive
