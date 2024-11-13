# Exercise-13-Invoice-Processing-automation-using-OCR

## Aim:

To automate the extraction of specific data (Invoice Number, Date, and Total Amount) from an invoice PDF using OCR and store the extracted information in an Excel file.

## Equipments Required:

UiPath Studio<br>
Invoice PDF file<br>
Excel file for storing extracted data<br>

#### Installed UiPath packages:

UiPath.PDF.Activities<br>
UiPath.IntelligentOCR.Activities<br>
UiPath.Excel.Activities<br>

## Procedure:

### Install UiPath and Required Packages:

Download and install UiPath Studio.<br>
Create a new project and install the necessary packages (PDF, OCR, Excel).<br>

### Read the Invoice PDF with OCR:

Use the Read PDF with OCR activity to extract text from the PDF.<br>
Choose an OCR engine like Tesseract to process the document.<br>

### Extract Specific Data Using Regex:

Add the Matches activity to extract the Invoice Number, Date, and Total Amount using regular expressions:<br>
Invoice Number: INV-\d+<br>
Date: \d{2}/\d{2}/\d{4}<br>
Total Amount: \₹?\d+(,\d{3})\*(\.\d{2})?<br>
Store the extracted values in variables.<br>

### Write Data to Excel:

Use the Excel Application Scope activity to open or create an Excel file.<br>
Write the extracted data (Invoice Number, Date, Total Amount) into specific cells using Write Cell activity.<br>

### Run and Test:

Run the workflow and verify that the data has been extracted correctly and saved into the Excel file.

## UiPath WorkFlow:
![Screenshot 2024-10-12 201545](https://github.com/user-attachments/assets/e578599f-0ed5-4dd0-8fde-04cdfa8b96ca)
![Screenshot 2024-10-12 202115](https://github.com/user-attachments/assets/a83f9882-a649-49bb-b27a-00a32a3b549f)
![Screenshot 2024-10-12 203238](https://github.com/user-attachments/assets/5c025df0-11ca-4e2c-bbb9-b9a986f6d03f)
![Screenshot 2024-10-12 203929](https://github.com/user-attachments/assets/b0440436-7881-4ff4-b637-69fc2abbfb05)
![Screenshot 2024-10-12 204423](https://github.com/user-attachments/assets/ed6c32d5-d871-407b-91e6-cef300986ef9)
![Screenshot 2024-10-12 204452](https://github.com/user-attachments/assets/8a2d0572-f23b-4ed7-ac31-6cf3ffb911ae)
![Screenshot 2024-10-12 204606](https://github.com/user-attachments/assets/b33004f2-1a67-4d54-b6d5-08090935f32b)
![Screenshot 2024-10-12 205632](https://github.com/user-attachments/assets/92aa12a9-ca3e-4b25-aebb-0009be824cbd)
![Screenshot 2024-10-12 205752](https://github.com/user-attachments/assets/f5547834-d4f7-490e-8dc3-97db35e7a888)
![Screenshot 2024-10-12 205924](https://github.com/user-attachments/assets/cf6fedbf-018f-47bb-ad28-c87371a032ce)
![Screenshot 2024-10-12 210327](https://github.com/user-attachments/assets/856d7719-f20b-4d84-ae16-5e893b5c783b)


## Result:

The automation successfully extracts the Invoice Number, Date, and Total Amount from the PDF and enters them into an Excel file, demonstrating efficient invoice processing using OCR.
