import json
from datetime import datetime
import os

input_file = "grype-report.json"
output_file = "grype-report.html"

if not os.path.exists(input_file):
    print("❌ JSON report not found, cannot create HTML file.")
    exit(1)

# Load JSON report
with open(input_file, "r") as f:
    data = json.load(f)

# Prepare HTML structure
html_content = f"""<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>Grype Vulnerability Report</title>
    <style>
        body {{
            font-family: Arial, sans-serif;
            margin: 40px;
            background: #fafafa;
        }}
        h1 {{
            color: #333;
        }}
        table {{
            border-collapse: collapse;
            width: 100%;
            margin-top: 20px;
        }}
        th, td {{
            border: 1px solid #ddd;
            padding: 8px;
        }}
        th {{
            background-color: #f2f2f2;
        }}
        tr:nth-child(even) {{
            background-color: #f9f9f9;
        }}
        tr:hover {{
            background-color: #e9e9e9;
        }}
        .critical {{ color: red; font-weight: bold; }}
        .high {{ color: darkorange; font-weight: bold; }}
        .medium {{ color: goldenrod; }}
        .low {{ color: green; }}
    </style>
</head>
<body>
    <h1>Grype Vulnerability Report</h1>
    <p>Generated on: {datetime.now().strftime("%Y-%m-%d %H:%M:%S")}</p>
    <table>
        <tr>
            <th>Package</th>
            <th>Version</th>
            <th>Vulnerability</th>
            <th>Severity</th>
            <th>Description</th>
        </tr>
"""

# Add vulnerabilities from JSON
for match in data.get("matches", []):
    vuln = match.get("vulnerability", {})
    artifact = match.get("artifact", {})
    severity = vuln.get("severity", "Unknown").lower()

    html_content += f"""
        <tr>
            <td>{artifact.get('name', 'N/A')}</td>
            <td>{artifact.get('version', 'N/A')}</td>
            <td>{vuln.get('id', 'N/A')}</td>
            <td class="{severity}">{vuln.get('severity', 'N/A')}</td>
            <td>{vuln.get('description', 'N/A')[:200]}...</td>
        </tr>
    """

html_content += """
    </table>
</body>
</html>
"""

# Write HTML file
with open(output_file, "w") as f:
    f.write(html_content)

print(f"✅ HTML report generated successfully: {output_file}")
