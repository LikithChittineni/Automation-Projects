AI-Powered Resume Screening Automation (n8n)
Overview

This workflow automates the initial candidate screening process using AI. 
Applicants submit their details and resume through a web form, the resume is analyzed by an LLM, and qualified candidates are automatically shortlisted, recorded in Google Sheets, and notified via email.

##Features
-📄 Resume upload and PDF text extraction
-🤖 AI-powered resume analysis using OpenAI GPT-4.1 Mini
-📊 ATS compatibility scoring (0-100)
-⭐ Candidate suitability rating and summary generation
-✅ Automatic shortlisting based on ATS score threshold
-📑 Candidate data storage in Google Sheets
-📧 HR notification emails
-📨 Automated confirmation emails to applicants

Candidate Form Submission
            │
            ▼
      Resume Upload
            │
            ▼
     PDF Text Extraction
            │
            ▼
      OpenAI Analysis
            │
            ▼
     Structured Output
            │
            ▼
     ATS Score Check
       (Score > 70)
            │
            ▼
   Add to Google Sheets
            │
            ▼
     Notify HR Team
            │
            ▼
 Send Confirmation Email



Workflow Steps:

1. Application Form

Candidates submit:

Full Name
Email Address
LinkedIn Profile
Resume (PDF)
2. Resume Processing

The uploaded PDF resume is automatically parsed and converted into text for AI evaluation.

3. AI Candidate Evaluation

The OpenAI model analyzes the resume against the target role:

Evaluation Outputs

ATS Score (0–100)
Compatibility Rating
Candidate Summary
Interview Recommendation
4. Shortlisting Logic

Candidates with an ATS Score greater than 70 are automatically shortlisted.

5. Data Storage

Qualified candidates are added to a Google Sheets database containing:

Candidate Name
Email
LinkedIn Profile
Resume Filename
ATS Score
AI Summary
6. Notifications
HR Notification

An automated email is sent to HR containing:

Candidate details
ATS score
LinkedIn profile
Resume information
Candidate Confirmation

Applicants receive an acknowledgment email confirming successful application submission.

Technologies Used
n8n – Workflow automation
OpenAI GPT-4.1 Mini – Resume analysis
Google Sheets API – Candidate database
Gmail API – Email notifications
PDF Extractor – Resume text extraction
Business Benefits
Reduces manual resume screening effort
Speeds up candidate evaluation
Provides consistent ATS scoring
Automates candidate communication
Creates a centralized shortlist database
Improves hiring efficiency
Future Enhancements
Multi-job role support
Dynamic job descriptions
Candidate ranking system
Interview scheduling automation
Integration with ATS platforms
Dashboard and analytics reporting
Result

This workflow transforms a traditional manual hiring process into an automated AI-assisted recruitment pipeline that evaluates resumes, shortlists qualified candidates, updates databases, and manages communication with minimal human intervention.
