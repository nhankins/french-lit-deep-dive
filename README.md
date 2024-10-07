# french-lit-deep-dive

# Goal: 
Using open-source LLMs to improve comprehension of advanced French literature for English learners (will look to expand for other languages).

# Solution: 
This repo should successfully detail how to use RAG and open-source LLMs available on Ollama using Langchain to read PDFs and Chroma DB as a retrieval database for the use case of language learning.

# Instructions to replicate:

1) git clone or download the files as a zip
   
2) Make a virtual environment (I used conda in VS Code and my local device is an M1 macbook) and run this command in the terminal: pip install -r requirements.txt

3) Run the cells in the notebook (ipynb) file and note that you may need to restart the kernel after pip installing some of the packages and the requirements.txt file

4) You need to have ollama running for this to work when you get to the "ollama pull" section

5) Know that you can change the string in the chain.invoke cells to prompt the LLM of your choosing with different questions to improve comprehension

# Quality Notes:

On data source: Used a merged pdf of 4 project gutenberg ebooks that were originally in ePUB format. ##
On embedding model: Used the same nomic embedding model used in the code from where the code template was retrieved (cited below as I did not write the code for this!) ##
On LLM: Used Aya 8B model given that the task is multilingual. Found that the larger model produced better results than the smaller stablelm2 model available on Ollama. 

# Sources:

The code template starting point and tutorial used as learning material/reference for this implementation was from this github repo and content creator: [https://github.com/tonykipkemboi/](https://github.com/tonykipkemboi/ollama_pdf_rag/tree/main)

