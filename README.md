# Metadata-Based-Document-Authenticity-Verification-System
A digital forensic analyser that extracts and cross-verifies metadata from PDF, DOCX, and image files. It uses SHA-256 hashing to check file integrity and basic anomaly detection to identify unusual metadata patterns, generating structured reports to help assess document authenticity and potential tampering.
# Metadata-Based Document Authenticity Verification System

A digital forensics project that analyses document metadata and file integrity to identify potential signs of tampering in digital documents.

## Overview

Digital documents contain metadata that can provide useful information about their origin, properties, and modification history. However, this information can be altered, making document verification challenging.

This project aims to examine metadata from multiple document formats, perform file integrity checks, and identify unusual metadata patterns to support basic digital forensic analysis.

## Features

- **Multi-Format Metadata Extraction:** Extracts available metadata from PDF, DOCX, and image files.
- **Metadata Analysis:** Examines document properties such as timestamps and author information where available.
- **File Integrity Verification:** Uses SHA-256 hashing to identify changes in file contents through hash comparison.
- **Cross-Verification:** Uses multiple tools to examine and compare extracted metadata.
- **Anomaly Detection:** Identifies unusual metadata patterns that may indicate potential inconsistencies.
- **Report Generation:** Generates structured reports containing document analysis results.

## Technologies Used

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Flask | Web application framework |
| SHA-256 | File integrity checking |
| HTML / CSS | User interface |
| Metadata extraction libraries | Document metadata analysis |

## Supported File Formats

- PDF (`.pdf`)
- Word Documents (`.docx`)
- Images (`.jpg`, `.jpeg`, `.png`, where supported)

## System Workflow

1. Upload a digital document.
2. Extract available metadata from the uploaded file.
3. Analyse metadata for unusual patterns.
4. Perform SHA-256 hashing for file integrity verification.
5. Cross-verify extracted information.
6. Generate a structured analysis report.

## Project Structure

```text
Metadata-Based-Document-Authenticity-Verification/
│
├── app.py
├── requirements.txt
├── templates/
├── static/
├── uploads/
├── reports/
└── README.md
```

*The directory structure may vary depending on the implementation.*

## Getting Started

### Prerequisites

- Python 3.x
- pip

### Installation

1. Clone the repository:

```bash
git clone <your-repository-url>
```

2. Navigate to the project directory:

```bash
cd Metadata-Based-Document-Authenticity-Verification
```

3. Install the required dependencies:

```bash
pip install -r requirements.txt
```

4. Run the application:

```bash
python app.py
```

5. Open the local URL displayed in your terminal to access the application.

## Project Objective

To explore the role of metadata analysis and file integrity verification in digital forensics and develop a system that helps identify potential inconsistencies and signs of document tampering.

## Disclaimer

This project is intended for educational and basic digital forensic analysis. Metadata analysis and hash comparisons can help identify inconsistencies but cannot independently guarantee document authenticity or conclusively prove tampering.

## Author

Developed as an academic project.
