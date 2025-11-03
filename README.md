# AI Customer Service & Donation Agent

## 🎯 Project Objective

This project details the development of "SANAD," a **sophisticated** AI agent created for the Life Makers Charity. The primary goal is to automate client interactions, **streamline** the donation collection process, and provide **instantaneous**, accurate information to users engaging with the charity.

## ✨ Key Features

* **Intelligent Interaction:** The agent engages in **dynamic** conversations to guide users through the donation process and answer inquiries about the charity's activities.
* **Automated Tool Integration:**
    * **Systematically** logs customer data and transaction details into `Google Sheets`.
    * **Automatically** archives donation transfer receipts (images) to a specific `Google Drive` folder, tagging them with the client's name and transaction date for easy auditing.
* **Data Precision & Validation:** The agent is **meticulously** designed to ensure data **integrity**. It actively validates inputs and prompts the user for critical missing information (e.g., the "intention" of the donation) before **committing** the data to the database.

## 🛠️ Technical Architecture & Stack

* **RAG (Retrieval-Augmented Generation) with Reranking:**
    * The agent's core relies on a **RAG** pipeline to fetch information from a dedicated knowledge base, ensuring all responses are accurate and context-aware.
    * To achieve **utmost** (C1) precision and **mitigate** hallucinations, a **Reranking** module is implemented. This module filters and re-orders the retrieved documents to select only the most **pertinent** context before feeding it to the language model for a final answer.
* **Deployment & Infrastructure:**
    * The entire application is deployed on an **Amazon EC2 (VPS)** instance, ensuring **high availability** and **stable**, 24/7 operation.
* **Database:**
    * **PostgreSQL** serves as the primary database management system. It was chosen for its **robustness** and **efficiency** in handling the complex, structured data required for the agent's memory and logging.

## 🏁 Outcome

The result is a **fully integrated** and **autonomous** automation system. It provides a **seamless** support experience for clients and ensures **dependable**, accurate data management for the charity's operations.
