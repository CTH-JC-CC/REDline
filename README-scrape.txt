Script Name:
scrape.py - IOC (Indicators of Compromise) Extraction Script

Purpose:
To scrape a given website URL for various Indicators of Compromise (IOCs) such as SHA256, MD5, SHA1 hashes, IP addresses, domain names, email addresses, and filenames. The extracted IOCs are then saved to separate text files.

Detailed Functionality:

Web Scraping: The script sends a GET request to the provided URL and retrieves the website content.

Regular Expression Matching: The script uses multiple regular expression patterns to identify and extract different types of IOCs from the website content.

Data Cleaning: The script performs some data cleaning operations, such as:

Removing SHA1 hashes that are also MD5 or SHA256 hashes.
Removing MD5 hashes that are also SHA1 or SHA256 hashes.
Replacing the [.] pattern with . in domain names and IP addresses.
Data Writing: The script writes the extracted IOCs to separate text files, such as SHA256.txt, MD5.txt, SHA1.txt, IP.txt, Url.txt, Email.txt, and File.txt.

Dependencies:

re: Python's built-in regular expression library.
requests: Python library for making HTTP requests.
Inputs:

User input for the website URL.
Outputs:

Multiple text files containing the extracted IOCs.

IOC-Extraction/
â”‚
â”œâ”€â”€ scripts/
â”‚   â”œâ”€â”€ scrape.py
â”‚   â””â”€â”€ ... (other scripts if any)
â”‚
â”œâ”€â”€ input/
â”‚   â””â”€â”€ ... (any input files if any)
â”‚
â”œâ”€â”€ output/
â”‚   â”œâ”€â”€ SHA256.txt
â”‚   â”œâ”€â”€ MD5.txt
â”‚   â”œâ”€â”€ SHA1.txt
â”‚   â”œâ”€â”€ IP.txt
â”‚   â”œâ”€â”€ Url.txt
â”‚   â”œâ”€â”€ Email.txt
â”‚   â”œâ”€â”€ File.txt
â”‚   â””â”€â”€ ... (other output files if any)
â”‚
â”œâ”€â”€ logs/
â”‚   â””â”€â”€ app_log.txt
â”‚
â”œâ”€â”€ config/
â”‚   â””â”€â”€ config.txt
â”‚
â”œâ”€â”€ assets/
â”‚   â””â”€â”€ ... (any images or other assets)
â”‚
â””â”€â”€ README.md