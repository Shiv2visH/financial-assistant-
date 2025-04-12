# financial-assistant-
The Financial Assistant is a web-based application designed to help users manage their personal finances effectively. It provides tools for tracking income, expenses, savings, and financial goals while offering personalized budgeting advice.
# **Financial Assistant Application - Project Description**    

### **Key Features**  
✅ **Income & Expense Tracking**  
- Record monthly income  
- Track expenses across multiple categories (Housing, Food, Transportation, etc.)  

✅ **Budget Analysis**  
- Automatic calculation of total expenses  
- Shows remaining balance after expenses  
- Alerts for overspending  

✅ **Savings & Debt Management**  
- Track savings progress  
- Manage debts with interest rates  
- Get recommendations for emergency funds  

✅ **Financial Goal Tracking**  
- Set savings goals (e.g., vacation, emergency fund)  
- Track progress with visual indicators  

✅ **Personalized Financial Advice**  
- Budgeting tips  
- Debt repayment strategies  
- Investment recommendations  

✅ **Data Persistence**  
- Save financial data locally (JSON file)  
- Load previous data on startup  

---

## **Technology Stack**  

### **Backend (Python - Flask)**  
- **Framework:** Flask (Lightweight web framework)  
- **CORS Handling:** `flask-cors` for frontend-backend communication  
- **Data Storage:** JSON file (`financial_data.json`)  
- **Endpoints:**  
  - `GET /api/data` → Load saved financial data  
  - `POST /api/data` → Save new financial data  
  - `GET /api/budget` → Calculate budget summary  

### **Frontend (HTML, CSS, JavaScript)**  
- **UI Structure:** Simple, responsive form-based interface  
- **Dynamic Updates:** Real-time budget calculations  
- **User Experience:**  
  - Clean, intuitive design  
  - Error handling with alerts  
  - Progress tracking  

---

## **How It Works**  

### **1. User Input**  
- Enter **name, income, expenses, debts, and savings goals**.  
- The app stores this data in a JSON file.  

### **2. Budget Calculation**  
- The backend computes:  
  - **Total expenses**  
  - **Remaining balance**  
  - **Budget health status** (Healthy, Warning, Danger)  

### **3. Financial Advice**  
- Based on income vs. expenses, the app suggests:  
  - **Savings targets** (e.g., 3-6 months of emergency funds)  
  - **Debt repayment strategies** (focus on high-interest debts first)  
  - **Investment tips** (if savings are sufficient)  

### **4. Data Persistence**  
- All data is saved in `financial_data.json` and reloaded when the app restarts.  

---

## **How to Run the Project**  

### **Backend Setup**  
1. Install dependencies:  
   ```bash
   pip install flask flask-cors
   ```
2. Run the Flask server:  
   ```bash
   python financial_assistant_api.py
   ```
   - Runs on `http://localhost:5000`  

### **Frontend Setup**  
1. Open `index.html` in a web browser (Chrome/Firefox recommended).  
2. Use **Live Server** (VS Code extension) for best results.  

---

## **Expected Output**  
- **Budget Summary:**  
  ```
  Income: $5000.00  
  Expenses:  
    - Housing: $1500.00 (30%)  
    - Food: $600.00 (12%)  
    ...  
  Total Expenses: $3500.00  
  Remaining: $1500.00  
  Status: ✅ Healthy  
  ```  
- **Alerts:**  
  - ⚠️ *"You're spending more than you earn!"*  
  - 💡 *"Consider saving 20% of your income."*  

---

## **Possible Improvements**  
🔹 **User Authentication** (Multiple profiles)  
🔹 **Charts & Visualizations** (Expense breakdown)  
🔹 **PDF Export** (Budget reports)  
🔹 **Mobile App Version** (React Native/Flutter)  

---

## **Conclusion**  
This **Financial Assistant** helps users gain better control over their finances with simple, actionable insights. It’s ideal for personal budgeting, debt management, and long-term financial planning.  

🚀 **Try it out and take control of your finances today!**
