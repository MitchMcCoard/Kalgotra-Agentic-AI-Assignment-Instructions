# Kalgotra-Agentic-AI-Assignment-Instructions
In this homework we'll be downloading Ollama to be able to run LLM machines locally on your laptop for free.
By the end of this tutorial you will:
- Install **Ollama**, a tool for running large language models (LLMs) locally on your laptop for free.
- Verify that the installation works by running a basic test command.
- Reflect briefly on your experience setting up a local LLM
should have installed Ollama and been able to get it running.

## **Part 1: Installation**

1. Go to the [Ollama website](https://ollama.com/download) and download the installer for your operating system (Mac, Windows, or Linux).
2. Follow the on-screen instructions to complete the installation.
3. Open a terminal (Command Prompt, PowerShell, or Terminal app, depending on your OS).
4. Run the following command to confirm Ollama is installed correctly:
	 `ollama --version`
## Part 2: Running Your First Model
1. Pull and run the `LLaMA 2` model with the following command
	`ollama run llama2`
2. Wait a few minutes for the LLM model to download (varies depending on WIFI connection)
3. When prompted, try it out!
4. Finish the session by typing `/bye`



## Part 3: Access it via API

Prerequisite [[Setup Postman Excercise]]

1. Open Postman
2. Create a new request
3. Set the request type to `POST`
4. In the URL field, enter: `http://localhost:11434/api/generate`
5. Select the body tab
6. Choose raw and set format to `JSON`
7. Copy the following JSON:
  ``` json
   {
	  "model": "llama2",
	  "prompt": "Write a haiku about computers."
	}
   ```
8. Click Send!
