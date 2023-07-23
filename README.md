#  Fine-tune LLM for Wine Price Prediction

## Install via Docker

```bash

# setup
docker build --no-cache --tag llm-fine-tune-wine-price -f Dockerfile .

# run
docker run --gpus all -v /home/ubuntu/work/llm-fine-tune-wine-price/:/workspace/    -p 5555:5555 --rm  -it --shm-size=55gb -d llm-fine-tune-wine-price tail -f /dev/null

```

## Run demo app

```bash
streamlit run basic_app.py --server.port 5555 --server.enableCORS false
```
