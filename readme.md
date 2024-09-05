# ScribeStarter

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python Version](https://img.shields.io/badge/python-3.10%2B-blue)](https://www.python.org/downloads/)
[![Poetry](https://img.shields.io/badge/poetry-package%20manager-blue)](https://python-poetry.org/)

## Introduction

ScribeStarter represents the cutting edge of content creation technology, harnessing the power of artificial intelligence to revolutionize the blog writing process. Built on the robust crewAI framework, ScribeStarter automates and optimizes every stage of blog post production, from initial research and planning through to writing and final editing.

This innovative tool is designed to meet the evolving needs of developers, content marketers, and digital strategists who demand high-quality, SEO-optimized content at scale. By leveraging advanced AI models and integrating with powerful web scraping tools, ScribeStarter not only accelerates the content creation process but also ensures that each piece is well-researched, engaging, and primed for maximum online visibility.

## Core Capabilities

ScribeStarter's functionality extends far beyond simple text generation. At its core, the framework orchestrates a complex series of AI-driven processes:

1. Automated Research: ScribeStarter begins by scouring the web for relevant, up-to-date information on the given topic. It utilizes advanced web scraping techniques through Firecrawl integration to gather comprehensive data from authoritative sources.

2. Intelligent Planning: Based on the collected data, the AI analyzes and structures the information to create a coherent and logical outline for the blog post. This ensures that each piece has a solid foundation and flow.

3. AI-Powered Writing: Leveraging OpenAI's GPT models, ScribeStarter generates high-quality, human-like text that adheres to the planned structure while maintaining engagement and readability.

4. SEO Optimization: Throughout the writing process, ScribeStarter implements SEO best practices, including keyword optimization, meta description creation, and proper heading structure to enhance the content's search engine visibility.

5. Thorough Editing: Once the initial draft is complete, ScribeStarter's AI editor reviews the content for grammar, style, consistency, and factual accuracy, making necessary refinements to polish the final product.

6. Customizable Workflow: The framework allows for extensive customization of agents and tasks, enabling users to tailor the content creation process to their specific needs and brand voice.

## Getting Started

### Prerequisites

Before diving into ScribeStarter, ensure your development environment meets the following requirements:

- Python 3.10 or higher installed on your system
- Poetry package manager for efficient dependency management
- Active API keys for both OpenAI and Firecrawl services

### Installation Process

Follow these steps to set up ScribeStarter on your local machine:

1. Clone the ScribeStarter repository:
   ```
   git clone https://github.com/yourusername/ScribeStarter.git
   cd ScribeStarter
   ```

2. Set up a virtual environment to isolate the project dependencies:
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. Install Poetry if you haven't already:
   ```
   pip install poetry
   ```

4. Use Poetry to install project dependencies:
   ```
   poetry install
   ```

This process ensures that all necessary libraries and tools are properly installed and configured within your project environment.

### Configuration

Proper configuration is crucial for ScribeStarter to function correctly. Follow these steps:

1. In the project root directory, create a `.env` file by copying the provided example:
   ```
   cp .env.example .env
   ```

2. Open the `.env` file and input your API credentials:
   ```
   OPENAI_API_KEY=your_openai_api_key_here
   FIRECRAWL_API_KEY=your_firecrawl_api_key_here
   ```

   To obtain these essential API keys:
   - For OpenAI: Visit [OpenAI's website](https://openai.com/api/), create an account, and generate an API key.
   - For Firecrawl: Navigate to [Firecrawl's platform](https://firecrawl.com/), sign up for an account, and obtain your API key.

Ensure that these keys are kept confidential and never shared publicly or committed to version control.

## Utilizing ScribeStarter

To harness the power of ScribeStarter for your content creation needs, use the following command:

```
poetry run scribe-starter
```

This command initiates the ScribeStarter framework, beginning the automated blog post creation process. The system will guide you through any necessary inputs and keep you informed of its progress throughout the content generation lifecycle.

For more advanced usage, including customizing the AI agents, modifying the content creation pipeline, or integrating with your existing workflows, please refer to our comprehensive [Documentation](docs/README.md).

## Project Architecture

ScribeStarter is structured to ensure modularity, scalability, and ease of maintenance. Here's an overview of the project's architecture:

```
ScribeStarter/
├── src/
│   └── scribe_starter/
│       ├── config/
│       │   ├── agents.yaml    # Defines AI agent configurations
│       │   └── tasks.yaml     # Specifies content creation tasks
│       ├── tools/
│       │   ├── summarizer_tool.py    # Text summarization utility
│       │   └── custom_tool.py        # Extensible custom functionality
│       ├── __init__.py
│       ├── crew.py    # Core logic for AI crew management
│       └── main.py    # Entry point for the application
├── tests/
│   └── ...            # Comprehensive test suite
├── docs/
│   └── README.md      # Detailed documentation
├── .env.example       # Template for environment variables
├── .gitignore         # Specifies intentionally untracked files
├── pyproject.toml     # Project metadata and dependencies
├── LICENSE            # MIT License details
└── README.md          # This file
```

This structure allows for easy navigation, clear separation of concerns, and straightforward expansion of functionality as the project evolves.

## Contributing to ScribeStarter

We warmly welcome contributions from the community. Whether you're fixing bugs, improving documentation, or proposing new features, your input is valuable. To contribute:

1. Fork the repository and create your branch from `main`.
2. If you've added code that should be tested, add tests.
3. Ensure your code adheres to the project's coding standards.
4. Issue a pull request with a comprehensive description of your changes.

For more detailed information on how to contribute, please read our [Contributing Guidelines](CONTRIBUTING.md).

## Licensing

ScribeStarter is open-source software licensed under the MIT License. This permits use, modification, and distribution of the code, subject to the conditions outlined in the [LICENSE](LICENSE) file. We encourage you to read and understand these terms before using or contributing to the project.

---

ScribeStarter: Revolutionizing content creation through the seamless integration of AI and human creativity. Join us in shaping the future of digital content production.