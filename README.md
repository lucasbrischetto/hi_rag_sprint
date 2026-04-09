# hi_rag_sprint
Small rag application that answers questions over pdf's. Add files to /files and the application creates a vectorstore of the contents.

## Acknowledgements
This application is based on the self-RAG implementation from 
[NirDiamant/RAG_Techniques](https://github.com/NirDiamant/RAG_TECHNIQUES), 
adapted to work with a custom document set. The core self-RAG pipeline 
(retrieval decision, relevance grading, generation, hallucination checking, 
and utility scoring) follows the original implementation closely, with 
modifications including:

- Multi-document PDF loading with metadata preservation
- Persistent vectorstore with automatic change detection
- Source citation in responses
- Restricted to document-grounded answers only
