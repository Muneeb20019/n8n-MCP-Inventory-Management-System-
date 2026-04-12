# 📦 Inventory-Management-Automation-n8n

![n8n](https://img.shields.io/badge/Workflow-n8n-FF6C37?style=flat&logo=n8n&logoColor=white)
![OpenRouter](https://img.shields.io/badge/AI-OpenRouter-blue?style=flat)
![MCP](https://img.shields.io/badge/Protocol-MCP-yellow?style=flat)
![Google Sheets](https://img.shields.io/badge/Database-Google_Sheets-34A853?style=flat&logo=googlesheets&logoColor=white)
![Memory](https://img.shields.io/badge/Logic-Simple_Memory-lightgrey?style=flat)

---

## 🚀 The Solution: Autonomous Supply Chain Concierge
Managing complex inventories often requires technical expertise in SQL or advanced spreadsheet formulas. This project is an **Advanced AI-Driven Inventory Engine** that democratizes data management. By bridging **n8n orchestration** with the **Model Context Protocol (MCP)**, it transforms a standard Google Sheet into a "Headless Database" that can be managed entirely through natural language.

The system acts as an **Autonomous Inventory Manager**: it understands conversational requests like *"Add 50 units of Chocolate Bar"* or *"What is our current stock for P008?"*, performs real-time calculations, manages unique ID generation, and ensures database integrity—all without the user ever opening a spreadsheet. 🤖📊✨

---

## 🖼️ System Visualization

### 🛠️ Workflow Orchestration (The MCP Pipeline)
The master blueprint featuring the AI Agent, MCP Tooling, and the Google Sheets integration layer.
<div align="center">
  <img src="https://raw.githubusercontent.com/Muneeb20019/Inventory-Management-Automation-n8n/main/MCP%20Inventory.png" width="100%" alt="n8n Inventory Workflow Architecture" style="border-radius:10px; box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);"/>
  <p><i>Figure 1: The n8n automation architecture featuring the AI Agent and MCP Trigger.</i></p>
</div>

### 📊 Persistent Database (Google Sheets)
The 'Inventory Management Sheet' is updated in real-time by the AI Agent, handling IDs and price math automatically.
<div align="center">
  <img src="https://raw.githubusercontent.com/Muneeb20019/Inventory-Management-Automation-n8n/main/Inventory%20Management%20Sheet.png" width="100%" alt="Inventory Management Google Sheet" style="border-radius:10px; box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);"/>
  <p><i>Figure 2: Real-time inventory records managed via autonomous AI logic.</i></p>
</div>

---

## 📊 Business Impact & Engineering Outcomes
This system is engineered to move inventory management from manual entry to intelligent automation:

*   **⚡ Conversational Efficiency:** Eliminates the need for manual data filtering. Users interact with the database as if they were talking to a human manager.
*   **📉 100% Data Consistency:** Automatically calculates **Total Price (Quantity * Unit Price)**, preventing human calculation errors.
*   **🧠 Session-Aware Intelligence:** Uses **Simple Memory** to maintain context, allowing users to refer to "the previous order" without repeating IDs.
*   **🛠️ Scalable ID Orchestration:** Dynamically generates unique **Order IDs (ORD-)** and **Product IDs (P-)**, ensuring a perfectly structured system.

---

## ✅ Problems Solved
- **🛑 Manual Entry Friction:** No more hunting for the right row; the AI Agent navigates the spreadsheet for you. 📂
- **🛑 Broken Formula Logic:** Moving calculations into the n8n layer prevents accidental spreadsheet formula deletions. 🎯
- **🛑 Technical Barriers:** Allows non-technical staff to perform complex database CRUD operations via simple chat messages. 📈

---

## 🧠 Core Technical Pillars

### 1. 🤖 Model Context Protocol (MCP) Integration
Using **MCP**, I have given the AI Agent a specific "skill set" for inventory management. Instead of just talking, the agent can trigger specific sub-workflows (`get_order`, `update_order`, `add_order`) based on user intent.

### 2. 🧠 Relational Memory & Reasoning (OpenRouter)
Powered by **Gemini/Claude** via **OpenRouter**, the agent performs high-level reasoning. It uses a **Simple Memory** node to retain session data, ensuring the conversation feels natural.

### 3. 🔢 Dynamic Data Synthesis (JavaScript Node)
- **Auto-Calculations:** Handles math for Quantities and Prices server-side to ensure accuracy.
- **Smart ID Generation:** Creates unique IDs using a combination of prefixes and Unix timestamps. 🏗️✨

### 4. 🗄️ Google Sheets as a Headless Database
The system treats **Google Sheets** as a robust backend. The workflow uses advanced filtering logic to find specific Product IDs and updates only the necessary rows. 📡🚀

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
