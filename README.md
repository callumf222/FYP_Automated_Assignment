# FYP_Automated_Assignment
Automated Assignment Marking VIA Azure ChatGPT. This is developed in Python for my final year project.


This project is an intelligent application that automates the process of grading student PDF assessments using Azure OpenAI services. Designed for university-level assignments, the tool aims to streamline the marking workflow for educators and provide students with high-quality feedback.

🚀 Features
    Drag-and-Drop Interface: Easily upload multiple student PDF files.
    Word Count Validation: Submissions under 500 words are flagged for manual review.
    AI Feedback Generation: Uses GPT-3.5-turbo via Azure OpenAI to provide automated feedback based on a provided marking scheme.
    Excel Export: Automatically saves the AI feedback and marks in a structured Excel sheet.
    Manual Review Handling: Flags assignments that fail basic criteria (e.g., low word count) and skips AI processing.
    Simple and Intuitive UI: Minimal training required for staff usage.

🛠️ Technologies Used
    Python 3
    PyQt6 for GUI
    Azure OpenAI for AI-based marking
    pdfplumber for PDF text extraction
    openpyxl for writing results to Excel
    shutil/os for file operations

🧪 How It Works
    1. Launch the application.
    2. Drag and drop PDF assignments or browse to upload.
    3. Click "Upload and Generate Feedback".
    4. The application:
        Validates each file
        Extracts text (skipping cover page)
        Sends valid content to Azure OpenAI
        Writes feedback and marks to an Excel file

⚠️ Known Limitations
    Rate-limited by Azure OpenAI usage caps.
    Cannot fine-tune the model due to institutional data protection policies.
    Accuracy of AI feedback depends on the clarity and structure of input text.

📈 Future Enhancements
    UI for filtering flagged/manual entries.
    Integration with university LMS for automated uploads.
    Feedback customization options per course/module.
    Advanced NLP to ignore titles/references when counting words.