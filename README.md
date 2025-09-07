# 📚 CitePoint – Your AI-Powered Academic Research Assistant  

CitePoint is an AI-powered research assistant that helps students, academics, and professionals generate **comprehensive research papers, structured summaries, and academic insights** with ease.  

It integrates multiple intelligent agents, APIs, and a **Lovable-built frontend** to handle the entire research workflow — from topic extraction to writing polished academic drafts.  

---

## 🌐 Live Demo  

Try CitePoint here: [https://citepoint.lovable.app](https://citepoint.lovable.app)  

No setup required — just enter your research query and get started.  

---

## 🚀 Features  

### 🔹 Frontend (Lovable UI)  
- Clean, minimal interface for entering research queries.  
- One-click **“Start Research”** functionality.  
- Option to refine existing drafts with **custom user feedback**.  

---

### 🔹 Backend (Pipeline Workflow)  

1. **Webhook & Switch**  
   - Receives research queries from the frontend.  
   - Routes requests based on action:  
     - **Research** → Runs the full pipeline (Topic → Summarize → Organize → Write).  
     - **Refine** → Sends directly to Refinement Agent for updates.  

2. **Topic Extractor Agent**  
   - Analyzes the user’s query.  
   - Extracts main keywords and research focus areas.  
   - Ensures external searches remain **relevant and accurate**.  

3. **Tavily API Integration**  
   - Fetches supporting material from the web.  
   - Retrieves **latest research papers, articles, and academic resources**.  
   - Provides the **knowledge base** for summarization and drafting.  

4. **Summarizer Agent**  
   - Processes raw search results.  
   - Generates **concise summaries** for each retrieved document.  
   - Filters out irrelevant or low-value content.  
   - Uses **structured parsing** for consistent outputs.  

5. **Organizer Agent**  
   - Organizes multiple summaries into a **research paper outline**.  
   - Groups related insights into sections:  
     - **Introduction**  
     - **Literature Review**  
     - **Discussion**  
     - **Conclusion**  
   - Prepares the base structure for the Writer Agent.  

6. **Writer Agent**  
   - Expands the outline into a **full research paper draft**.  
   - Writes in a **professional, academic tone**.  
   - Preserves references and section structure.  

7. **Refinement Agent**  
   - Applies user-requested edits:  
     - Add / remove / restructure information.  
     - Adjust tone, formatting, or detail level.  
   - Returns an **updated draft for iterative improvements**.  

8. **Respond to Webhook**  
   - Sends the final draft (or refined version) back to the frontend.  

---

## ⚙️ Tech Stack  

- **Frontend**: Built with **Lovable** (no-code platform).  
- **Backend**: Agent-based pipeline with structured orchestration.  
- **Models**:  
  - Gemini-2.5-Flash → Topic Extraction  
  - GPT-4o-mini → Summarization, Organization 
  - GPT-4o → Writing, Refinement  
- **External API**: Tavily API (for real-time research material).  

---
