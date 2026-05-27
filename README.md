# DevOps-Beginner-Roadmap3


# Log Analyzer Tool

A simple shell script tool for analyzing Nginx access logs from the command line.

This project helps practice basic shell scripting and Linux text-processing commands such as:

- awk
- sort
- uniq
- head
- grep
- sed

---

# Features

The script analyzes an Nginx access log file and displays:

- Top 5 IP addresses with the most requests
- Top 5 most requested paths
- Top 5 response status codes
- Top 5 user agents

---

# Project Structure

```bash
.
├── access.log
├── log_analyzer.sh
└── README.md
```

---

# Requirements

- Linux / macOS / WSL
- Bash shell
- Basic Unix utilities installed

---

# Download Sample Log File

You can download the sample Nginx log file using:

```bash
wget https://raw.githubusercontent.com/elastic/examples/master/Common%20Data%20Formats/nginx_logs/nginx_logs
```

Rename the file:

```bash
mv nginx_logs access.log
```

---

# Usage

## 1. Make the Script Executable

```bash
chmod +x log_analyzer.sh
```

## 2. Run the Script

```bash
./log_analyzer.sh
```

---

# Example Output

```text
Top 5 IP addresses with the most requests:
45.76.135.253 - 1000 requests
142.93.143.8 - 600 requests
178.128.94.113 - 50 requests
43.224.43.187 - 30 requests
86.134.118.70 - 20 requests

Top 5 most requested paths:
/api/v1/users - 1000 requests
/api/v1/products - 600 requests
/api/v1/orders - 50 requests
/api/v1/payments - 30 requests
/api/v1/reviews - 20 requests
Top 5 response status codes:
200 - 1000 requests
404 - 600 requests
500 - 50 requests
304 - 20 requests
```

---

# Commands Used


Used to extract specific fields from the log file.

Example:

```bash
awk '{print $1}'
```

---

## sort

Sorts the output alphabetically or numerically.

---


Counts duplicate entries.

---

## head

Displays the top results.

---

# Stretch Goal

Alternative implementations can be created using:

- grep
- sed

instead of relying mainly on `awk`.

---

# Learning Outcomes


- Shell scripting basics
- Log analysis
- Text processing in Linux
- Bash pipelines
- Command-line automation

These are important skills for DevOps and System Administration.

---

# Author

owolabigrace

#Project URL
https://roadmap.sh/projects/nginx-log-analyser
