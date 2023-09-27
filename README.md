# HuggingChatAPI Wrapper (HCA) 🚀
Langchain custom LLM wrapper based on hugging-chat-api



## Introduction

HCA is a Python wrapper for the HuggingChatAPI library, designed to supercharge your AI projects! It's your ticket to democratizing AI, making cutting-edge language models accessible to everyone. 🌍✨


## Installation 🛠️

Getting started with HCA is a breeze! Just follow these steps:

1. Install the required libraries: `pip install -U hugchat langchain`

2. Grab your HuggingFace credentials:
- Sign up or log in to [HuggingFace](https://huggingface.co/).
- You'll need your email and password or a valid cookie file for authentication. 🛡️

## Usage 💬

### Basic Usage 🚀

Here's how you can effortlessly unleash the power of HCA:

#### Example 1: Using email and password 📧🔑

```python
from HCA import HCA

llm = HCA(email="YOUR_EMAIL", password="YOUR_PASSWORD")
response = llm("Hello, how are you?")
print(response)
```

#### Example 2: Using a cookie file 🍪

```python
llm = HCA(cookie_path="YOUR_COOKIE_PATH")
response = llm("Hello, how are you?")
print(response)
```

#### Advanced Usage 🌟
Customize your AI adventures with a myriad of options when creating an HCA instance:

```python
llm = HCA(
    email="YOUR_EMAIL",
    password="YOUR_PASSWORD",
    log=True,
    model=1,
    temperature=0.9,
    top_p=0.95,
    repetition_penalty=1.2,
    top_k=50,
    truncate=1024,
    watermark=False,
    max_new_tokens=1024,
    stop=["</s>"],
    return_full_text=False,
    stream=True,
    use_cache=False,
    is_retry=False,
    retry_count=5
)
response = llm("Hello, how are you?")
print(response)
```


#### Interactive Usage 🤖🗣️
Experience the magic of AI in real-time! Engage in a lively conversation with the chatbot:

```python
from HCA import HCA

llm = HCA(email="YOUR_EMAIL", password="YOUR_PASSWORD", log=True, model=1)

txt = input("\n\nYou (write 'exit' for stop): ")
while txt != "exit":
    print("Bot : " + llm(txt)+ "\n")
    #print("Avg response time : " + str(llm._get_avg_response_time))
    txt = input("You : ")

```

## Contributing 🤝
Passionate about democratizing AI? Join the revolution! Contributions to this project are more than welcome! If you find any issues or have dazzling ideas for improvements, please open an issue or submit a pull request. Together, we'll change the AI landscape! 🌟🌐

##License 📜
Let's democratize AI with open-source spirit! 🤗🌈


Feel free to adjust the emojis or text further to match your enthusiasm and vision for democratizing AI. It's all about showcasing your passion and excitement! 🚀✨🌟🤖🌈🤗🌍💡

