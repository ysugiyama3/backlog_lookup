# backlog_lookup
Using OpenRefine and OCLC's WorldCat Search APIs, the process automatically searches WorldCat cataloging copy by LCCN, ISBN, and NETWORK_NUMBERe (OCLC number) This automates the work of backlog searching.

# What you need
1. OpenRefine (openrefine.org)
2. Your own WSKey (https://www.oclc.org/developer/develop/authentication/how-to-request-a-wskey.en.html)
3. Spreadsheet that contains columns: BIB_ID, MFHD_ID, TITLE_BRIEF, BEGIN_PUB_DATE, LANGUAGE, DISPLAY_CALL_NO, LCCN, ISBN, NETWORK_NUMBER in that order.

# Steps
1. Replace {YOUR_WSKEY} with your own wskey in backlog-lookup.txt.
2. Open OpenRefine and create a new project.
3. Once your spreadsheet is uploaded, go to Undo/Redo tab, click "Apply."
4. Copy the entire JSON code and paste it into the pop-up window.
5. Click "Perform Operations."
6. If the process finds good matching records, it returns OCLC number, call number, existence of LC Subject Headings, and encoding level.
7. The process considers OCLC records with English cataloging language, encoding levels (blank, 1, 4, I, M) and LC Subject Headings (except for fictions) acceptable for copy cataloging.

# Demo
https://youtu.be/2TY6RHxEe0E
