# Developer’s Diary – AI Collaboration Guide

This diary documents the development of a Smart Finance Assistant using AI tools. It shows how AI was used to design, build, test, and improve the system. Each entry includes the artifact, context, improvements, and reflection.

---

# Foundation Skills Examples

---

## Entry 1 – Designing the Finance Problem
**Artifact:** ChatGPT brainstorming conversation

**Context:** Defining a clear problem for the project.

**My Prompt:**  
"Help me brainstorm personal finance problems that can be solved using CSV transaction analysis."

**AI Response Summary:**  
AI suggested budgeting, spending tracking, savings, and travel expense management.

**My Critique/Improvement:**  
I narrowed the focus to travel finance and currency conversion.

**Result:**  
A clear project idea focused on helping travellers manage expenses in different currencies.

**Reflection:**  
AI helped generate ideas quickly, but I needed to refine the scope to make the project focused and realistic.

---

## Entry 2 – Designing Data Inputs and Outputs
**Artifact:** AI system design response

**Context:** Defining system inputs and outputs.

**My Prompt:**  
"For a travel finance assistant, what inputs and outputs should I include?"

**AI Response Summary:**  
Suggested transaction data, exchange rates, and financial summaries.

**My Improvement:**  
I refined outputs to match assignment requirements.

**Result:**  
Inputs: CSV transactions, exchange rates, user preferences  
Outputs: spending analysis, insights, currency conversion, recommendations

**Reflection:**  
Clear inputs and outputs helped structure the entire system.

---

# Data Processing and Analysis Development

---

## Entry 3 – Building the Data Cleaning Function
**Artifact:** load_and_clean_transaction_data function

**Context:** Cleaning raw financial data.

**My Prompt:**  
"Write a pandas function to clean CSV financial data with dollar signs and missing values."

**AI Response Summary:**  
Basic cleaning logic for numeric conversion.

**My Critique/Improvement:**  
I added validation, error handling, and removal of invalid rows.

**Result:**  
A reliable data cleaning function for financial datasets.

**Reflection:**  
I learned that real-world data is messy and must always be cleaned before analysis.

---

## Entry 4 – Building Spending Analysis Engine
**Artifact:** analyze_spending_patterns function

**Context:** Creating financial insights from transactions.

**My Prompt:**  
"How do I calculate spending by category and generate insights?"

**AI Response Summary:**  
Suggested grouping and aggregation.

**My Improvement:**  
I added:
- percentage calculations  
- refund handling  
- better insight generation  
- edge case handling  

**Result:**  
A full spending analysis system that produces meaningful insights.

**Reflection:**  
I learned that analysis is not just about numbers. It is about turning data into useful information that people can understand and act on.

---

# Recommendation and Intelligence Layer

---

## Entry 5 – Financial Recommendation System
**Artifact:** generate_financial_recommendations function

**Context:** Turning analysis into advice.

**My Prompt:**  
"Generate financial recommendations based on spending data."

**AI Response Summary:**  
Provided general savings suggestions.

**My Critique/Improvement:**  
I improved structure and added:
- category-based insights  
- percentage-based reasoning  
- actionable advice sections  

**Result:**  
A structured financial recommendation report.

**Reflection:**  
I learned that insights are more valuable than raw analysis. Users need clear actions they can follow, not just numbers or statistics.

---

## Entry 6 – Simple RAG System
**Artifact:** retrieve_documents function

**Context:** Adding knowledge retrieval to the system.

**My Prompt:**  
"How can I retrieve relevant financial advice based on user questions?"

**AI Response Summary:**  
Suggested keyword matching.

**My Improvement:**  
I built a structured document system and retrieval logic.

**Result:**  
A simple retrieval system for financial knowledge.

**Reflection:**  
This introduced me to how AI systems combine data analysis with external knowledge to improve responses.

---

# Agent-Based System Development

---

## Entry 7 – Finance Agent Architecture
**Artifact:** FinanceAgent class

**Context:** Building a tool-based AI system.

**My Prompt:**  
"Create a simple AI agent that can register and use tools."

**AI Response Summary:**  
Basic tool registry design.

**My Improvement:**  
I added:
- structured tool storage  
- error handling  
- reusable architecture  

**Result:**  
A working agent system that can run multiple financial tools.

