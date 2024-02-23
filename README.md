# LLM chatbot runs locally   
This code once downloaded and packages installed, should allow you to run a large language model (llm) from your own computer.
Think of something similar to chatGPT running on your local machine, except you can choose which source material it uses to answer your questions by dropping file in the  
"source_documents" folder.  
Here, we have placed a pdf file of the famous philosophical text written by Ludwig Wittgenstein, the Tractatus Logico Philisophicus.  
Any other pdf, text, word document, power point, etc., file can be added or replaced here.   

Once the language model is downloaded from huggingface (see README in "models" dir), and langchain et al. installed (will go over install later), we can start reading our source file(s).  

### ingestion
Running in win cmd terminal  
  ```python ingest.py```  
  will start the language model reading through the files in "source_documents" dir and training itself on this material.
  After a few minutes, this process will have completed and we can ask the chatbot a question!  

  Once ingestion is complete you should see a terminal screen like so:  
  ![ingestion_comp](https://github.com/oliver-bigdata/local-llm-chatbot/blob/main/screenshots/ingestion_complete.png?raw=true)

### ask query  
Running in win cmd terminal  
```python run_query.py```  

will start loading the llm model, and its embeddings i.e. what it learned from reading our source material.  
We can now start asking it questions about WIttgenstein's philoshophy!   

### screenhots of answers  
it takes a while to answer questions, as expected on a CPU (a fast version requires a large memory GPU chip)  
But after a few minutes, we get our answers!  

![wittgenstein queryA](https://github.com/oliver-bigdata/local-llm-chatbot/blob/main/screenshots/wittgen.png?raw=true)  

![wittgenstein queryB](https://github.com/oliver-bigdata/local-llm-chatbot/blob/main/screenshots/wittgen%20query%20lion.png?raw=true)


## installation of packages  

  
