### Install ollama

- download from https://ollama.com/download/mac
- install
- run ollama run llama3.2
- ollama list
- test with curl

```
curl http://127.0.0.1:11434/v1/chat/completions \
    -H "Content-Type: application/json" \
    -d '{
        "model": "llama3.2",
        "messages": [
            {
                "role": "system",
                "content": "You are a helpful assistant."
            },
            {
                "role": "user",
                "content": "Hello! Who are you?"
            }
        ]
    }'


```

### run streamlit

- cd simple-rag
- create virtual environment
- enable environment
- pip install langchain streamlit streamlit_chat langchain_community pypdf fastembed chromadb
- streamlit run app.py
- upload pdf
- ถามเลย
