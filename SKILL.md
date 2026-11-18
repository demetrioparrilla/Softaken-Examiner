name: softaken-examiner-email-forensics description: Perform email forensic investigations using Softaken Examiner, a Windows-based email forensic examination tool. Examine PST, OST, EML, MSG, and MBOX evidence; search emails; inspect message headers, attachments, and metadata; analyse communication patterns; verify evidence integrity using SHA-256; reconstruct timelines; perform OCR; manage forensic cases; and generate investigation reports for legal investigations, compliance, and incident response. domain: cybersecurity subdomain: digital-forensics tags: [email-forensics, softaken-examiner, pst, ost, eml, msg, mbox, email-investigation, email-headers, attachment-analysis, metadata-analysis, sha256, evidence-integrity, timeline-analysis, ocr, forensic-reporting, case-management] version: "1.0" author: mahipal license: Apache-2.0
Softaken Examiner for Email Forensics
Overview

Softaken Examiner is a Windows-based email forensic examination tool designed to investigate, analyse, and manage digital email evidence. It supports multiple email storage formats, including PST, OST, EML, MSG, and MBOX.

The application provides forensic capabilities for examining email messages, searching communication records, reviewing message headers, analysing attachments, extracting metadata, identifying communication patterns, and maintaining evidence integrity.

Softaken Examiner also provides case management, timeline analysis, OCR capabilities, SHA-256 file integrity verification, and flexible reporting and export options.

This skill provides a structured operational workflow for using Softaken Examiner during digital forensic investigations, incident response, corporate investigations, and legal evidence examination.

When to Use
When investigating email-based security incidents using Softaken Examiner.
When examining PST, OST, EML, MSG, or MBOX evidence files.
When searching email communications for investigative keywords.
When reviewing suspicious email headers and sender information.
When examining email attachments and associated metadata.
When identifying communication patterns between individuals.
When reconstructing email communication timelines.
When verifying evidence integrity using SHA-256.
When conducting corporate email investigations.
When preparing forensic reports for legal or compliance investigations.
Prerequisites
Windows operating system.
Softaken Examiner installed on the forensic workstation.
Access to authorized email evidence files.
Sufficient disk space for evidence processing and report exports.
Appropriate permissions to examine the supplied evidence.
A dedicated investigation workspace.
Secure evidence storage for original files and exported results.

Official resources:

GitHub Repository: https://github.com/demetrioparrilla/Softaken-Examiner
Official Product Website: https://www.softaken.com/examiner/
Supported Email Evidence Formats
Format	Description	Forensic Purpose
PST	Outlook Personal Storage Table	Examine Outlook mailbox evidence
OST	Outlook Offline Storage Table	Examine cached Outlook mailbox data
EML	Electronic Mail Message	Investigate individual email messages
MSG	Outlook Message Format	Examine individual Outlook messages
MBOX	Mailbox Storage Format	Examine archived email communications
Softaken Examiner Investigation Workflow
1. Case Management

Begin by organizing the investigation using the application's case management functionality.

Recommended case information:

Field	Description
Case ID	Unique investigation identifier
Case Name	Investigation title
Investigator	Assigned forensic analyst
Investigation Date	Date of examination
Evidence Source	Origin of email evidence
Investigation Objective	Purpose of examination
Evidence Format	PST, OST, EML, MSG, or MBOX
Case Notes	Relevant investigative observations

Maintain separate records for original evidence, working evidence, and generated reports.

2. Import Email Evidence

Use Softaken Examiner to load the authorized email evidence files.

Investigation procedure:

Launch Softaken Examiner.
Create or select the relevant investigation case.
Locate the email evidence supplied for examination.
Import or open the supported email file.
Identify the available mailbox folders and messages.
Review the loaded evidence.
Record any processing errors or unsupported items.

Do not modify original evidence during examination.

3. Email Search and Examination

Use the application's email search capabilities to identify relevant communications.

Investigative search criteria may include:

Sender email address.
Recipient email address.
Email subject.
Message body keywords.
Date ranges.
Relevant communication terms.
Suspicious domains or addresses.

Example investigative keywords:

Keyword	Investigative Purpose
confidential	Identify potentially sensitive communications
password	Identify credential-related communications
transfer	Identify financial or data transfer discussions
invoice	Identify financial correspondence
attachment	Locate attachment-related communications
backup	Identify backup-related discussions
external	Investigate external communication
delete	Identify potentially relevant deletion discussions

Document search criteria and preserve the context of every relevant result.

