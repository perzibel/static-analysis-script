
## Static-analysis-script 
Welcome to the Static Analysis Script! This Python tool is crafted to extract emails, paths, files, URLs, and IPs from the specified file for analysis.
## Purpose
This tool aids in the collection of data essential for static analysis, accelerating the detection of Indicators of Compromise (IOCs) and other potentially malicious activities executed by files.
## Installation

Before executing the tool, ensure the necessary packages are installed with the following command:

```bash
  pip install static-analysis-script
```
please make sure to download the latest version, currently 0.1.1
    
## Usage

```javascript
to execute the script:
main.py < file_path> < option>

Available options:

-u, -U Show only unique values from the strings

-e, -E Prints out the entropy calculation only

-c, -C Print the cert information including plenty of extra
```

![image](https://github.com/perzibel/static-analysis-script/assets/58742092/d6e8d129-3990-47ec-b68e-bd87aacc8d81)



## Analysis of Executables and DLL Files
The tool employs strings.exe to pull strings from executable (EXE) and dynamic link library (DLL) files, analyzing these strings to pinpoint paths, files, IP addresses, and URLs.
## Analysis of CSV Files
For Comma-Separated Values (CSV) files, the tool extracts relevant information by directly reading the contents of the files.
## Analysis of Word Documents
Utilizing the zipfile library, the tool processes Word documents, extracting embedded emails and URLs from various sections.
## Analysis of PDF Files

Currently, analysis of PDF files does not retrieve complete data and is under review for improvements.
