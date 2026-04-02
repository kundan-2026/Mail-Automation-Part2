# 📩 Customer Request Automation (UiPath)

This project automates the processing of customer request emails received with the subject **"New Customer Request"**. It extracts, validates, and categorizes data based on predefined business rules.

## 🚀 Workflow

1. Filter emails with subject **"New Customer Request"**  
2. Identify data source:
   - Email body  
   - PDF attachment  
3. Extract required details:
   - Customer Name  
   - Email ID  
   - Request Type  
   - Date of Birth (format: yyyy-MM-dd)  
   - Phone (digits only)  
   - Country (uppercase)  

## 📊 Validation Rules

- **Mandatory Fields**:
  - Customer Name  
  - Email ID  
  - Request Type  

- **Data Formatting**:
  - DOB → yyyy-MM-dd  
  - Phone → digits only  
  - Country → uppercase  

## 📂 Folder Classification

- ✅ **Success**  
  - All fields are valid  

- ⚠️ **Business Exception**  
  - Any mandatory field is missing  

- ❌ **System Exception**  
  - PDF reading failure or Outlook issue  

## 📈 Logging & Reporting

- Maintain a **log table** to track:
  - Total emails processed  
  - Successful transactions  
  - Business exceptions  
  - System exceptions  

- Send a **final summary email** including:
  - Total Emails Processed  
  - Successful Count  
  - Business Exceptions Count  
  - System Exceptions Count  

## ✅ Benefits

- Automates customer request handling  
- Ensures data validation and standardization  
- Improves accuracy and efficiency  
- Provides clear reporting and tracking  

---

💡 Built using UiPath to demonstrate end-to-end email automation with validation, exception handling, and reporting.