4. Email Header Analysis

Use the application's message header examination capabilities to inspect available email routing and authentication information.

Important email headers:

Header	Forensic Significance
From	Claimed sender identity
To	Primary recipient
CC	Additional recipients
BCC	Blind-copy information, if available
Subject	Email subject
Date	Message timestamp
Message-ID	Message correlation identifier
Received	Mail routing information
Return-Path	Return address
Reply-To	Reply destination
Authentication-Results	SPF, DKIM, and DMARC results
DKIM-Signature	Email domain signature
X-Originating-IP	Possible originating IP information

Investigate:

Sender identity inconsistencies.
Suspicious email routing.
Unusual message timestamps.
Potential sender spoofing.
Authentication failures.
Unexpected external domains.

Do not treat an individual header anomaly as conclusive proof of malicious activity.

5. Attachment Analysis

Use Softaken Examiner's attachment examination capabilities to identify and review attachments associated with relevant email messages.

Record:

Field	Description
Email Subject	Source email subject
Sender	Attachment sender
Recipient	Attachment recipient
Filename	Original attachment filename
File Type	Identified attachment format
File Size	Attachment size
SHA-256	Attachment integrity hash, when calculated
Evidence Reference	Associated email or case identifier

Investigative considerations:

Unexpected executable attachments.
Office documents containing macros.
Archives and compressed files.
Files with misleading extensions.
Unusually large attachments.
Repeated attachment transfers.
Attachments sent to external email addresses.

Never execute suspicious attachments during forensic examination.

6. Email Metadata Analysis

Review available email metadata to identify relevant investigative information.

Examine:

Sender information.
Recipient information.
Message identifiers.
Message timestamps.
Message properties.
Attachment information.
Mailbox folder information.
Available file metadata.

Use metadata to correlate messages and identify inconsistencies.

Record unavailable metadata explicitly rather than assuming values.

7. Communication Pattern Analysis

Use the application's communication analysis capabilities to investigate relationships between email accounts.

Investigative objectives:

Identify frequently communicating email addresses.
Examine communication frequency.
Identify external communication relationships.
Identify unusual communication patterns.
Correlate messages between relevant individuals.
Identify potentially significant communication periods.

Example analysis:

Indicator	Investigative Relevance
Frequent external communication	Potentially relevant external relationships
Sudden increase in messages	Unusual communication activity
Large attachment transfers	Potential data movement
Unusual recipients	Communication requiring additional review
Repeated correspondence	Possible investigative relationship

Communication patterns are indicators for investigation, not automatic evidence of wrongdoing.

8. SHA-256 Evidence Integrity Verification

Use the application's SHA-256 integrity verification functionality to document evidence integrity.

For each evidence item, record:

Evidence identifier.
Original filename.
SHA-256 hash.
Verification date.
Verification result.
Evidence handling information.

Example verification record:

Evidence	Hash Algorithm	Verification
mailbox.pst	SHA-256	Record actual result
suspicious.eml	SHA-256	Record actual result
attachment.docx	SHA-256	Record actual result

A matching SHA-256 hash indicates that the compared files have matching hash values. It does not independently establish the authenticity or completeness of the evidence.

9. Timeline Analysis

Use the application's timeline analysis functionality to organize relevant email events chronologically.

Recommended timeline fields:

Field	Description
Date	Event date
Time	Event time
Sender	Email sender
Recipient	Email recipient
Subject	Message subject
Message ID	Unique message identifier
Event	Relevant communication
Evidence Reference	Associated evidence

Investigate:

Communication before and after an incident.
Unusual email activity.
Relevant attachment transfers.
Communication between important individuals.
Changes in communication frequency.

Preserve original timestamps and timezone information.

10. OCR Examination

Use Softaken Examiner's OCR capabilities when examining supported image-based or scanned evidence.

Potential investigative uses:

Extract text from scanned documents.
Examine image-based email evidence.
Identify readable information in document images.
Search extracted text for relevant keywords.
Correlate OCR findings with existing email evidence.

Document OCR limitations and manually verify important findings against the original evidence.

11. Forensic Reporting and Export

Use Softaken Examiner's reporting and export capabilities to prepare investigation documentation.

A professional forensic report should include:

Case identification.
Investigation objective.
Evidence inventory.
Evidence formats.
Examination methodology.
Email search findings.
Header analysis findings.
Attachment analysis findings.
Metadata observations.
Communication pattern analysis.
Timeline findings.
SHA-256 verification results.
OCR findings, where applicable.
Investigation limitations.
Conclusions.

