# GitMagenticAgent

## 🌟 Overview
GitMagenticAgent is a robust and intelligent agent designed to automate and streamline Git operations. It leverages AI capabilities to interact with Git repositories, perform various tasks, and provide real-time updates. This project is ideal for developers and teams looking to simplify their Git workflows and integrate automation into their development processes.

## ✨ Features
- 🛠️ Clone repositories, create branches, and switch between branches.
- 📤 Commit and push changes to remote repositories.
- 🔄 Pull the latest changes and handle merge conflicts.
- 📝 Create and manage GitHub issues and pull requests.
- 📊 Fetch repository status and list branches.
- ⚡ Real-time task updates and artifact management.

## 📂 Project Structure
The project is organized as follows:

```
GitMagenticAgent/
├── .env                     # Environment variables
├── .gitignore               # Git ignore file
├── .python-version          # Python version file
├── agent_executer.py        # Main agent execution logic
├── agent.py                 # Core agent implementation
├── client.py                # Client to interact with the agent
├── main.py                  # Entry point for the application
├── pyproject.toml           # Project dependencies and configuration
├── README.md                # Project documentation
├── uv.lock                  # Dependency lock file

```

## 🛠️ Prerequisites
- Python 3.12 or higher
- Git installed on your system
- A GitHub personal access token (PAT) with appropriate permissions

## 🚀 Setup Instructions

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/utkarsh-alpuria/Agent_2_Agent.git
   cd Agent_2_Agent/GitMagenticAgent
   ```

2. **Install UV (if not already installed):**
   ```bash
   pip install uv
   ```

3. **Sync Dependencies:**
   ```bash
   uv sync
   ```

4. **Set Up Environment Variables:**
    **e.g.**
   - Create a `.env` file in the root directory and add the following:
     ```env
     AZURE_OPENAI_API_KEY=<your_azure_openai_api_key>
     AZURE_OPENAI_ENDPOINT=<your_azure_openai_endpoint>
     AZURE_OPENAI_API_VERSION=<api_version>
     AZURE_OPENAI_DEPLOYMENT_NAME=<deployment_name>
     AZURE_OPENAI_MODEL_NAME=<model_name>
     GITHUB_TOKEN=<your_github_token>
     ```

5. **Run the Application:**

   - **To Run the agent server**
   ```bash
   uv run main.py
   ```
   After running this command, the agent server starts.
   You can see the agent card at http://localhost:9999/.well-known/agent-card.json

   Now you can change the task in client.py file according to the git operations you want the agent to perform.
   - **To Run the client**
   ```bash
   uv run client.py
   ```

## 💡 How to Use
- **Agent Execution:** Use `main.py` to start server and execute Git-related tasks.
- **Client Interaction:** Use `client.py` to interact with the agent and send queries.


## 🌐 What This Project Does
GitMagenticAgent simplifies Git operations by automating repetitive tasks and providing an AI-powered interface for interacting with repositories. It is designed to:
- Enhance productivity by reducing manual effort.
- Provide real-time updates on task progress.
- Integrate seamlessly with GitHub for issue and pull request management.

## 🤝 Contributing
Contributions are welcome! Please fork the repository and submit a pull request with your changes.

## 📜 License
This project is licensed under the MIT License. See the LICENSE file for details.

## 📧 Contact
For any questions or support, please contact the repository owner at [utkarsh-alpuria](https://github.com/utkarsh-alpuria).
