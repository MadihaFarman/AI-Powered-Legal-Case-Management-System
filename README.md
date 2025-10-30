## AI Powered Legal Case Management System


There are a lot of cases waiting to be heard in Pakistan, and the large number of unstructured court documents makes it hard for lawyers, judges, and researchers to work
with them quickly. These papers are often long and complicated, which makes it hard
to find important information or figure out which cases need to be looked at right away.
To fix this, we made the AI-Powered Legal Case Management System during the AI
Techathon 2025. The system uses machine learning, natural language processing, and
retrieval-augmented generation (RAG) to better organize, prioritize, and find knowledge
based on past cases.

We made our solution by focusing on three main tasks: classifying, prioritizing, and
using a RAG-based app to do smart legal searches. We taught models how to sort
Supreme Court decisions into three groups: Criminal, Constitutional, and Civil. The
model was right 93.

The RAG part made the system more dynamic by letting it give answers based on
what has happened before instead of just making predictions. We turned legal judgments
into dense vectors and saved them in ChromaDB using Hugging Face embeddings (allMiniLM-L6-v2). Then, GROQ’s LLM API (llama-3.1-8b-instant) was used to answer
user questions in context. Retrieval always got more than 80
There were problems. A lot of work had to be done on the Kaggle dataset before it
could be used, including AI-assisted labeling. The prioritization data was a little uneven,
especially in the Low-priority class, which had a small effect on performance. Also, the
fact that there aren’t many labeled legal datasets in Pakistan makes it hard to use them
on a large scale. The classification and prioritization tasks still worked well, and the RAG
system gave clear, relevant answers based on past cases.

This project shows how AI could change the way the law works. Lawyers and clerks
can save time by automating classification and prioritization. RAG, on the other hand,
makes it easier to find precedent knowledge and cuts down on manual search. As datasets
grow and LLMs get better, the system could become a very useful tool for Pakistan’s
courts. The project shows how modern NLP techniques can help solve one of Pakistan’s
biggest problems: making the justice system work better.
