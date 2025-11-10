# Azure RAG Sales Assistant

**An AI-powered Retrieval-Augmented Generation (RAG) solution** that helps sales teams query company data using natural language.  
This prototype integrates **Azure OpenAI**, **Azure Cognitive Search**, and **Microsoft Fabric Lakehouse** to provide real-time, context-aware answers sourced from internal knowledge bases.

---

## Overview

The **Azure RAG Sales Assistant** demonstrates how sales organizations can harness enterprise data securely with Large Language Models (LLMs).  
It connects structured and unstructured data sources — such as CRM data, product information, and support documents — and augments Azure OpenAI responses with context retrieved from indexed content.

---

## Key Capabilities

- Natural language Q&A interface for sales and customer data  
- Context retrieval via **Azure Cognitive Search** or **Fabric Lakehouse**  
- Vector indexing and embeddings for semantic search  
- Secure integration using **Azure Entra ID (Active Directory)**  
- Optionally connects to **Power BI** or **Fabric Data Warehouse** for reporting  
- Fully serverless — deployable using Azure App Service, Functions, or Fabric Notebooks  

---

## Architecture

| Layer | Technology |
|--------|-------------|
| LLM | Azure OpenAI (GPT-4 or GPT-4 Turbo) |
| Data Indexing | Azure Cognitive Search / Fabric Lakehouse |
| Embeddings | OpenAI text-embedding-3-large |
| Storage | Fabric OneLake or Azure Blob |
| Orchestration | Python (FastAPI) or Logic Apps |
| UI | Streamlit or React (optional frontend) |

---

## Quick Start

```bash
# Clone repository
git clone https://github.com/incra-ai/azure-rag-sales-assistant.git
cd azure-rag-sales-assistant

# Create virtual environment
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows

# Install dependencies
pip install -r requirements.txt

# Run locally
python app.py
```
