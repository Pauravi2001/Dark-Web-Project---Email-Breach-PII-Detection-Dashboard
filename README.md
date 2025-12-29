This project implements a privacy-preserving email breach and PII detection system using only synthetic and publicly allowed datasets. 
The system allows a user to enter an email address and checks whether it appears in a simulated breach dataset. Institutional email addresses 
such as @spit and @spit.ac.in are automatically flagged to highlight higher-risk exposure.

In addition, the system scans synthetic data-leak files to detect Personally Identifiable Information (PII) including email addresses, phone numbers, 
and names using regex-based detection techniques. Each detected PII instance generates a structured alert containing the source file, PII type, detected value, 
confidence score, and timestamp.

All detected alerts are automatically exported as CSV and JSON reports for audit and analysis purposes. A Streamlit-based interactive dashboard summarizes 
breach status, PII detections, and institutional exposure through tables, metrics, and visualizations. The application is deployed in a headless environment 
(Google Colab) using ngrok, demonstrating a practical and ethical approach to breach analysis without performing real dark-web crawling.
