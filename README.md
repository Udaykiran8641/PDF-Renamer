PDF Bulk Renamer
This is a simple, client-side web application that allows users to upload multiple PDF files and a corresponding list of new names. It then processes these files in the browser, "renaming" them (by creating new PDF files with the specified names), and packages them into a single ZIP archive for download.

Features
Bulk Renaming: Process up to 2000 PDF files at once.

Client-Side Processing: All file operations occur directly in your browser. No files are uploaded to any server, ensuring your privacy and data security.

ZIP Output: Downloads all processed PDFs conveniently in a single .zip file.

Progress Indicator: Shows the processing progress for large batches of files.

How it Works
Due to browser security restrictions, a web application cannot directly modify or rename files on your local file system. Instead, this application reads the content of your uploaded PDF files, creates new PDF files in memory with the desired names, and then bundles these new files into a ZIP archive for you to download.

Technologies Used
HTML5: For the basic structure of the web page.

CSS3 (Tailwind CSS): For modern and responsive styling.

JavaScript (Vanilla JS): For all the application logic and DOM manipulation.

PDF-Lib: A JavaScript library for creating, modifying, and embedding PDF documents in any JavaScript environment.

JSZip: A JavaScript library for creating, reading, and editing .zip files.

Setup and Running Locally
To use this application, you need to have the index.html, style.css, and script.js files in the same directory.

Save the files:

Save the HTML code as index.html.

Save the CSS code as style.css.

Save the JavaScript code as script.js.

Open in Browser: Simply open the index.html file in any modern web browser (e.g., Chrome, Firefox, Edge, Safari).

No web server is required as all processing is done client-side.

How to Use
Upload PDF Files:

Click on the "1. Upload PDF Files (Max 2000)" input field.

Select all the PDF files you wish to rename from your computer. The application will display the number of files selected.

Enter New Names/Serial Numbers:

In the "2. Enter New Names/Serial Numbers (One per line)" text area, type the desired new name for each PDF file.

Important: Enter one name per line. The order of the names in this text area must correspond to the order in which you selected the PDF files. For example, the first name in the list will be applied to the first PDF you selected, the second name to the second PDF, and so on.

Rename & Download PDFs:

Once you have selected your PDF files and provided the corresponding list of names, the "Rename & Download PDFs" button will become active.

Click this button to start the processing.

A progress indicator will show the current percentage of completion.

Once finished, a "Download Renamed PDFs (.zip)" link will appear. Click this link to download the ZIP file containing all your "renamed" PDFs.

Important Notes
Matching Counts: Ensure that the number of PDF files you upload exactly matches the number of names you provide in the text area. If they do not match, the application will display an error message.

File Extension: You do not need to include .pdf in your new names; the application will automatically append it if it's missing.

Performance: Processing a large number of PDFs (especially if they are large in file size) can consume significant browser memory and CPU resources, and may take some time. Please be patient.

Corrupted Files: If any individual PDF file is corrupted or in an unsupported format, the application will attempt to skip it and continue processing the remaining files, displaying an error message for the skipped file.

Privacy: Since all processing happens locally in your browser, your files are never transmitted over the internet or stored on any server.
