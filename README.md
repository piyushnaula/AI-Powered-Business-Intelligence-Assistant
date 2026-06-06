# AI-Powered Business Intelligence Assistant

# Week 1 Project Brief
### AI-Assisted Full Stack Web Development — Summer Internship Program
**Intern Name:** Piyush Naula
**Intern ID:** TBI-26100676
**Week:** 1 — Orientation & Project Setup
**Submission Due:** Sunday, 7 June 2026, 11:59 PM

---

## Q1. Briefly summarize the core tasks you completed for this week's module.

This week was focused on **orientation and project setup**. Here is what I completed:

**Project Idea Finalization**
I decided to build an **AI-Powered Business Intelligence Assistant for the Food Processing Industry**. The idea came from a real problem — food processing companies have lots of documents like production reports, audit reports, inventory records, and safety guidelines, but employees waste a lot of time searching through them manually. My project will solve this by letting users ask questions in simple language and get answers directly from their company documents.

**Problem Statement and Objectives**
I wrote a clear problem statement explaining why this project is needed. I also listed the main goals — like reducing document search time by 70%, improving decision-making, and supporting food safety compliance monitoring.

**Key Features Planning**
I planned all the major features of the project:
- Document upload and management system
- AI-powered chat assistant that answers questions based on uploaded documents
- Semantic search (search by meaning, not just keywords)
- Business Intelligence module covering production, inventory, quality control, and compliance
- A dashboard to show key stats and alerts

**Technology Stack Selection**
I finalized the full tech stack:
- **Frontend:** React.js + Tailwind CSS
- **Backend:** Python + FastAPI
- **AI Layer:** Google Gemini API + LangChain + HuggingFace Embeddings + RAG (Retrieval-Augmented Generation)
- **Databases:** PostgreSQL (for user data, metadata, chat history) + ChromaDB (for storing document embeddings for semantic search)
- **Deployment:** Docker + Vercel + Render

**High-Level System Design (HLD)**
I designed two main pipelines:
1. **Document Processing Pipeline** — Documents are uploaded → parsed → chunked → embedded → stored in ChromaDB
2. **Query Pipeline** — User asks a question → question is embedded → relevant document chunks are fetched from ChromaDB → Gemini LLM generates the final answer with source references

**Database Design**
I planned the database tables: Users, Documents, Production Reports, Inventory Records, Audit Reports, and Chat History.

**API Design**
I listed all the REST API endpoints needed for authentication, document management, chat, and business analytics.

**GitHub Repository Setup**
I created and initialized the GitHub repository for the project with a proper folder structure.

---

## Q2. What challenges or roadblocks did you face this week, and how did you handle them? (If Any)

**Challenge 1: Choosing the Right Domain**
At first, I was thinking of building a general-purpose document chatbot. But after reading the internship requirements carefully, I realized it needed to be tied to a real industry. I shifted my focus to the **Food Processing Industry**, which made the project much more meaningful and specific. This also helped me think of real-world use cases like compliance monitoring and production batch analysis.

**Challenge 2: Deciding Between AI APIs**
I was unsure whether to use OpenAI or Google Gemini API. After comparing cost, availability, and features, I chose **Google Gemini API** because it offers a free tier that is good for development, and it supports long-context responses which is useful for reading large business documents.

**Challenge 3: Designing the RAG Pipeline**
Understanding how RAG (Retrieval-Augmented Generation) works — especially the combination of ChromaDB for vector search and an LLM for answer generation — took some time. I studied LangChain documentation and a few tutorials to understand the flow clearly before planning my architecture.

---

## Q3. What extra steps or creative ideas did you explore this week beyond the basic module?

**Industry-Specific Focus**
Instead of building a generic chatbot, I specifically designed the system for the **Food Processing industry**. This means my Business Intelligence module has sections dedicated to food safety compliance tracking, audit report summarization, and defect trend analysis — things that are directly useful for real companies in this field.

**Dual Database Architecture**
I came up with the idea of using **two separate databases** — PostgreSQL for structured data (user info, metadata, chat history) and ChromaDB for unstructured document embeddings. This gives the system both traditional data management and modern vector search capabilities.

**Executive Summary API**
Beyond the basic analytics, I planned an extra API endpoint — `POST /api/v1/analytics/executive-summary` — that will generate an AI-written summary of overall business health for managers, combining production, inventory, quality, and compliance data together in one response.

**Future Enhancements Roadmap**
I also thought ahead and listed future features like:
- Voice-based assistant
- OCR support for scanned reports
- Multi-language support
- Predictive inventory forecasting
- ERP and warehouse system integration

These show that the project is designed with real scalability in mind, not just for the internship.

---

## Q4. Do you need any specific support, resources, or guidance from the team for next week?

As I move into **Week 2 (Frontend Foundations & UI Development)**, I would appreciate guidance on the following:

1. **UI Design References** — Any recommended design references or templates for dashboards built with React.js + Tailwind CSS for enterprise/B2B tools.
2. **Folder Structure Feedback** — A quick review of my planned frontend folder structure to make sure it follows best practices before I start coding.
3. **Clarification on Submission Format** — Should the Week 2 deliverable include a deployed link (Vercel), or just the GitHub repository with the frontend code?

---

## Submission Checklist

- [x] Project Brief document written
- [x] Problem Statement defined
- [x] Technology Stack finalized
- [x] High-Level System Design (HLD) completed
- [x] Database Design planned
- [x] API Design listed
- [x] GitHub Repository initialized
- [ ] PDF exported as `W1_ProjectBrief_[InternID].pdf`
- [ ] GitHub repository URL added to LMS submission
- [ ] ZIP archive created with all Week 1 files
- [ ] Posted on Cohort Introductions Forum
- [ ] Weekly Progress Report submitted on LMS Form by Sunday 11:59 PM IST

---

*AI-Assisted Full Stack Web Development Summer Internship — TBI-GEU*
