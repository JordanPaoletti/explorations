# Notes on Running Local LLMs

## Ollama

Ollama is a tool for running LLMs locally

### Reference Links
* [Ollama](https://github.com/jmorganca/ollama)
* [Ollama Docker](https://hub.docker.com/r/ollama/ollama)
* [Article on fine-tuning Mixtral 8x7b](https://scalastic.io/en/mixtral-ollama-llamaindex-llm/#installing-mixtral-8x7b)

### Usage via Docker

Start the container
```bash
docker run -d --gpus=all -v ollama:/root/.ollama -p 11434:11434 --name ollama ollama/ollama:latest
```

Run a model
```bash
docker exec -it ollama ollama run llama2
```
