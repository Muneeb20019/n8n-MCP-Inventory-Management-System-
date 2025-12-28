# 📦 Smart Inventory Management System 🚀

An advanced, AI-driven automation workflow built with **n8n** and **MCP (Model Context Protocol)**. This system transforms an AI Agent into a powerful Inventory Manager capable of handling complex database operations on Google Sheets through simple natural language chat.

(https://github.com/Muneeb20019/n8n-MCP-Inventory-Management-System-/blob/main/MCP%20Inventory.png?raw=true)
*Figure 1: The n8n automation architecture featuring the AI Agent and MCP Trigger.*

## ✨ Features
*   **🤖 Intelligent AI Agent**: Leverages **OpenRouter** (Gemini/Claude) to interpret human requests like *"What's the stock for P008?"* or *"Add 50 units of Chocolate Bar."*
*   **📊 Dynamic Inventory Control**: Fully integrated with Google Sheets to manage `Order ID`, `Product ID`, `Quantity`, and `Pricing`.
*   **⚡ MCP Tooling**: Uses the Model Context Protocol to provide the AI with a specific "skill set" for Inventory Management.
*   **🧠 Contextual Memory**: Utilizes **Simple Memory** to remember Order IDs and previous interactions within a session.
*   **🔢 Automated Logic**: 
    *   **Auto-Calculations**: Automatically calculates `Total Price` based on `Quantity` * `Unit Price`.
    *   **Smart ID Generation**: Generates unique, timestamp-based `Order IDs` (ORD-) and `Product IDs` (P-) if they are not provided.

## 🚀 Technologies Used
*   **n8n**: Workflow automation platform.
*   **OpenRouter**: AI Model gateway for advanced reasoning.
*   **Google Sheets**: Serving as the real-time inventory database.
*   **MCP (Model Context Protocol)**: To bridge the AI Agent with custom workflow tools.
*   **Simple Memory**: For session-based data retention.

## 🖼️ Inventory Database
The system manages a structured database as shown below:

![Google Sheets Inventory](https://github.com/Muneeb20019/n8n-2/raw/main/inventory_sheet_screenshot.png)
*Figure 2: The 'Inventory Management Sheet' managed by the AI Agent.*

## ⚙️ How It Works
1.  **Chat Trigger**: The user interacts via a chat interface.
2.  **Reasoning**: The AI Agent identifies the intent (Read, Update, or Create).
3.  **MCP Routing**: The **MCP Client** routes the request to the **MCP Server Trigger**.
4.  **Database Action**: 
    *   **`get_order`**: Filters and retrieves specific row data.
    *   **`update_order`**: Matches the `Product ID` and updates stock or pricing.
    *   **`add_order`**: Appends a brand new row with generated IDs and calculated totals.
5.  **Response**: The agent confirms the action with a professional summary.

## 🛠️ Setup and Installation

### Prerequisites
*   An active n8n instance.
*   Google Sheets API credentials (OAuth2).
*   OpenRouter API Key.

### Steps
1.  **Clone this Repository**:
    ```bash
    git clone https://github.com/Muneeb20019/n8n-2.git
    ```
2.  **Import Workflow**:
    *   Import the `MCP_Inventory.json` file into your n8n editor.
3.  **Configure Environment**:
    *   Update the Google Sheets nodes with your specific **Sheet ID**.
    *   Add your **OpenRouter API Key** to the Chat Model node credentials.
4.  **Deployment**:
    *   Toggle the workflow to **Active**.

## ✍️ Author
**Muneeb Ali Khan**
*   [GitHub Profile](https://github.com/Muneeb20019)
*   [LinkedIn Profile](https://www.linkedin.com/in/muneeb-ali-khan-2a1675365)
