# SCC Québec — Suppliers' Day / Journée des fournisseurs

Vercel-ready static attendance and certificate application.

## Deploy
Import this folder into Vercel. No build command is required.

## Included
- SCC Québec logo, embedded inline (header, certificate, and favicon) and brand colors
- Suppliers' Day / Journée des fournisseurs
- English/French certificate language selection
- Conference attendance selection, with a "Select all / Deselect all" toggle
- Automatic selected-session time calculation
- Certificate signed by Hiba Al Hakim, President of SCC Québec, with a styled signature and printed name/title
- Montréal, Québec, Canada location
- Automatic PDF generation and download as soon as the certificate is generated (no extra click needed), plus manual "Download PDF" and "Print" buttons as backups
- Vercel configuration

## Note
The PDF generator uses the html2canvas and jsPDF CDNs (both from cdnjs) loaded in `index.html`, so the deployed site needs internet access for PDF generation. The PDF page is sized to exactly match the rendered certificate, so it always comes out as a single page with no splitting or extra blank space. If the CDN fails to load (e.g. offline), the page falls back to the browser's Print dialog ("Print" button) so a certificate can still be saved as PDF.
