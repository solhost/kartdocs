# Kart API documentation (1.12.0)
## What is Kart?
Kart is a free inference provider, by the community for the community
# Client Integrity
To use the Kart API, you need to have a Kart Client Integrity Key (KCIK)
These are manually issued, in order to get one email solhost@tutamail.com
# Your request
You need to send a POST request to https://kart-j0it.onrender.com/v1/ with the following json:
```jsonc
{
"client_integrity": "YOUR_KEY_HERE",
"prompt": "Hello Kart",
// optional
"system": "Your system prompt here",
"history": {"role": "user": "old prompt"}
}
```
# Using Kart's response
Kart returns 2 JSON keys, `content` and 'model', as you can probably guess by the name, `model` contains the model name.
`content` contains the model's response
