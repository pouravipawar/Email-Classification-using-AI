# Email Classification Using Artificial Intelligence

## Project Overview
This project implements an automated email classification and forwarding system using Natural Language Processing (NLP) and machine learning. Leveraging Google's Generative AI model and Python libraries, the system classifies incoming emails into predefined categories (complaint, query, or request) and forwards them to the respective departments. This solution aims to improve organizational efficiency by automating routine email management tasks.

## Key Features
- **Real-Time Monitoring**: Continuously monitors an inbox for new, unread emails.
- **AI-Powered Classification**: Utilizes Google Generative AI to classify emails based on their content.
- **Automated Forwarding**: Redirects emails to the appropriate recipient based on their classification.
- **Customizable**: Easily extendable to include additional categories or modify existing ones.

## System Workflow
1. **Email Retrieval**:
   - Connects to the email server via IMAP.
   - Retrieves unread emails from the inbox.

2. **Content Extraction**:
   - Extracts subject and body content of each email.
   - Handles multipart emails to extract plain text content.

3. **Classification**:
   - Uses Google Generative AI (`gemini-pro`) to classify emails into:
     - Complaint
     - Query
     - Request

4. **Forwarding**:
   - Based on the classification, emails are forwarded to the respective department's email address.

5. **Mark as Read**:
   - Marks the processed email as read to avoid reprocessing.

6. **Error Handling**:
   - Captures and logs errors to ensure robust operation.
