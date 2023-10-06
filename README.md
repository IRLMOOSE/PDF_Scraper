<h1>PDF Scraper and Uploader</h1>
<p>This script scans specified websites for PDF files, downloads them, and uploads them to a Notion database.</p>

<h2>Requirements</h2>
<p>Notion Database Key</p>
<p>Notion API Token
<p>Python 3.6 or higher requests bs4 notion_client tenacity</p>
<p>You can install these packages using pip:</p>
<code>pip install requests bs4 notion_client tenacity</code>

<h2>Usage</h2>
<p>Replace "YOUR_NOTION_TOKEN" and "YOUR_NOTION_DATABASE_URL" in the script with your actual Notion token and database URL. Replace the websites_to_scan list with the websites you want to scan. Run the script:</p>
<code>python script.py</code>
<p>The script will scan each website in the list for PDFs, download them, and upload them to the specified Notion database.</p>

<h2>Features</h2>
<p>The script uses the notion_client library to interact with the Notion API. It uses BeautifulSoup to parse the HTML of the web pages and find links to PDF files. It uses the requests library to download the PDF files. It includes error handling for the Notion API calls and the file downloads. It uses a set to keep track of visited URLs, preventing it from scanning the same page multiple times. It includes a delay between file downloads to prevent overloading the server.</p>

<h2>Limitations</h2>
<p>The script currently does not support scanning websites that require login or have CAPTCHA protection.</p>

<h2>Future Improvements</h2>
<p>Future improvements could include support for scanning websites that require login, better error handling, and more customization options.</p>
