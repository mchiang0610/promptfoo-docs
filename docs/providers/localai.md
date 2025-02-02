---
sidebar_label: LocalAI (Llama, Alpaca, GPT4All, ...)
sidebar_position: 99
---

# Local AI

LocalAI is an API wrapper for open-source LLMs that is compatible with OpenAI. You can run LocalAI for compatibility with Llama, Alpaca, Vicuna, GPT4All, RedPajama, and many other models compatible with the ggml format.

View all compatible models [here](https://github.com/go-skynet/LocalAI#model-compatibility-table).

Once you have LocalAI up and running, specify one of the following based on the model you have selected:

- `localai:chat:<model name>`
- `localai:completion:<model name>`
- `localai:<model name>` - defaults to chat-type model

The model name is typically the filename of the .bin file that you downloaded to set up the model in LocalAI. For example, `ggml-vic13b-uncensored-q5_1.bin`

Supported environment variables:

- `LOCALAI_BASE_URL` - defaults to `http://localhost:8080/v1`
- `REQUEST_TIMEOUT_MS` - maximum request time, in milliseconds. Defaults to 60000.

