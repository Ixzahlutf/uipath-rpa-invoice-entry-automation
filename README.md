# UiPath RPA – Invoice Entry Automation

## 📌 Introduction
This project is part of the **UiPath RPA Specialization Capstone**.  
The goal is to automate the **invoice entry process** by downloading invoices from Outlook, extracting data, and uploading it into an ERP application. The automation also generates an Excel report containing processed invoice details.

---

## 🎯 Project Background
Organizations often receive invoices as email attachments. Manually downloading, extracting, and uploading invoice data into ERP systems is **time-consuming** and **error-prone**.  
This automation project reduces manual effort by performing the entire workflow end-to-end.

---

## 📝 Problem Statement
- Invoices are received via Outlook email attachments.  
- Data from invoices must be extracted and uploaded to an ERP application.  
- A report must be generated after processing all invoices.  

---

## ✅ Expected Output
- Automate downloading of PDF invoice attachments.  
- Extract relevant fields (e.g., seller, buyer, items, totals).  
- Upload data into ERP form fields.  
- Generate an Excel report containing:  
  - Invoice number  
  - Number of processed items  
  - Timestamp  

---

## ⚙️ Environment Prerequisites

### 1. Applications / Software
- **UiPath Studio** (Academic Alliance Version 2021.10)  
- **Microsoft Excel** (for reporting)  
- **Microsoft Outlook** (for fetching invoices)  
- **ERP Application (InvoiceEntry.exe)** (provided with course materials)  

### 2. UiPath Packages
- UiPath.Excel.Activities (v2.11.4)  
- UiPath.System.Activities (v22.4.1)  
- UiPath.UiAutomation.Activities (v21.10.5)  
- UiPath.Mail.Activities (v1.12.3)  
- UiPath.PDF.Activities (v3.6.0)  

### 3. Initial Data Files
- Sample invoice PDFs (provided with course)  

---

## 🔄 Process Overview
1. **Read Outlook Emails** → Find unread emails with subject containing *“Invoice”*.  
2. **Download Attachments** → Save PDF invoices to project folder.  
3. **Open ERP Application** → Launch `InvoiceEntry.exe`.  
4. **Extract Invoice Data** → Company details, customer details, items, totals.  
5. **Upload Data** → Enter details into ERP fields and submit.  
6. **Generate/Update Excel Report** → Add invoice number, items processed, and timestamp.  
7. **Delete Processed Invoice** → Move to next invoice.  
8. **End** → Close ERP application when no invoices remain.  

---

## 📊 Example Invoice Fields
- **Company Info**: Name, Address, City, State, Pin Code, Contact No, TIN  
- **Customer Info**: Name, Address, City, State, Pin Code, Contact No, TIN  
- **Invoice Details**: Number, Date  
- **Items**: Item No, Description, Quantity, Price  
- **Totals**: Subtotal, GST, Total  

---

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/Ixzahlutf/uipath-rpa-invoice-entry-automation.git
````

2. Open the project in **UiPath Studio**.
3. Restore dependencies and configure Outlook mailbox.
4. Place sample invoices in Outlook with subject *“Invoice”*.
5. Run `Main.xaml`.

---

## 🏆 Outcome

* Automated retrieval and processing of invoice emails
* Accurate data entry into ERP application
* Automatic Excel reporting for processed invoices

---

## 👩‍💻 Author

Nurul Izzah Luthfiah Nur
📍 Jakarta, Indonesia
📧 [izzahluthfiah@gmail.com](mailto:izzahluthfiah@gmail.com)
🔗 [LinkedIn](https://linkedin.com/in/izzahluthfiah) | [GitHub](https://github.com/Ixzahlutf)

