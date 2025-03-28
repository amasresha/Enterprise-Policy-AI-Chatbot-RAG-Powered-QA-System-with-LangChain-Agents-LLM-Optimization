# Enterprise Policy AI Chatbot: RAG-Powered QA System with LangChain Agents & LLM Optimization
## Architecture
![Agent Architecture Diagram](https://github.com/user-attachments/assets/948f4a36-ff32-40a6-8566-8785959f6bc2)

## Overview

An AI-powered assistant that combines RAG architecture with LangChain's agent framework to deliver precise HR policy answers. The system features:

- **Intelligent Routing**: Agent decides between document search and HR referral
- **Optimized Performance**: CPU-efficient TinyLlama implementation
- **Context-Aware**: Maintains conversation history for follow-up questions

## Key Features

### Agent-Centric Design
- 🧠 **ReAct Decision-Making**: Uses reasoning-action loops to select tools
- 🔧 **Two-Tool System**:
  - `PolicySearch`: Retrieves exact policy excerpts (RAG-powered)
  - `HR_Contact`: Fallback for complex/unanswered questions
- ⚖️ **Hallucination Prevention**: Constrained to only use authorized tools

### Technical Advantages
- 🚀 **Document Intelligence**: Processes PDFs, Word docs, and text files
- ⚡ **CPU Optimization**: 40% faster than baseline LLM implementations
- 🔄 **Stateful Conversations**: Remembers 5+ previous exchanges

## Technical Stack

| Component | Implementation Details |
|-----------|------------------------|
| **LLM** | TinyLlama-1.1B-Chat (quantized) |
| **Vector DB** | ChromaDB with all-MiniLM-L6-v2 embeddings |
| **Agent Framework** | LangChain 0.1.16 |
| **Query Processing** | Custom prompt templating |
| **Hardware** | CPU-only operation (tested on 4-core VM) |
