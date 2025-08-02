# quickdesk
A simple, easy-to-use help desk solution to streamline communication between user and support team.
import os
import zipfile

# Define the directory structure and placeholder files
project_structure = {
    "quickdesk/": {
        "README.md": "# QuickDesk\n\nQuickDesk is a simple, easy-to-use help desk solution where users can submit support requests, and staff can manage and resolve them efficiently.",
        ".gitignore": "__pycache__/\nnode_modules/\n.env",
        "LICENSE": "MIT License\n\nCopyright (c) 2025",
        "backend/": {
            "app.py": """# Backend entry point
from flask import Flask, jsonify

app = Flask(__name__)

@app.route('/')
def home():
    return jsonify({'message': 'Welcome to QuickDesk API'})

if __name__ == '__main__':
    app.run(debug=True)
""",
            "requirements.txt": "flask\n",
        },
        "frontend/": {
            "index.html": """<!DOCTYPE html>
<html>
<head>
  <title>QuickDesk</title>
</head>
<body>
  <h1>Welcome to QuickDesk</h1>
  <script src="app.js"></script>
</body>
</html>
""",
            "style.css": "body { font-family: Arial, sans
