<div align="center"><img src="https://i.postimg.cc/Kv5hDh5q/Chat-GPT-Image-27-aug-2025-12-03-08.png" alt="Alt text" width="300"></div>

## What is this?

This is a simple price calculator for the language models provided by OpenRouter.

It fetches the latest language model list along with pricing details and more, and allows you to specify your expected number of input tokens, output tokens, and the number of API calls made.

For example, if you're using a 16 KB context length model with filled context (i.e. a typical long term chat scenario), you send 50 messages a day for a month, and are receiving replies on average about 1-2 paragraphs long each per query (about 500 tokens), you'd specify:

* Input Tokens: 16384 (16×1024)
* Output Tokens: 500
* API Call Count: 1500 (50×30)

You can sort the lists by price and include or exclude their completely free models.

It's all in a single page suitable for static hosting and the OpenRouter API call to fetch the latest model list does not require an API key.

Have fun! 🥳

## TODO

* Column (and sorting) by added date.
* Configurable thresholds for "cheap" (green), "average", "expensive" (orange) and filters for those categories.
* Exclude or higlight models that cannot satisfy input token count due to exceeding their context window.

## Demo

https://openrouter-calc.netlify.app
