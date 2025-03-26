# BADAZ-ANTI-MVT
import os

# Path to scan
directory = "C:\\Path\\To\\Scan"  # add path or file location li biti

# List of known malicious file names
malicious_files = ['malware.exe', 'virus.bat', 'trojan.dll']

# Function to scan for malicious files
def scan_directory(path):
    for dirpath, dirnames, filenames in os.walk(path):
        for filename in filenames:
            if filename in malicious_files:
                print(f"Malicious file detected: {os.path.join(dirpath, filename)}")

# Start scanning
scan_directory(directory)
run on python btw
