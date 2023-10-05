PDF Scraper and Uploader
This script scans specified websites for PDF files, downloads them, and uploads them to a Notion database.

Requirements
Python 3.6 or higher
requests
bs4
notion_client
tenacity
You can install these packages using pip:

pip install requests bs4 notion_client tenacity
Copy
Usage
Replace "YOUR_NOTION_TOKEN" and "YOUR_NOTION_DATABASE_URL" in the script with your actual Notion token and database URL.
Replace the websites_to_scan list with the websites you want to scan.
Run the script:
python script.py
Copy
The script will scan each website in the list for PDFs, download them, and upload them to the specified Notion database.

Features
The script uses the notion_client library to interact with the Notion API.
It uses BeautifulSoup to parse the HTML of the web pages and find links to PDF files.
It uses the requests library to download the PDF files.
It includes error handling for the Notion API calls and the file downloads.
It uses a set to keep track of visited URLs, preventing it from scanning the same page multiple times.
It includes a delay between file downloads to prevent overloading the server.
Limitations
The script currently does not support scanning websites that require login or have CAPTCHA protection.

Future Improvements
Future improvements could include support for scanning websites that require login, better error handling, and more customization options.
