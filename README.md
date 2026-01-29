🤖 AI Procurement Proposal Analyzer
AI-powered pipeline for supplier proposal analysis using Python + OpenAI API, focused on Strategic Sourcing, Procurement and Executive Decision-Making.

📌 Overview
This project demonstrates a real-world application of Generative AI to business decision processes, automating the analysis, comparison, and recommendation of supplier proposals in procurement scenarios.

The solution was designed with governance, auditability, and business rationale in mind — not just automation.

🎯 Business Problem
Procurement and sourcing teams frequently deal with:

multiple proposals in unstructured formats
high manual effort to compare technical and commercial data
subjective evaluations with limited traceability
difficulty justifying decisions to executives and auditors
This project addresses these challenges by applying LLMs in a structured and controlled pipeline, transforming raw proposals into clear, defensible insights.

🧩 Solution
The solution is implemented as a three-step AI pipeline:

Proposal Normalization
Extracts and standardizes commercial, technical, and contractual data without judgment.

Evaluation & Scoring
Applies weighted criteria (TCO, risk, SLA, compliance, ESG) and generates a ranked comparison.

Executive Report Generation
Produces a structured executive and technical report to support approval and negotiation.

🏗️ Project Architecture
ai-procurement-proposal-analyzer/
│
├── config.py
├── main.py
│
├── prompts/
│   ├── normalize.txt
│   ├── evaluate.txt
│   └── report.txt
│
├── loaders/
│   ├── text_loader.py
│   └── pdf_loader.py
│
├── llm/
│   └── openai_client.py
│
├── pipeline/
│   ├── step1_normalize.py
│   ├── step2_evaluate.py
│   └── step3_report.py
│
├── inputs/
│   └── propostas.txt
│
├── outputs/
│   └── sample_report.md
│
└── README.md
⚙️ Technologies
Python 3.10+
OpenAI API (LLMs)
Prompt Engineering
Markdown for report generation
Easily extensible to Pandas, Matplotlib, python-docx, and Streamlit.

🔐 Governance & Best Practices
No hallucinated data
Explicit marking of missing information as “NOT PROVIDED”
Clear separation between facts, risks, and interpretation
Reproducible and auditable pipeline
All data used in this repository is fictitious or anonymized.

🚀 How to Run
pip install -r requirements.txt
export OPENAI_API_KEY=your_openai_api_key_here
python main.py
The final report will be generated in the outputs/ folder.

📈 Expected Outputs
Structured supplier comparison
Weighted scoring and ranking
Risk identification
Executive recommendation with justification
🧠 Key Differentiators
AI applied to a real business problem
Focus on executive decision-making, not demos
Modular, scalable architecture
Professional prompt engineering
👤 Author
José Alexandre
Procurement Specialist & AI Applied to Business

📌 Disclaimer
This project is presented as a professional portfolio and does not represent real company data or decisions.
