Branch electron-nwjs-node-stream purpose is to use "PDFNodeStream" under electron/nwjs because it bypasses CORS restrictions.  

src/pdf.js
- If electron and blob URL: use PDFNetworkStream
- If electron: PDFNodeStream

src/shared/is_node.js:
- Added boolean to differenciate node and electron
