AI-Powered Code Review Assistant
This project is a proof-of-concept tool designed to automate the code review process using AI. It extracts Git diffs, performs static analysis with Flake8, runs tests using Pytest, and leverages OpenAI's GPT-3.5-turbo to deliver a human-like code review verdict. The verdict provides either an "approve" decision or "request changes" along with detailed reasoning and suggestions.

Features
Git Diff Extraction: Compares the current code changes against the main branch (or a specified branch) to isolate the differences.

Static Analysis: Uses Flake8 to catch code style issues and potential bugs.

Automated Testing: Runs your project's test suite with Pytest to ensure functional correctness.

AI-Driven Code Review: Summarizes code changes, static analysis, and test results; then provides an AI-generated review using OpenAI's GPT-3.5-turbo.

Clear Feedback: Presents a clear verdict (approve or request changes) along with detailed insights similar to a human code reviewer.

Disclaimer
Important:
This project is for educational and proof-of-concept purposes only. Do not hardcode your API keys or other sensitive credentials in production code. Instead, use environment variables or secure vault solutions to manage your keys safely.

Installation
Clone the Repository:

bash
Copy
git clone https://github.com/yourusername/code_review_assistant.git
cd code_review_assistant
Install Required Packages: Ensure you have Python installed, then run:

bash
Copy
pip install openai flake8 pytest
Usage
Initialize or Verify a Git Repository:
Ensure that your project is a valid Git repository. If not, run:

bash
Copy
git init
Run the Code Review Assistant: Execute the script with the branch you want to review:

bash
Copy
python code_review_assistant.py <branch-name>
Replace <branch-name> with the actual branch name (e.g., feature-branch).

View the Results: The script will display:

The list of changed files.

Output from Flake8 static analysis.

Test results from Pytest.

The AI-generated code review verdict with detailed feedback.

Contributing
Contributions are welcome! Feel free to fork the repository, make enhancements or fixes, and submit a pull request.

License
This project is licensed under the MIT License. See the LICENSE file for details.
