# AI Powered Invoice & Accounting Automation System

This project is an AI-powered invoice processing and accounting automation workflow built using n8n, Google Gemini AI, Gmail API, Google Drive API, and Notion API.

The workflow automatically detects invoice emails, extracts PDF invoice data, processes invoice information using AI, and stores structured accounting records into a Notion database.

---

# Workflow Architecture

![Workflow](Screenshot%20From%202026-05-11%2000-16-26.png)

---

# Features

- Automatic invoice email detection from Gmail
- PDF invoice extraction and processing
- AI-powered invoice data parsing using Google Gemini
- Structured JSON output generation
- Line-item extraction and validation
- Automatic database record creation in Notion
- Automated invoice management workflow
- Real-time accounting automation
- AI-based invoice verification and cleanup

---

# Tech Stack

- n8n
- Google Gemini AI
- Gmail API
- Google Drive API
- Notion API
- JSON Structured Output Parser

---

# Workflow Process

## 1. Gmail Invoice Detection

The workflow automatically monitors Gmail inbox for invoice-related emails and attachments.

---

## 2. File Upload and Processing

Invoice PDF files are uploaded and processed through Google Drive integration.

---

## 3. PDF Data Extraction

The system extracts raw text content from invoice PDF files.

---

## 4. AI Invoice Analysis

Google Gemini AI analyzes the extracted invoice text and identifies:

- Invoice name
- Company name
- Total invoice amount
- Line items
- Product/service descriptions
- Individual amounts

---

## 5. Structured JSON Generation

AI converts extracted invoice data into clean structured JSON format.

Example Output:

```json
{
  "invoice_name": "INV-2025-7789",
  "company_name": "Brightline Solutions Ltd.",
  "total_invoice_amount": 1549.75,
  "line_items": [
    {
      "description": "Website development",
      "amount": 1200
    },
    {
      "description": "Monthly hosting",
      "amount": 199.75
    },
    {
      "description": "Maintenance fee",
      "amount": 150
    }
  ]
}
```

---

## 6. Notion Database Integration

Processed invoice records are automatically stored into a Notion database for accounting and tracking purposes.

---

## 7. Automated Email Workflow

The workflow can send automated notifications and confirmations after successful invoice processing.

---

# AI Prompt Engineering

The workflow uses custom AI prompt engineering to:

- Extract invoice details accurately
- Handle missing or unclear fields
- Validate invoice totals
- Generate structured output
- Improve invoice processing consistency

---

# Automation Benefits

- Reduces manual invoice processing
- Saves accounting time
- Minimizes human errors
- Automates bookkeeping workflow
- Improves financial data organization
- Enables scalable invoice management

---

# Future Improvements

- Multi-currency support
- OCR support for scanned invoices
- Excel/CSV export
- Advanced analytics dashboard
- Duplicate invoice detection
- ERP integration

---

# Repository Structure

```text
project/
│
├── screenshots/
│   └── workflow.png
│
├── workflow/
│   └── workflow.json
│
└── README.md
```

---

# Demo

## Workflow Screenshot

The repository includes workflow architecture screenshots and execution flow examples.

---

# Author

Radoanul Arifen
