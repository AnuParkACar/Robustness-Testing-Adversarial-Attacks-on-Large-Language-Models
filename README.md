# Robustness-Testing-Adversarial-Attacks-on-Large-Language-Models
LLMs can be easily manipulated using adversarial attacks. This project systematically tests LLMs against adversarial attacks, measure their robustness, and propose defenses

# 🤗 Hugging Face Setup for Local Mistral Inference

To run Mistral models locally via Hugging Face, follow the steps below:

## 1. Create or Log In to a Hugging Face Account

If you haven’t already, you’ll need a Hugging Face account.

🔗 Sign up or log in here: [https://huggingface.co/join](https://huggingface.co/join)

## 2. Accept Model License and Enable Access

Some models like **Mistral** require you to:

- Accept the model's license or terms of use.
- Enable **contact sharing** to gain access.

➡️ Visit the model page (e.g., [Mistral-7B-Instruct-v0.1](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.1)) and click **"Access repository"** if needed.

## 3. Generate a Hugging Face Access Token

To authenticate and download models programmatically, you’ll need a personal access token.

🔗 Generate a token here: [https://huggingface.co/settings/tokens](https://huggingface.co/settings/tokens)

- Make sure it has **read access**.
- Copy this token for later use.

## 4. Add Token to Scripts

When running inference locally (e.g., loading models with `transformers` or `AutoModelForCausalLM`), you’ll be prompted to enter the token or add it programmatically.

You can:
- Paste the token in the appropriate cell/block in the script.
- Or set it as an environment variable:
  ```bash
  export HUGGINGFACE_TOKEN=your_token_here
