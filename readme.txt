CLASS NOTES HUB
================

Overview
--------
Class Notes Hub is a simple, responsive student resource website prototype.
It provides a place to browse academic units, filter units by semester, search
for units, and open learning-resource files.

Current project files
---------------------
notes_hub.html
    Main website page. It contains the HTML structure, CSS styling, semester
    filters, search functionality, and the unit/resource catalog.

readme.txt
    Project information and setup notes.

How to preview
--------------
1. Download or clone the repository.
2. Open notes_hub.html in a modern web browser.
3. Use the semester tabs to filter the displayed units.
4. Enter a unit name in the search field to find a unit.

Configure resource downloads
----------------------------
The page uses this S3 storage base URL:

https://notes-hub-precious-2026.s3.eu-north-1.amazonaws.com/public/

The units list is currently empty because no learning resources have been
uploaded yet. After uploading resources under the public/ prefix, add each
unit and its exact object keys to the units array in notes_hub.html. For
example, use a unique key such as Intro-to-Programming/Week-1-Notes.pdf
when the object is stored in that folder.

Resources must be reachable by the browser at their HTTPS URLs. Do not put
private credentials or secret keys in frontend files.

Current functionality
---------------------
- Responsive unit-card layout
- Semester 1, Semester 2, and All filters
- Search by unit name
- Empty state until real unit and resource data is added

Not yet implemented
-------------------
- User accounts and authentication
- Student resource uploads
- Upload moderation and administrator tools
- Database-backed units and resources
- Resource preview and download tracking

Development notes
-----------------
This is currently a static HTML/CSS/JavaScript prototype. No backend or
database is configured yet. Do not place private credentials or secret keys
in frontend files.

Future development can introduce a backend, database, secure file storage,
student contributions, and administration features as the project grows.
