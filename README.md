# 📦 Inventory-Management-Automation-n8n

![n8n](https://img.shields.io/badge/Workflow-n8n-FF6C37?style=flat&logo=n8n&logoColor=white)
![OpenRouter](https://img.shields.io/badge/AI-OpenRouter-blue?style=flat)
![MCP](https://img.shields.io/badge/Protocol-MCP-yellow?style=flat)
![Google Sheets](https://img.shields.io/badge/Database-Google_Sheets-34A853?style=flat&logo=googlesheets&logoColor=white)
![Memory](https://img.shields.io/badge/Logic-Simple_Memory-lightgrey?style=flat)

---

## 🚀 The Solution: Autonomous Supply Chain Concierge
Managing complex inventories often requires technical expertise in SQL or advanced spreadsheet formulas. This project is an **Advanced AI-Driven Inventory Engine** that democratizes data management. By bridging **n8n orchestration** with the **Model Context Protocol (MCP)**, it transforms a standard Google Sheet into a "Headless Database" that can be managed entirely through natural language.

The system acts as an **Autonomous Inventory Manager**: it understands conversational requests like *"Add 50 units of Chocolate Bar"* or *"What is our current stock for P008?"*, performs real-time calculations, manages unique ID generation, and ensures database integrity—all without the user ever needing to manually edit a cell. 🤖📊✨

---

## 📊 Business Impact & Engineering Outcomes
This system is engineered to move inventory management from manual entry to intelligent automation:

*   **⚡ Conversational Efficiency:** Eliminates the need for manual data filtering or complex VLOOKUPs. Users interact with the database as if they were talking to a human manager.
*   **📉 100% Data Consistency:** Automatically calculates **Total Price (Quantity * Unit Price)** and enforces strict data types, preventing human calculation errors.
*   **🧠 Session-Aware Intelligence:** Uses **Simple Memory** to maintain context, allowing users to refer to "the previous order" or "that product" without repeating long IDs.
*   **🛠️ Scalable ID Orchestration:** Dynamically generates unique, timestamp-based **Order IDs (ORD-)** and **Product IDs (P-)**, ensuring a perfectly structured primary key system.

---

## ✅ Problems Solved
- **🛑 Manual Entry Friction:** No more hunting for the right row or column; the AI Agent navigates the spreadsheet architecture for you. 📧
- **🛑 Broken Formula Logic:** By moving calculations (Quantity * Price) into the n8n workflow layer, the system prevents accidental spreadsheet formula deletions. 🎯
- **🛑 Lack of Audit Trail:** Every interaction is processed through a structured logic gate, ensuring every "Add" or "Update" action is logged correctly. 📂
- **🛑 Technical Barriers:** Allows non-technical staff to perform complex database CRUD (Create, Read, Update, Delete) operations via simple chat messages. 📈

---

## 🖼️ System Architecture

### Workflow Orchestration (The MCP Pipeline)
The master blueprint featuring the AI Agent, MCP Tooling, and the Google Sheets integration layer.
<div align="center">
  <img src="https://raw.githubusercontent.com/Muneeb20019/n8n-MCP-Inventory-Management-System-/main/workflow_screenshot.png" width="100%" alt="n8n Inventory Workflow Architecture" style="border-radius:10px; box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);"/>
  <p><i>Full Agentic Orchestration featuring the AI Agent and MCP Trigger.</i></p>
</div>

---

## 🧠 Core Technical Pillars

### 1. 🤖 Model Context Protocol (MCP) Integration
This is the "Secret Sauce." Using **MCP**, I have given the AI Agent a specific "skill set" for inventory management. Instead of just talking, the agent can now "reach out" and trigger specific sub-workflows (`get_order`, `update_order`, `add_order`) based on the user's intent, effectively bridging the LLM to the database.

### 2. 🧠 Relational Memory & Reasoning (OpenRouter)
Powered by **Gemini/Claude** via **OpenRouter**, the agent performs high-level reasoning. It doesn't just execute commands; it validates them. It uses a **Simple Memory** node to retain session data, ensuring the conversation feels natural and the AI remembers which product you are currently discussing. 🧠🔍

### 3. 🔢 Dynamic Data Synthesis (JavaScript Node)
To maintain a professional database, the workflow includes a custom logic layer:
- **Auto-Calculations:** Handles math for Quantities, Unit Prices, and Totals server-side to ensure accuracy.
- **Smart ID Generation:** Creates unique, non-colliding IDs using a combination of prefixes and Unix timestamps, making the spreadsheet a true relational system. 🏗️✨

### 4. 🗄️ Google Sheets as a Headless Database
The system treats **Google Sheets** as a robust backend. The workflow uses advanced filtering logic to find specific Product IDs and updates only the necessary rows. This architecture allows the UI to be a simple chat bubble while the data stays organized in a professional spreadsheet. 📡🚀

---

## 🛠️ Technical Stack
| Layer | Technology |
| :--- | :--- |
| **🔄 Automation** | **n8n** (State Management & Tool Orchestration) |
| **🧠 AI Brain** | **OpenRouter (Gemini/Claude)** (Conversational Reasoning) |
| **🔌 Protocol** | **MCP (Model Context Protocol)** (AI-to-Tool Bridge) |
| **🗄️ Database** | **Google Sheets API** (Inventory Repository) |
| **💾 Memory** | **n8n Simple Memory** (Contextual Data Retention) |
| **📜 Scripting** | **JavaScript / JSON** (ID Generation & Math Logic) |

---

## ✍️ Author
**Muneeb Ali Khan**
- **GitHub:** [@Muneeb20019](https://github.com/Muneeb20019)
- **LinkedIn:** [Muneeb Ali Khan](https://www.linkedin.com/in/muneeb-ali-khan-2a1675365)

---

## 📜 License
This project is licensed under the MIT License.
