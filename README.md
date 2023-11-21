# PDF Query App
A user-friendly application built with Streamlit, converts PDFs into embeddings and store them for future querying. 
The app has two main functionalities: converting PDFs into embeddings and a separate interface for querying the stored embeddings. 
It uses Zephyr-7B for the LLM model and Stella for the embedding model and Chroma DB for the vector database.

## Features
- PDF to embedding conversion: Easily convert PDF documents into embeddings.
- Embedded storage: Store embeddings securely for efficient querying.
- Querying on stored embeddings: Utilize the separate interface to query the stored embeddings for specific information retrieval.

## Running Locally
install [ollama](https://ollama.ai/download)
and have it up and running with command ollama serve ( applicable to some systems only )  

download the required model ( this can be changed in this [line](https://github.com/Govind-S-B/pdf_query/blob/f80867040a419d2963b157d4e38c17676f2080aa/pages/query_pdf.py#L14C1-L15C1) )
```
ollama pull zephyr
```


clone the repo and move into the directory
```
git clone https://github.com/Govind-S-B/pdf_query.git
cd pdf_query
```
install the required python dependencies
```
pip install -r requirements.txt
```
run the streamlit app
```
streamlit run embed_pdf.py
```
