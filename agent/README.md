# Supervisory AI Agent Layer (Planned)

This folder will contain the **AI agent layer** built on top of the
Cambridge × Bank of England financial NLP system in this repository.

The planned agent will be able to:

- query and filter JP Morgan & HSBC Q&A segments by topic and PRA risk area  
- analyse sentiment and tone divergence between management and analysts  
- flag potentially evasive or non-transparent answers  
- generate short, supervisory-style briefings for a chosen bank and quarter  

The first implementation is expected as:
- an n8n-based workflow (no-code orchestration), and
- a lightweight Python prototype using the existing notebooks as tools.
