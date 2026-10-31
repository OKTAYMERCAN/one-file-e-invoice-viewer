# 🧾 One-File E-Invoice Viewer

![Dependencies](https://img.shields.io/badge/dependencies-none-brightgreen.svg)
![Platform](https://img.shields.io/badge/platform-Browser-darkred.svg)

A single HTML file that opens e-invoice files from around the world and shows them as a readable invoice, so you no longer have to deal with the PDF copy. No server, no build step, no installation, no internet connection. Download one file, open it and read your invoices.

## 🚀 Key Features

* ✅ **Zero setup:** One HTML file, no dependencies, no web server. Works offline by double-clicking. The page makes no network requests at all.
* ✅ **Many standards in one tool:** Detects the format by itself and converts it to one common invoice layout.
  * **UBL 2.1:** UBL-TR (Turkey e-Fatura and e-Arşiv), PEPPOL BIS 3.0, XRechnung (UBL), EN 16931, OIOUBL, NLCIUS. Invoices, credit notes and debit notes.
  * **UN/CEFACT CII:** Factur-X, ZUGFeRD 2 and XRechnung (CII), including the XML embedded inside a PDF/A-3 file.
  * **FatturaPA** (Italy), **CFDI 3.3 / 4.0** (Mexico), **NF-e / NFC-e** (Brazil) and **India e-Invoice** (IRP JSON, including the signed `SignedInvoice` token).
* ✅ **Any container:** Opens `.xml`, `.json`, `.pdf`, `.zip` and `.p7m`. Select several files at once, drop a ZIP full of invoices, or paste text with Ctrl+V.
* ✅ **Readable invoice:** Seller, buyer, document box, line items, tax breakdown, payment details, notes and totals. Credit notes, withholding, exemptions and prepaid amounts are shown correctly.
* ✅ **Copy tools:** Copy a text summary, or copy all line items and paste them straight into Excel.
* ✅ **Private by design:** Nothing is uploaded and nothing is stored except your language and theme choice. Text from the invoice is never run as HTML. XML files with a `DOCTYPE` or `ENTITY` are refused, and unpacked ZIP and PDF content is size-limited.
* ✅ **True black theme:** Pure `#000000` background for OLED screens, plus a light theme.
* ✅ **Bilingual:** Turkish and English interface, selected automatically from your browser language. Labels, dates, numbers, units and payment methods follow the language.

## 💻 Usage

[!NOTE] There is nothing to install. The file runs entirely inside your browser.

1. Download `one-file-e-invoice-viewer.html`
2. Open it in any modern browser (double-click is enough)
3. Choose a file, or drag one onto the page

Limits: it does not verify digital signatures, it only tells you whether the file contains one. ZUGFeRD 1.0 and non-invoice documents (despatch advice, application responses) are not supported and show a clear message. Signed `.p7m` files are read on a best-effort basis. Each file or unpacked archive is limited to 80 MB.

## 📸 Screenshots
(Light theme with example invoice)
<img width="914" height="1213" alt="image" src="https://github.com/user-attachments/assets/94245efe-552c-4b94-a92c-5d7f531e47c9" />

(Pure Black theme with example invoice)
<img width="923" height="1316" alt="preview" src="https://github.com/user-attachments/assets/dfaa5d19-aa8a-4f15-968f-660505dc22a7" />

## 📄 License

Copyright (C) 2026 Oktay Mercan https://github.com/OKTAYMERCAN/one-file-e-invoice-viewer

---
AI used.