Maintain exported reports separately from original evidence.

Investigation Example
Scenario: Corporate Email Data Leakage Investigation

Objective:

Investigate suspected unauthorized transmission of confidential corporate information through email.

Evidence supplied:

Evidence ID	Filename	Format
EV-001	employee_mailbox.pst	PST
EV-002	external_message.eml	EML
EV-003	suspicious_message.msg	MSG
Examination Procedure

Step 1: Case Creation

Create a dedicated investigation case in Softaken Examiner and record the evidence inventory.

Step 2: Mailbox Examination

Load the supplied PST evidence and examine available email folders and messages.

Step 3: Keyword Searching

Search for relevant terms:

confidential
internal
transfer
customer data
database
backup

Step 4: Header Examination

Review suspicious messages and examine sender, recipient, routing, and authentication information.

Step 5: Attachment Examination

Identify messages containing attachments and review their filenames, types, sizes, and associated metadata.

Step 6: Communication Analysis

Review communication patterns involving external recipients.

Step 7: Timeline Reconstruction

Correlate relevant messages chronologically to establish the sequence of communication events.

Step 8: Integrity Verification

Record SHA-256 hashes and verification results for available evidence.

Step 9: Report Generation

Generate and export the investigation report using Softaken Examiner.

Expected Investigation Output

The investigation should produce:

text
Softaken Examiner - Email Forensic Investigation
=================================================

Case ID: CASE-2026-001
Investigation: Corporate Email Data Leakage
Application: Softaken Examiner

--- Evidence Inventory ---

EV-001: employee_mailbox.pst
EV-002: external_message.eml
EV-003: suspicious_message.msg

--- Email Examination ---

Mailbox Examination: Completed / Pending
Email Search: Completed / Pending
Header Analysis: Completed / Pending
Attachment Examination: Completed / Pending

--- Metadata Analysis ---

Sender Information: Reviewed
Recipient Information: Reviewed
Message Identifiers: Reviewed
Email Timestamps: Reviewed

--- Communication Analysis ---

External Communications: Review Required
Unusual Communication Patterns: Review Required
Relevant Recipients: Documented

--- Evidence Integrity ---

Hash Algorithm: SHA-256
Hash Verification: Record Actual Results

--- Timeline Analysis ---

Relevant Events: Documented
Chronological Correlation: Reviewed

--- Reporting ---

Forensic Report: Exported / Pending
Case Documentation: Updated

--- Conclusion ---

Findings must be based on examined evidence.
Unverified observations must remain clearly identified.


The above is an illustrative report template, not actual output generated by the application.

Operational Guidelines for AI Agents

When assisting with Softaken Examiner investigations:

Always identify the investigation objective.
Identify the evidence formats supplied.
Guide the user through the corresponding Softaken Examiner functionality.
Do not substitute unrelated forensic utilities for the user's application unless explicitly requested.
Do not invent application menus, buttons, commands, or capabilities.
Do not claim that an investigation was completed without actual examination.
Preserve evidence integrity throughout the workflow.
Maintain a distinction between observations and conclusions.
Reference relevant evidence identifiers in findings.
Prepare structured reports based on actual examination results.
Important Limitations
Softaken Examiner is a Windows-based application.
Exact interface elements and supported operations should be verified against the installed application version.
Do not assume a command-line interface or public API exists.
Do not assume every email format exposes identical metadata.
Do not claim deleted-message recovery unless the relevant capability has been verified.
OCR accuracy depends on source quality.
SHA-256 verification must be based on actual calculated hashes.
The AI agent must not claim direct application control without an available integration.
References
Softaken Examiner GitHub: https://github.com/demetrioparrilla/Softaken-Examiner
Softaken Examiner Official Website: https://www.softaken.com/examiner/
libpff Project: https://github.com/libyal/libpff
RFC 5322 - Internet Message Format: https://datatracker.ietf.org/doc/html/rfc5322
RFC 6376 - DomainKeys Identified Mail: https://datatracker.ietf.org/doc/html/rfc6376
NIST Digital Evidence Guidance: https://www.nist.gov/digital-evidence
Final Objective

Use Softaken Examiner as the primary email forensic examination application to investigate digital email evidence, identify relevant communications, analyse headers and attachments, review metadata, examine communication patterns, validate evidence integrity, reconstruct timelines, and produce structured forensic investigation reports.

Prioritize evidence preservation, accuracy, reproducibility, and defensible forensic conclusions.
