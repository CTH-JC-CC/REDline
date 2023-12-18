Script Name:
upload_github.py - GitHub File Uploader Script

Purpose:
To upload or update text files from the current directory to a specified GitHub repository.

Detailed Functionality:

GitHub API Interaction: The script interacts with the GitHub API to upload or update files in a repository.

File Reading: For each file, the script reads its content and encodes it in base64 format, which is required for the GitHub API.

File Checking: Before uploading, the script checks if the file already exists in the repository. If it does, the script updates the file; otherwise, it uploads the file as a new addition.

Authentication: The script uses a provided GitHub username and a personal access token for authentication.

Dependencies:

os: Python's built-in library for interacting with the operating system.
glob: Python's built-in library for file path pattern matching.
requests: Python library for making HTTP requests.
base64: Python's built-in library for base64 encoding.
Inputs:

GitHub username (hardcoded as 'CTH-JC-CC').
GitHub personal access token (hardcoded as 'github_api_key').
User input for the GitHub repository name.
Outputs:

Text files from the current directory are uploaded or updated in the specified GitHub repository.
Console messages indicating the success or failure of each file upload.

GitHub-Uploader/
â”‚
â”œâ”€â”€ scripts/
â”‚   â”œâ”€â”€ upload_github.py
â”‚   â””â”€â”€ ... (other scripts if any)
â”‚
â”œâ”€â”€ data/
â”‚   â”œâ”€â”€ ... (text files or other data files to upload)
â”‚
â”œâ”€â”€ logs/
â”‚   â””â”€â”€ upload_log.txt
â”‚
â”œâ”€â”€ config/
â”‚   â””â”€â”€ config.txt
â”‚
â”œâ”€â”€ assets/
â”‚   â””â”€â”€ ... (any images or other assets)
â”‚
â””â”€â”€ README.md