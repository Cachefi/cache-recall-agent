Cache Agent

Welcome to the Cache Agent project! This is a simple but powerful agent designed to interact with the Recall network, utilizing LangChain and the Recall Agent Toolkit. The purpose of this agent is to demonstrate the integration of AI with decentralized storage and computation via Recall. Cache aims to efficiently manage and retrieve data with minimal setup.

Features

Efficient Data Storage: Cache can create and manage buckets in Recall.
AI Integration: Built on LangChain and OpenAI GPT-4 for natural language processing and reasoning.
Testnet Ready: Initially configured to work with Recall's testnet for experimentation.
Seamless Interaction: Using the Recall toolkit, the agent can store, retrieve, and manipulate data with ease.

Setup Instructions

Prerequisites
Before you get started, make sure you have the following:
- Node.js 20 or later
- NPM (Node Package Manager) or Yarn
- A code editor (Visual Studio Code, or your favorite IDE)

Installation

1. Clone this repository to your local machine:

    ```bash
    git clone https://github.com/yourusername/cache-agent.git
    cd cache-agent
    ```

2. Install the required dependencies:

    ```bash
    npm install
    ```

3. Set up your environment variables by creating a `.env` file in the root directory. This file should contain your Recall private key, Recall network, and OpenAI API key:

    ```
    RECALL_PRIVATE_KEY=your_private_key_here
    RECALL_NETWORK=testnet
    OPENAI_API_KEY=your_openai_api_key_here
    ```

    Note: Never share your `.env` file publicly! Keep your private key and API key safe.

4. Run the agent:

    ```bash
    npx tsx agent.ts
    ```

What’s Happening?

When you run the agent, it will:
- Create a bucket called "memories" in the Recall network.
- Store a note with the key "first-memory" and the content "This is my first memory."
- Retrieve that note and summarize the action it took.

.gitignore

We’ve included a `.gitignore` file to ensure that sensitive files like your `.env` file are never accidentally pushed to GitHub. This helps keep your private keys and other sensitive information safe.

Files Overview
- `agent.ts`: Contains the main logic for the agent, including how it interacts with Recall and processes requests.
- `.env`: Stores sensitive configuration variables like private keys and API keys (never share this file publicly).
- `.gitignore`: Tells Git which files to ignore, making sure sensitive information is never tracked.

Contributing

Feel free to contribute to the project! Here are some ways you can help:
Report any bugs you find
Suggest new features
Submit pull requests to fix issues or improve the agent

If you need help, feel free to reach out through the [GitHub Issues](https://github.com/yourusername/cache-agent/issues) or join our Discord community.

Next Steps

After you’ve set up and run your agent, you can:
Experiment with other Recall network functionalities
Submit your agent to a Recall competition
Improve the agent by adding more features or optimizing its performance

Credits

LangChain: A framework for developing applications powered by language models.
Recall: A decentralized storage and computational network.
OpenAI GPT-4: The AI language model that powers the intelligent capabilities of Cache.

License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
