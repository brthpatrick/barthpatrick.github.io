---
title: "Table Recognition & Analysis App (Azure Form Recognizer)"
excerpt: "A C#/.NET application using Microsoft Azure Form Recognizer to extract, normalize and analyze tables from arbitrary documents for value extraction and relation discovery."
collection: portfolio
---

![Table Recognition](https://raw.githubusercontent.com/brthpatrick/barthpatrick.github.io/refs/heads/master/images/tablerecognizer.png)

**Table Recognition & Analysis** is a project implemented in **C# (.NET Framework)** that leverages **Microsoft Azure Form Recognizer** to automatically detect and parse *n* arbitrary tables from uploaded documents (PDFs, images). The application extracts structured data, normalizes values across multiple tables, and discovers relationships and commonalities between extracted datasets.

### Key goals
- Automatically detect and extract tables from heterogeneous documents.  
- Normalize and merge column values coming from different table layouts (e.g., unify date formats, currencies, product names).  
- Identify common keys and relationships across multiple tables and generate summary insights (aggregations, matches, discrepancies).  
- Provide a simple interface to upload files, review extracted tables, correct OCR errors, and export results (CSV/SQL).

### Main features
- **Azure Form Recognizer** integration for robust layout & table detection (pre-built and custom models).  
- **Backend** implemented in **C# (.NET Framework)** handling file uploads, calling the Azure service, and post-processing the predicted JSON.  
- **Normalization pipeline**: heuristics + rule-based and lightweight fuzzy matching to align column headers and values across tables.  
- **Relation discovery**: algorithms to find candidate join keys, compute intersections and discrepancies, and create summary reports.  
- **UI**: basic web interface for uploading documents, previewing extracted tables, manual correction, and exporting results.  
- **Persistence**: optional storage of results in SQL (MS-SQL) for further querying and historical analysis.  
- **Security & privacy**: consideration for sensitive data — support for local processing or controlled cloud storage, and deletion routines.

### Technologies
- Microsoft Azure Form Recognizer (REST API / SDK)  
- C# (.NET Framework) for backend processing  
- MS-SQL for optional storage and reporting  

### Outcomes & learnings
- Practical experience integrating AI/OCR cloud services into production-like workflows.  
- Handling noisy real-world tabular data: schema matching, normalization, and fuzzy joining.  
- Designing pipelines that combine ML-powered extraction with deterministic business logic for reliable results.  
- Considerations for data privacy when processing documents with potentially sensitive information.


