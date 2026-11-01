# Office and PDF Reference

## DOCX
Use `python-docx` for paragraphs, runs, tables, styles, sections, headers, and footers. Advanced Word features may not round-trip perfectly. Render to PDF with LibreOffice when installed to check pagination.

## XLSX
Use `openpyxl` for workbook-aware edits. Load macro-enabled files with `keep_vba=True` when preserving VBA. Formula cells are not recalculated by openpyxl; use Excel or LibreOffice Calc when recalculation is required.

## PDF
Use PyMuPDF for rendering and page-level operations, pypdf for structural page manipulation, and ReportLab for creating PDFs. True redaction must remove underlying content. Reopen and render the final PDF to verify it.
