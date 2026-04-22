# ai-customer-service-agent
ai-customer-service-agent
E-Commerce Customer Service & Data Analysis AI Agent

An intelligent customer service system based on **LLM + MCP (Model Context Protocol) + Database Query**, supporting order inquiry, logistics tracking, after-sales service, and business data analysis.

---

## 🚀 Project Overview

This project builds an AI-powered customer service system for e-commerce scenarios, integrating:

- 🤖 Large Language Model (LLM)
- 🔧 MCP Tool Invocation
- 🗄️ MySQL Database
- 📱 Frontend (Mini Program / Vue)

It implements a full workflow:


User Input → AI Decision → Tool Invocation → Database Query → Response Generation


---

## 🧩 Core Features

### 1️⃣ Customer Service Capabilities
- Order query (by username / order ID)
- Logistics tracking
- Product information query
- User purchase history

### 2️⃣ After-Sales Services
- Return policy
- Exchange policy
- Refund process
- Damaged goods handling

### 3️⃣ Human Support Escalation
- Create support tickets
- Query ticket status
- Fallback to human service

### 4️⃣ Data Analysis Capabilities
- Product sales ranking
- Customer purchase frequency
- Order status distribution
- User consumption analysis

---

## 🏗️ System Architecture


User (Frontend)
↓
AI Agent (LLM)
↓
MCP Tool Layer
↓
MySQL Database


---

## 📁 Project Structure

```bash
ai-customer-service-agent/
├── frontend/        # Frontend (Mini Program / Vue)
├── backend/         # Backend API (Django / FastAPI)
├── mcp/             # MCP Server (Tool Layer)
├── sql/             # Database Initialization Scripts
└── README.md
⚙️ Tech Stack
Frontend: Vue / uni-app / Mini Program
Backend: Python (Django / FastAPI)
Database: MySQL 5.7
AI Agent: LLM (with tool-calling capability)
Protocol: MCP (Model Context Protocol)
🔧 MCP Tools

The system provides the following tools via MCP:

get_data_base(sql)
→ Execute SQL queries (orders, users, products, etc.)
get_after_sales_policy(type)
→ Retrieve after-sales policies
create_human_service_ticket(...)
→ Create a customer support ticket
query_human_service_ticket(id)
→ Query ticket status
📊 Example Workflow
User Input
Check the orders of user Zhang Wei
System Behavior
Generate SQL query automatically
Call MCP tool
Query database
Return structured natural language response
📱 Frontend UI
Chat-style interaction (similar to messaging apps)
Auto-scroll conversation
Markdown rendering support
Customer service style UI
Responsive design for mobile devices
🧠 Highlights
✅ LLM + Tool Calling (not just chatbot)
✅ Data-driven responses (real database queries)
✅ Customer service + Data analysis integration
✅ Full after-sales workflow (AI + human fallback)
✅ Scalable architecture (easy to extend tools)
⚠️ Notes
This project is for learning and demonstration purposes
The MCP database tool currently has full permissions (not safe for production)
Local deployment requires database and backend setup
📌 Future Improvements
Integrate real LLM APIs (OpenAI / DeepSeek / etc.)
Add multi-turn conversation memory
Improve SQL generation accuracy
Deploy to cloud server
Publish as real mini-program
👨‍💻 Author
Undergraduate AI Project
Focused on practical application and system design
⭐ If you like this project

Feel free to Star ⭐ the repository!