**Reflection:**  
I learned how AI agents work by using tools instead of doing everything in one function. This makes systems more flexible and scalable.

---

## Entry 8 – Savings Calculator Tool
**Artifact:** savings_calculator function

**Context:** Adding financial planning features.

**My Prompt:**  
"Create a function that calculates how long it takes to reach a savings goal."

**AI Response Summary:**  
Provided basic calculation formula.

**My Improvement:**  
I added input validation and improved output formatting.

**Result:**  
A savings tool that estimates time to reach financial goals.

**Reflection:**  
Breaking complex financial problems into tools makes the system easier to expand and maintain.

---

# Chatbot and Personality Layer

---

## Entry 9 – Finny Chatbot Personality
**Artifact:** system prompt

**Context:** Designing an AI financial assistant personality.

**My Prompt:**  
"Create a system prompt for a financial assistant chatbot."

**AI Response Summary:**  
Basic helpful assistant prompt.

**My Improvement:**  
I refined tone, focus, and limitations.

**Result:**  
A defined chatbot personality called Finny.

**Reflection:**  
The system prompt is very important because it controls how the AI behaves and communicates with users.

---

## Entry 10 – Chatbot and Data Integration
**Artifact:** ask_finny function

**Context:** Connecting chatbot with financial data.

**My Prompt:**  
"How do I pass financial analysis data into a chatbot?"

**AI Response Summary:**  
Suggested combining context with user input.

**My Improvement:**  
I structured the financial data into readable context before sending it to the chatbot.

**Result:**  
A chatbot that responds using real financial data.

**Reflection:**  
Adding context makes the chatbot more intelligent and personalised.

---

# UI Development

---

## Entry 11 – Currency Converter Interface
**Artifact:** Gradio UI

**Context:** Building a user interface for currency conversion.

**My Prompt:**  
"Create a Gradio interface for a currency converter."

**AI Response Summary:**  
Basic UI with inputs and output.

**My Improvement:**  
I added validation, formatting, and error handling.

**Result:**  
A working and user-friendly web interface.

**Reflection:**  
A good interface is important because it makes complex systems easy for users to interact with.

---

## Entry 12 – Full System Integration
**Artifact:** Complete project pipeline

**Context:** Connecting all components into one system.

**Work Completed:**
- Data cleaning  
- Spending analysis  
- Recommendation engine  
- RAG retrieval system  
- AI agent tools  
- Chatbot integration  
- Gradio interface  

**Reflection:**  
The main challenge was making all parts work together. AI helped build individual components, but I had to ensure they were connected properly and produced consistent results.

---

# AI Collaboration Best Practices

---

## Prompting Improvements
- Always include business context
- Clearly define inputs and outputs
- Specify desired format and audience
- Ask for explanations, not just code

---

## Evaluation Questions
- Does this work with real messy data?
- Can a non-technical user understand it?
- Does it provide useful actions or just information?
- Can it scale to larger datasets?

---

## Development Process
1. Generate initial AI solution  
2. Test with real data  
3. Identify problems  
4. Refine prompts  
5. Improve structure and usability  

---

# Key Learning

Throughout this project, I learned that building systems with AI is not just about asking for code. It is about learning how to guide AI properly so it produces useful and reliable results.

At the start, I thought AI could directly build complete solutions. However, I realised that the quality of output depends heavily on how I communicate the problem. When I gave vague prompts, the results were basic and not very useful. When I added context, structure, and clear requirements, the AI produced much better and more professional solutions.

I also learned that development is an iterative process. I rarely got the final solution on the first attempt. Instead, I had to test the code, find problems, and then improve my prompts or adjust the logic. This cycle of generating, testing, and refining was important for building a working system.

Another key learning was understanding real-world data issues. Financial data is not clean or perfect. It can include missing values, incorrect formats, refunds, and unexpected inputs. I had to design my system to handle these cases, which made it more realistic and reliable.

I also learned how different parts of an AI system work together. My project included data processing, analysis, recommendations, retrieval systems, AI agents, and a chatbot. Each part had a different role, but they all needed to work together to create a complete system. This helped me understand how real AI applications are built in layers.

Finally, I learned that AI is a tool that supports development, not a replacement for thinking. It can generate ideas, code, and suggestions, but I still need to evaluate, improve, and connect everything logically. The most important skill is not just using AI, but knowing how to guide it effectively to solve real problems.
