# 📄 CV Analysis Tool

A Streamlit-based application for analyzing CVs, identifying skill gaps, and ranking candidates for specific job roles.

## 🌟 Overview

This project consists of three main Python scripts that provide a comprehensive CV analysis and recruitment tool:

- **🚀 app3_streamlit.py**: Launcher interface for selecting and running CV analysis modules.
- **🔍 Section1_streamlit.py**: Analyzes a single CV to identify skill gaps against a chosen job role, with features to ask custom questions and generate learning paths.
- **📊 Section3_streamlit.py**: Batch processes multiple CVs, ranks candidates based on skills and experience, and includes a chatbot for querying processed CV data.

## ✨ Features

- **🛠️ Skill Gap Analysis**: Compares CV skills against job requirements using Gemini AI and MongoDB.
- **📂 Batch Processing**: Processes multiple CVs in parallel, storing results in MongoDB for ranking.
- **🏆 Candidate Ranking**: Scores CVs based on skill match and relevant experience.
- **💬 Chatbot Interface**: Allows querying of processed CV data for insights.
- **🎨 Interactive UI**: Streamlit frontend with intuitive controls and result visualization.

## 🛠️ Tech Stack

- **🐍 Python**: Core programming language.
- **🌐 Streamlit**: Web framework for building interactive UIs.
- **🗄️ MongoDB**: Database for storing job roles, required skills, and processed CV data.
- **🤖 Google Gemini AI**: For skill extraction, experience calculation, and chatbot functionality.
- **📜 pdfplumber**: PDF text extraction.
- **🖼️ pytesseract**: OCR fallback for text extraction from images in PDFs.
- **📈 pandas**: Data manipulation and display for ranking results.
- **⚡ concurrent.futures**: Parallel processing of CVs in batch mode.

## 🚀 Usage

1. **🛠️ Setup**: Install dependencies (`pip install streamlit pymongo pdfplumber pytesseract google-generativeai pandas`).
2. **🔧 Configuration**:
   - Set `GOOGLE_API_KEY` and `MONGODB_URI` in Streamlit secrets.
   - Ensure Tesseract is installed for OCR (optional).
3. **▶️ Run**: Launch the app with `streamlit run app3_streamlit.py`.
4. **📚 Modules**:
   - Use **Employee Skill Gap Analyzer** for single CV analysis.
   - Use **Recruitment Batch Processing** for bulk CV processing and ranking.

## 📝 Notes

- Requires valid Google API keys and MongoDB URI for full functionality.
- Ensure CVs are in PDF format for processing.
- Batch processing uses parallel execution to optimize performance.
