# backlog_lookup
Using OpenRefine and OCLC's WorldCat Search APIs, the process automates the work of backlog searching. It automatically searches WorldCat for cataloging copy by LCCN, ISBN, and NETWORK_NUMBER (OCLC number).

# What you need
1. OpenRefine (openrefine.org)
2. Your own WSKey (https://www.oclc.org/developer/develop/authentication/how-to-request-a-wskey.en.html)
3. Spreadsheet that contains the following columns: BIB_ID, MFHD_ID, TITLE_BRIEF, BEGIN_PUB_DATE, LANGUAGE, DISPLAY_CALL_NO, LCCN, ISBN, NETWORK_NUMBER in that order. Sample spreadsheet is Sample_Backlog_List.xlsx.

# Steps
1. Replace {YOUR_WSKEY} with your own WSKey in backlog_lookup.txt.
2. Open OpenRefine and create a new project.
3. Once your spreadsheet is uploaded, go to Undo/Redo tab, click "Apply."
4. Copy the entire JSON code in backlog_lookup.txt and paste it into the pop-up window.
5. Click "Perform Operations."
6. If the process finds good matching records, it returns OCLC number, call number (if any), existence of LC Subject Headings, and encoding level.
7. The process considers OCLC records with English cataloging language, encoding levels (blank, 1, 4, I, M) and LC Subject Headings (except for fiction) acceptable for copy cataloging.

# Demo
https://youtu.be/4zoIGS1G_QI
