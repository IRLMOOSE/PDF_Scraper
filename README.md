<!DOCTYPE html>
<html>
<head>
    <title>README</title>
</head>
<body>
    <h1>Python Script for Downloading PDFs from Websites and Adding Them to Notion</h1>
    <p>This Python script scans specified websites for PDF files, downloads them, and adds them to a specified Notion database. It uses the notion_client library to interact with the Notion API.</p>

<h2>Dependencies</h2>
    <ul>
        <li>time</li>
        <li>requests</li>
        <li>os</li>
        <li>PyPDF2</li>
        <li>pdfreader</li>
        <li>BeautifulSoup from bs4</li>
        <li>urljoin, urlparse from urllib.parse</li>
        <li>Client from notion_client</li>
        <li>retry, stop_after_attempt, wait_fixed from tenacity</li>
    </ul>

<h2>Usage</h2>
    <p>Replace the NOTION_TOKEN and NOTION_DATABASE_URL variables with your Notion token and database URL, respectively. Add the websites you want to scan to the websites_to_scan list. Run the script.</p>

 <h2>Functions</h2>
    <ul>
        <li><b>log_to_file(message):</b> Logs messages to a file and prints them to the terminal.</li>
        <li><b>convert_rich_text_to_plain_text(rich_text):</b> Converts rich text (HTML) to plain text.</li>
        <li><b>get_pdf_info(file_path):</b> Returns the number of pages and file size of a PDF.</li>
        <li><b>add_to_notion(url, file):</b> Adds a PDF file to a Notion database.</li>
        <li><b>download_file(url):</b> Downloads a file from a URL.</li>
        <li><b>get_pdfs_from_url(url):</b> Scans a URL for PDFs, downloads them, and adds them to Notion.</li>
        <li><b>get_pdfs_from_websites(websites):</b> Calls get_pdfs_from_url() on a list of websites.</li>
    </ul>

<h2>Note:</h2>
    <p>The script waits 30 seconds between each download to avoid overloading the server.</p>

 </body>
</html>
