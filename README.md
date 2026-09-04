# bharat-mind-2.0
BharatMind - AI-powered Business Intelligence and Decision Operating System for Indian MSMEs
# 🚀 BharatMind

### AI-Powered Business Intelligence & Decision Operating System for Indian MSMEs

> **From business data to intelligence to decisions.**

BharatMind is an AI-powered business intelligence platform designed for Indian MSMEs.

It connects with a business's existing data, understands the underlying business structure, analyzes performance, researches markets, identifies risks and opportunities, and helps business owners make faster, data-driven decisions.

---

## 🎯 The Problem

Indian MSMEs generate large amounts of business data across spreadsheets, accounting systems, ERP software, sales systems, inventory records and other tools.

The problem is not a lack of data.

The problem is turning that data into **clear business decisions**.

Business owners often have to:

- Manually analyze spreadsheets
- Switch between multiple business tools
- Search the web for market information
- Build reports manually
- Identify trends themselves
- Understand why revenue or margins changed
- Decide what action to take next

This creates a gap between:

**Data → Understanding → Decision → Action**

BharatMind is built to close that gap.

---

# 💡 Our Solution

BharatMind creates an intelligent business workspace around the user's data.

### The core workflow

```text
Business Data
     ↓
Data Ingestion
     ↓
Schema & Business Understanding
     ↓
Business Intelligence
     ↓
AI Research
     ↓
Forecast & Scenario Analysis
     ↓
Recommendations & Decisions

Instead of simply showing dashboards, BharatMind attempts to answer:

"What is happening in my business, why is it happening, and what should I do next?"

✨ Key Features
1. 🧠 AI Business Assistant

A business-focused AI research and decision assistant.

Users can ask questions about:

Revenue
Profitability
Customers
Products
Sales
Inventory
Competitors
Markets
Pricing
Industry trends
Business strategy
Growth opportunities

The assistant can combine business data with external research when available.

Example
"Why did my revenue decline?"

"What are my highest-performing products?"

"Who are my major competitors?"

"What market opportunities should I explore?"

"Analyze this industry and suggest a 90-day strategy."
2. 📊 Business Centre

A centralized business intelligence workspace.

It can surface relevant metrics such as:

Revenue
Costs
Gross profit
Margins
Sales trends
Product performance
Customer performance
Business growth

The system is designed to adapt to the type of data provided rather than assuming every business has the same schema.

3. 📥 Intelligent Data Ingestion

Users can upload business files such as:

Excel
CSV
Business reports
Financial data
Sales data
Product data
Customer data
Operational datasets

BharatMind analyzes the structure of the uploaded data before deciding which business metrics and insights are actually valid.

Important principle

The platform should not invent metrics that are not supported by the uploaded dataset.

For example:

If a dataset contains financial statements but no customer-level transactions, BharatMind should not pretend that customer transactions exist.

4. 🔮 Forecast & Strategic Decisions

Where sufficient time-series data exists, BharatMind can analyze historical trends and support:

Forecasting
Scenario analysis
Trend analysis
Risk identification
Decision support
Strategic recommendations

Forecasts are only shown when the underlying dataset contains sufficient relevant information.

5. 🌐 Industry Intelligence

Businesses can research their external environment.

The platform can organize intelligence around:

Industries
Markets
Competitors
Companies
Business trends
Government policies
Opportunities
Risks

The goal is to connect:

Internal Business Data
        +
External Market Intelligence
        ↓
Better Business Decisions
6. 🔍 AI-Powered Research

BharatMind is designed to provide research-oriented answers rather than simple chatbot responses.

Research can involve:

Multi-step queries
Web research
Source collection
Evidence analysis
Competitor research
Market research
Company analysis
Strategic analysis

Research outputs are designed to distinguish between:

Facts
Analysis
Inferences
Scenarios
Risks
🏗️ Architecture
                    ┌─────────────────────┐
                    │     BharatMind UI   │
                    │   Web Application   │
                    └──────────┬──────────┘
                               │
                               ↓
                    ┌─────────────────────┐
                    │ Application Backend │
                    └──────────┬──────────┘
                               │
             ┌─────────────────┼─────────────────┐
             ↓                 ↓                 ↓
       ┌───────────┐     ┌────────────┐    ┌──────────────┐
       │ Supabase  │     │ Gemini AI  │    │ Web Research │
       │           │     │            │    │ / Grounding  │
       └─────┬─────┘     └─────┬──────┘    └──────┬───────┘
             │                 │                  │
             └─────────────────┼──────────────────┘
                               ↓
                    ┌─────────────────────┐
                    │ Business Intelligence│
                    │ & Decision Engine    │
                    └─────────────────────┘
🧠 AI Architecture

BharatMind uses AI as a reasoning and decision layer over business information.

High-level pipeline
User Query
    ↓
Query Understanding
    ↓
Context Detection
    ↓
Business Data Retrieval
    ↓
External Research (when required)
    ↓
Evidence / Data Analysis
    ↓
Reasoning
    ↓
Structured Response
    ↓
Recommendation / Decision Support

The system is designed to keep the user's current business workspace as the primary context for business-related questions.

🔐 Authentication & Data Isolation

BharatMind uses a workspace-oriented architecture.

User
 ↓
Workspace
 ↓
Business Files
 ↓
Processed Business Data
 ↓
AI Context

Each workspace is intended to keep its business information isolated from other users and workspaces.

Supabase is used for authentication, database and storage infrastructure.

🗂️ Business Data Model

BharatMind is designed around flexible business data rather than one fixed industry schema.

Potential data domains include:

Sales
Products
Customers
Inventory
Expenses
Suppliers
Orders
Payments
Financial Statements
Business Segments
Operational Data

The platform first attempts to understand what information is actually present.

🏪 Industry Adaptability

BharatMind is designed for different types of businesses, including:

Retail
Trading
Manufacturing
Services
E-commerce
Other MSMEs

The interface and insights should adapt to the available business data instead of forcing every business into the same dashboard.

🧪 Example

Consider a business uploading an Excel file containing sales data.

BharatMind can transform:

Raw Excel
    ↓
Schema Detection
    ↓
Revenue / Cost Mapping
    ↓
Business Metrics
    ↓
Trend Analysis
    ↓
AI Interpretation
    ↓
Recommended Actions

The user can then ask:

"Which products are driving growth?"

or:

"What should I focus on next month?"

🎯 What Makes BharatMind Different?

Traditional BI tools generally answer:

"What happened?"

BharatMind aims to go further:

What happened?
      ↓
Why did it happen?
      ↓
What could happen next?
      ↓
What should I do?

The product combines:

Business Data + AI + Research + Forecasting + Decision Support

inside one business workspace.

🛠️ Technology Stack
Frontend
React / Next.js
Modern responsive UI
Component-based architecture
Backend
Node.js / application API layer
Server-side AI integration
Database & Authentication
Supabase
PostgreSQL
Supabase Auth
Supabase Storage
Row Level Security
AI
Google Gemini API
Gemini-powered reasoning
Web grounding / research capabilities
Data
Excel
CSV
Structured business datasets
🔑 Environment Variables

Create a .env file locally.

Example:

GEMINI_API_KEY=your_gemini_api_key

NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
NEXT_PUBLIC_SUPABASE_PUBLISHABLE_KEY=your_supabase_publishable_key

SUPABASE_SECRET_KEY=your_supabase_secret_key

Never commit .env or API keys to GitHub.

Use your project's actual environment-variable names if they differ from the example above.

🚀 Local Setup
1. Clone the repository
git clone https://github.com/YOUR_USERNAME/bharat-mind-2.0.git
cd bharat-mind-2.0
2. Install dependencies
npm install
3. Configure environment variables

Create:

.env.local

and add the required keys.

4. Start development server
npm run dev

Open:

http://localhost:3000
🧪 Testing

The application should be tested with different types of business datasets.

Example:

Dataset A
→ Sales dataset
→ Sales/business metrics

Dataset B
→ Financial statement
→ Financial metrics

Dataset C
→ Product/inventory dataset
→ Inventory/product insights

The system should not assume that every uploaded file represents the same business structure.

🛡️ Data Integrity Principles

BharatMind follows several important principles:

No fabricated business metrics

If the uploaded dataset does not contain a metric, the system should communicate that it is unavailable.

No fabricated sources

External research should use actual sources when available.

Dataset-aware analytics

Analytics should depend on the actual structure and quality of the uploaded data.

Workspace isolation

Business information should remain scoped to the correct user/workspace.

🏆 Built for the Razorpay Buildathon

BharatMind is submitted under the Open Track.

The product focuses on using AI to solve a practical business problem:

Helping businesses turn fragmented business information into actionable intelligence and decisions.

The goal is not to replace existing business software.

Instead, BharatMind acts as an intelligent layer across the information a business already has.

👥 Team

BharatMind

Built for the Razorpay Buildathon 2026.

📌 Project Status

🚧 Hackathon / Prototype

The platform is actively being developed and tested.

Some integrations and capabilities may still be under development.
