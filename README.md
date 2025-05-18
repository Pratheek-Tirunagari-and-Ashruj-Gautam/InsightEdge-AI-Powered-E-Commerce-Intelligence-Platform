# E-Commerce Analytics System with LLM-Augmented Intelligence (Work in Progress) 

## Overview

This project presents a comprehensive e-commerce analytics system developed using PostgreSQL. It is based on the Brazilian E-Commerce Public Dataset and is designed to enable scalable storage, efficient querying, and insightful reporting of customer, order, payment, and seller data. The system is currently being extended with LLM-powered capabilities to support intelligent text analysis and automated business reporting.

## Phase 1: PostgreSQL-Based Analytics System

### Technologies Used
- PostgreSQL
- SQL (DDL, DML, analytical queries)
- PL/pgSQL (stored procedures, triggers)
- Indexing and query optimization
- Dataset: Brazilian E-Commerce (Olist) from Kaggle

### Core Features Implemented
- Structured schema with 11+ interconnected tables representing customers, orders, products, payments, geolocation, and more
- Data cleaning and loading using SQL scripts
- Complex queries including sales analysis, delivery performance, seller rankings, and customer behavior
- Stored procedures for customer and order management
- Transaction handling with error logging via triggers
- Performance improvements using EXPLAIN ANALYZE and targeted indexing

### Deliverables
- `load_create.sql`: Defines all table schemas, constraints, and data load operations
- `sql project 2.sql`: Contains all core SQL operations including CRUD operations, business queries, functions, triggers, and indexing logic
- `Phase2report.pdf`: Project documentation detailing schema design, implementation rationale, ER diagram, use cases, and optimization analysis

## Phase 2: Integration of Large Language Models (In Progress)

The project is being expanded to incorporate LLMs for deriving insights from unstructured data, particularly customer interactions and feedback. This will include both inference using pre-trained models and fine-tuning smaller open-source models.

### Planned Additions
- Python scripts for:
  - Summarizing feedback from the `customer_interactions` table
  - Classifying feedback into actionable categories (e.g., delivery issue, product defect, etc.)
  - Generating natural-language summaries of monthly sales and KPI reports
- Fine-tuning a 7B parameter LLM (e.g., Mistral or LLaMA 2) using QLoRA on an RTX 4090 setup
- Building a Gradio or Streamlit interface for real-time text analysis
- Integrating visual dashboards (Power BI or Tableau) to present insights

### Intended Use Cases
- Automated executive summaries from raw SQL outputs
- Topic classification of free-text customer complaints
- Time-based sentiment tracking from feedback scores

## Authors and Contributions

| Name               | Contributions                                              |
|--------------------|------------------------------------------------------------|
| Pratheek Tirunagari| Schema design, stored procedures, analytics queries, indexing, documentation |
| Ashruj Gautam      | Trigger mechanisms, performance analysis, advanced SELECT queries, data maintenance logic |

## Project Status

- SQL infrastructure and analytics complete
- LLM integration and NLP module under development (Expected completion in ~6–8 weeks)

## License

This project is licensed under the MIT License.

## Contact

For inquiries, collaboration, or more information, please reach out via LinkedIn or email.
